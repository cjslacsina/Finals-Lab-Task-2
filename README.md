# Final-Lab-Task-2
This portfolio demonstrates my understanding of MySQL database creation through a simplified student assignment submission system. It outlines the step-by-step process of developing tables for students, assignments, and submissions, utilizing data types, relationships, and constraints like primary keys and foreign keys to build a functional relational schema.

**Step-by-Step Process**

### **Step 1: Create the Student Table:**

* Define `username` as a `VARCHAR(50)`.
* Set `username` as the Primary Key.

### **Step 2: Create the Assignment Table:**

* Define `shortname` as a `VARCHAR(50)` and set it as the Primary Key.
* Define `due_date` as a `DATE` and set it as `NOT NULL`.
* Define `url` as a `VARCHAR(255)`, which can be `NULL`.

### **Step 3: Create the Submission Table:**

* Define `username` and `shortname` as `VARCHAR(50)`.
* Define `version` as an `INT`.
* Define `submit_date` as a `DATE` and set it as `NOT NULL`.
* Set a composite primary key using `(username, shortname, version)`.
* Add foreign key constraints referencing the `student` and `assignment` tables.

### **Table Relationships:**

* **Many-to-One with Student:** Each submission belongs to one student.
* **Many-to-One with Assignment:** Each submission is for one assignment.
* **Many-to-Many between Students and Assignments:** This models the relationship where each student can submit multiple versions of assignments, with version tracking each submission.


# Screenshots
# Query Statements:
## 1. Student Table:
 ![Image]()

## 2. Assignment Table:
![Image]()

## 3. Submission Table:
![Image]()

# Table Structure
## 1. Student Table:
![Image]()

## 2. Assignment Table:
![Image]()

## 3. Submission Table:
![Image]()

# Entity-Relationship Diagram (EER)
![Image]()
