# Databases – COM-424.1
## American University of Central Asia (AUCA)  

_Department of Software Engineering_  
📌 Instructor: _Ph.D., Associate Professor Gulzada Esenalieva_     
📌 Semester: Fall 2025      
📌 Credits: 6

### 📖 Course Overview   

This repository contains my lab work and final project for the Databases (COM-424.1) course.
The course is practice-oriented, focusing on PostgreSQL, SQL queries, ER modeling, database design, transactions, indexing, and backup strategies.      

The goal of this repository is to:  
Document weekly lab assignments             
Provide code, queries, and database schemas     
Showcase the final project implementation

### 📂 Repository Structure  

├── labs/   
│   ├── lab01-introduction.sql  
│   ├── lab02-installation.md   
│   ├── lab03-basic-psql.sql    
│   ├── lab04-first-query.sql   
│   ├── ...     
│   └── lab17-backup.sql            
│   
├── project/    
│   ├── er-diagram.png  
│   ├── schema.sql  
│   ├── queries/    
│   │   ├── basic-queries.sql   
│   │   ├── advanced-queries.sql    
│   │   └── joins.sql   
│   ├── transactions.sql    
│   ├── indexing.sql    
│   └── backup-restore.md   
│   
├── docs/   
│   ├── syllabus.pdf    
│   ├── oracle-certificate.pdf  
│   └── report.md   
│   
└── README.md

## 🚦 Final Project: Smart City Traffic & Transportation Database System
### 🧠 Project Concept   
This database project is developed as part of a larger research initiative on machine learning algorithms for road traffic optimization.
The system is designed to collect, store, and analyze real-time and historical urban traffic data from sensors, cameras, and GPS devices.
The resulting database will later be used as a data foundation for predictive modeling and optimization algorithms in my senior thesis.    

### 🎯 Objectives
Design a normalized relational database for managing traffic flow and signal data.
Enable efficient SQL queries for congestion analysis and trend visualization.
Prepare the dataset for future integration with ML models (e.g., regression, clustering).
Support both real-time and batch data updates with ACID-compliant transactions.

### 🧩 Database Design
Main Entities:  
Roads (road_id, name, lanes, length, district_id)   
Intersections (intersection_id, location, signal_type)  
Sensors (sensor_id, type, location, road_id)    
Traffic_Data (record_id, sensor_id, timestamp, vehicle_count, avg_speed, congestion_level)  
Traffic_Lights (light_id, intersection_id, phase, duration, updated_at) 
Districts (district_id, name, population, avg_traffic_volume)   
ER Diagram: project/er-diagram.png  
### 💾 Implementation
Database: PostgreSQL    
Data Population: CSV import & PL/pgSQL scripts  
Optimization: Indexing on timestamp, road_id, and intersection_id   
Transactions: Used for batch updates during signal changes  
Backup: Automated daily dump with pg_dump   
### 🔍 Example Queries
Find top 5 most congested intersections per hour    
Calculate average vehicle speed per district during rush hours  
Detect abnormal traffic spikes from sensor data 
Suggest optimal signal timing adjustments using aggregated data 
### 🚀 Future Integration    
This database will be directly extended in my senior thesis:    
“Machine Learning Algorithms for Road Traffic Optimization in Bishkek.” 
The structured data collected through this database will serve as a foundation for building and testing predictive ML models to improve city traffic efficiency.    
### 🛠️ Technologies Used
PostgreSQL (main database system)   
pgAdmin (GUI for PostgreSQL)    
psql (command-line tool)    
GitHub/GitLab (version control & submissions)   
### 📚 Learning Outcomes
By completing this course and repository, I will be able to:    
✔ Understand relational database concepts and architecture  
✔ Design ER-diagrams and normalize relational databases 
✔ Write SQL queries of varying complexity   
✔ Implement and manage transactions (ACID)  
✔ Create indexes and analyze performance    
✔ Perform backup, restore, and data migration   
✔ Understand basic NoSQL concepts   
### 📑 Course Requirements   
Completion of all lab assignments   
Submission of Oracle Academy Database Course certificate    
Team-based final project uploaded to GitHub/GitLab  
### ⚖️ Academic Integrity   
All code and assignments in this repository represent my own work for educational purposes under AUCA’s academic honesty policy. Plagiarism or unauthorized sharing of solutions is strictly prohibited.