# Databases

### Typea of Databases
- Hierarchical Databases
- Relational Databases
- Graph Databases
- Centralised Databases

### Primary and Foreign Keys

**Primary Keys**
- A primary key is a field used to uniquely identify every record in the database e.g. ID

**Foreign Key**
- A foreign key is a primary key from one table that appears in another table to link the two together

![](./images/PrimaryForeignKey.png)

## Data Modelling

### What is Data Modelling
- Data modelling is the process of creating a visual representation of data structres and relationships within a system

**Data Model**
- Data models are abstract representations that define how data is structured, organised, and related within a system.

![](./images/DataModel.png)

## ERD's (Entity Relationship Diagram)
- An ERD is a visual representation of how items in a database interact and relate to each other

## Crows Feet Notation
- Crows foot notation is a visual language used in ERD to depict the type of relationship between the entities


![](./images/CrowsFoot.png)

## Normalisation and Forms 1NF, 2NF, 3NF (Normal Form)
- Normalisation is a database design principle for oragnising to data in a way which is consistent

##3 Types of Normalisation**

**The First Normal Form – 1NF**
- For a table to be in the first normal form, it must meet the following criteria:

- a single cell must not hold more than one value (atomicity)
- there must be a primary key for identification
- no duplicated rows or columns
- each column must have only one value for each row in the table

**The Second Normal Form – 2NF**
- The 1NF only eliminates repeating groups, not redundancy. That’s why there is 2NF.

- A table is said to be in 2NF if it meets the following criteria:

- it’s already in 1NF
- has no partial dependency. That is, all non-key attributes are fully dependent on a primary key.
- The Third Normal Form – 3NF
- When a table is in 2NF, it eliminates repeating groups and redundancy, but it does not eliminate transitive partial dependency.

-This means a non-prime attribute (an attribute that is not part of the candidate’s key) is dependent on another non-prime attribute. This is what the third normal form (3NF) eliminates.

**So, for a table to be in 3NF, it must:**

-be in 2NF
-have no transitive partial dependency.