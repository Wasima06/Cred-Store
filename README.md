# Cred-Store

Project Summary
This Node.js Express application provides a CRUD (Create, Read, Update, Delete) interface for managing user data in a MySQL database. It leverages the following technologies:

Express.js: Web framework for building web applications
faker.js: Library for generating realistic fake data (used for initial data population)
mysql2: Driver for interacting with MySQL databases
EJS: Templating engine for generating dynamic HTML pages

Key Functionalities
Get Total User Count: Retrieves the total number of users from the database.
Get All Users: Fetches all user records from the database.
Edit User: Allows modifying a user's username (with password verification).
Add New User: Enables creating new user entries in the database.
Delete User: Provides functionality to delete users from the database (with password confirmation).

Project Usage
1. Prerequisites:
Node.js and npm (or yarn) installed on your system.
A MySQL database server running with a database named delta_app created.
Update the database connection details (host, user, password) in the code (connection variable) if necessary.
2. Installation:
Clone or download this repository.
Navigate to the project directory in your terminal.
Run npm install (or yarn install) to install dependencies.
3. Database Setup (Optional):
If you don't have a user table in your delta_app database, create it using a MySQL client with the following schema:

CREATE TABLE user ( 
  id VARCHAR(255) PRIMARY KEY, 
  username VARCHAR(255) NOT NULL, 
  email VARCHAR(255) NOT NULL,
  password VARCHAR(255) NOT NULL
);  
4. Running the Application:
Run node app.js (or npm start if using a package.json script) to start the server.
The application will listen on port 8080 by default. Access it in your browser at http://localhost:8080.
