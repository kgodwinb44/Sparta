# Data Concepts

---

## Data Format

### Data Types

- int, char, float, boolean

### SQL

- Date and Time Format YY/MM/DD

- Key-Value Pairs is a set of two linked data items e.g. Movie, Genre, Actor, Year

### File Format/ Types

- .txt, .yml, .csv, .xml, .json, .dat

---

## Data Storage

### ETL (Extract, Transform, Load)
- Extract the data, Tranform the data, Load the data

### Relational Data Processing

**OLTP (Online Transaction Processing)**
- Database Transcations (payments recived, booking, orders taken, stock price movement)
- Requires high degree of normalisation
- Heavy write (a lot of updating of the DB), low read (not really looking at the DB)

**OLAP (Online Analytic Processing)**
- Designed to extract buisness itnelligence from OLTP
- Adds layers of abstraction and aggregation
- Heavy read, low write

**ACID (Atomicity, Consistency, Isolation, Durability)**
- **Atomicity** Each transaction must be treated as a single unit
- **Consistency** Each transaction must result in a valid database state
- **Isolation**
- **Durability**
- A set of principles that guarantee the reliability and integrity of database transactions

### Data Warehouse

- A system that integrates and centralizes data from multiple sources for the purpose of reporting, analysis, and business intelligence
- Designed for data analysis
- Only stores critical data
- Slices of the warehouse stored as Data Marts e.g. Mart Finance, Mart Sales, Mart Personal
- Examples Amazon Redshift, Snowflake, Oracle, Microsoft Azure Synapse Analytics

**Data Warehouse Approaches**

- Inmon Architecture (Top Down Approach, Normalised Data Warehouse created first, Data the summarised and distributed out to Data Marts, Harder to set up, easier to maintain)

- Kimbal Architecture (Bottom up approach, Seperate Data Marts created first, then place the warehouse around them, Easier to set up, harder to maintain)

**Dimensional Modelling**

- Kimbal Architecutre
- Instead of representing tables, represents people/ items/ objects
- Contain data corresponding to instances of objects (Product details, calendar info)
- Contains dimensional data

**Start Schema**

- A databse schema used in data warehousing to organise into central fact table surrounded by dimensional tables
- Fact tables join denormalised dimensional tables using foreign keys

**Snowflake Schema**

- Dimension tables are normalised
- Reducing data redundancy but potentially increasing query complexity

---

## Data Lakes

- Newer, made possible with Big Data technology
- Stores structured and unstructred data in original form
- Processed when analysis is needed, not when stored (Schema-On-Read)
- Low cost storage vs Warehouse
- Highly scalable, Highly agile

## Data Lakehouses

- Taakes the best aspect of Data Warehouses and Data Lakes
- Offers some strcutre and control, including ACID principles
- Flexible and scalable
- Often the architecture can be decoupled 
- Governace can be difficult

---

# Acitivty

**Difference between Databses, Date Warehouses and Data Lakes**
- Databases store current data for application and transactional operations
- Data Warehouses aggregates historical data from multiple sources for analysis often strcutred and semi-structred
- Data Lakes stores vast amounts of raw, structured, semi-stuctred and unstrcutered data for exploration and analaysis