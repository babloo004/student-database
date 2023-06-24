# student-database
# Student Database

This repository contains a database for storing student details, including their CGPA, branch, and scholarship information. The database schema and sample data are provided to help you get started.

## Table of Contents

- [Database Schema](#database-schema)
- [Sample Data](#sample-data)
- [Queries](#queries)
- [Contributing](#contributing)
- [License](#license)

## Database Schema

The database consists of the following table:

### student_details

| Column        | Data Type | Description                          |
| ------------- | --------- | ------------------------------------ |
| student_id    | INT       | Unique identifier for each student    |
| first_name    | VARCHAR   | First name of the student             |
| last_name     | VARCHAR   | Last name of the student              |
| cgpa          | DECIMAL   | Cumulative Grade Point Average        |
| branch        | VARCHAR   | Branch of study                       |
| scholarship   | VARCHAR   | Scholarship information               |

## Sample Data

Sample data has been provided in the `sample_data.sql` file. It includes a set of student details with their respective CGPAs, branches, and scholarship information. You can import this data into your database to have some initial records for testing and exploration.

To import the sample data, follow these steps:

1. Create a new database in your MySQL server (if not already created).
2. Open a terminal or command prompt and navigate to the directory containing the `sample_data.sql` file.
3. Run the following command to import the data:
   ```
   mysql -u <username> -p <database_name> < sample_data.sql
   ```
   Replace `<username>` with your MySQL username and `<database_name>` with the name of the database where you want to import the data. You will be prompted to enter your MySQL password.
4. Once the import is complete, you will have the sample data in your database.

## Queries

This section provides some sample queries that you can execute on the database to retrieve and manipulate student data. Feel free to modify these queries or create your own based on your requirements.

1. Retrieve all students' details:
   ```sql
   SELECT * FROM student_details;
   ```

2. Retrieve students with a CGPA above a certain threshold:
   ```sql
   SELECT * FROM student_details WHERE cgpa > 8.0;
   ```

3. Retrieve students from a specific branch:
   ```sql
   SELECT * FROM student_details WHERE branch = 'Computer Science';
   ```

4. Update a student's scholarship information:
   ```sql
   UPDATE student_details SET scholarship = 'Full' WHERE student_id = 1234;
   ```

These are just a few examples to get you started. Explore the database and create more queries based on your specific needs.

## Contributing

Contributions to this project are welcome. If you have any suggestions, improvements, or bug fixes, please submit a pull request. Make sure to follow the project's coding conventions and provide a clear description of your changes.



Please feel free to customize this README file based on your specific database and requirements. Provide clear instructions, usage examples, and any other relevant information to help users understand and utilize the database effectively.
