# Final-Lab-Task-2

This portfolio highlights my understanding of MySQL database creation through a simplified student assignment submission system. It details the step-by-step development of tables for students, assignments, and submissions, using data types, relationships, and constraints such as primary keys and foreign keys to construct a functional relational schema.

# Step by Step Processs

## Step 1. Create the student table:
* Define username as a VARCHAR (50)
* Set username as the Primary Key

## Step 2. Create the assignment table:
* Define shortname as a VARCHAR (50) and set it as the Primary Key
* Define due date as a DATE and make it NOT NULL
*Define url as VARCHAR (255), which can be null

## Step 3. Create the submission table:
* Define username and shortname as VARCHAR (50)
* Define version as an INT
* Define submit date as a DATE and make it NOT NULL
* Set a composite primary key using (username, shortname, version)
* Add foreign key constraints referencing the student and assignment tables

# Table Relationships:

- Many-to-One with student: Each submission belongs to one student.

- Many-to-One with assignment: Each submission is for one assignment.

- This models a Many-to-Many relationship between students and assignments, with version tracking multiple submissions.

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

