## Student Management System (SMS) Overview:

Introduction:

The Student Management System (SMS) is a comprehensive solution designed to streamline and organize the management of student information within educational institutions. This system aims to provide an efficient and user-friendly platform for administrators to handle student data with ease.

Technical Implementation:
The system employs a relational database management system (RDBMS) for data storage and retrieval, utilizing MySQL as the backend database. The connection between Python and MySQL is established using the MySQL Connector. This ensures a robust and reliable foundation for managing vast amounts of student information.

Installation Process:

Install MySQL Python Connector:

The system requires the installation of the MySQL Python connector, which serves as the bridge between Python and the MySQL database.
bash
Copy code
pip install mysql-connector-python
MySQL Installation:

MySQL itself needs to be installed to create and manage the database. This involves installing the MySQL server and setting up the necessary configurations.
bash
Copy code
# Example command for MySQL installation
sudo apt-get install mysql-server
Features:

Login and Register:

The system incorporates a secure login panel that allows administrators to register themselves and subsequently log in. This feature ensures that only authorized personnel can access and manage student data.
Adding New Student:

The SMS facilitates the addition of new student records with relevant details such as personal information, contact details, and enrollment information. This feature ensures the systematic entry of updated student data into the database.
Viewing Students:

Administrators can easily view the entire list of students enrolled in the institution. This feature provides a comprehensive overview of the student body, aiding in better decision-making and administrative planning.
Searching Student:

The system includes a powerful search functionality that enables administrators to quickly locate specific student records based on various criteria. This feature enhances accessibility and reduces the time required to retrieve specific information.
Updating Student:

Administrators have the ability to update student information as needed. This includes modifications to personal details, contact information, or enrollment status. This feature ensures that the database remains current and accurate.
Deleting Student:

In cases where a student leaves the institution or other circumstances necessitate removal from the database, administrators can use the deletion feature. This ensures the maintenance of a clean and up-to-date student database.
  
## MySQL Table Structure


### Admin Table

| Field    | Type         | Null | Key | Default | Extra |
|----------|--------------|------|-----|---------|-------|
| id       | varchar(50)  | YES  |     | NULL    |       |
| password | varchar(100) | YES  |     | NULL    |       |
 


### Student Information Table

| Field      | Type         | Null | Key | Default | Extra |
|------------|--------------|------|-----|---------|-------|
| sch_no     | int          | NO   | PRI | NULL    |       |
| name       | varchar(100) | YES  |     | NULL    |       |
| class      | varchar(50)  | YES  |     | NULL    |       |
| fee_status | varchar(100) | YES  |     | NULL    |       |
| age        | int          | YES  |     | NULL    |       |
| email      | varchar(150) | YES  |     | NULL    |       |
| phone      | varchar(150) | YES  |     | NULL    |       |


## Deployment

To deploy this project just run .py files.
