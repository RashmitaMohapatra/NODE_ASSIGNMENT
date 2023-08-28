# NODE_ASSIGNMENT
**USER AND ROLE MANAGMENT SYSTEM**
This project implements a User and Role Management System with different user roles and permissions using SQL Workbench, Node.js, and React.js. The system provides authentication through JWT, allows the creation of different user types with varying levels of access, and enables CRUD operations on users and feeds based on their roles. Additionally, it supports logging functionality accessible only to the super admin.

**FEATURES**
User Roles: The system has three user roles: Super Admin, Admin, and Basic.
Authentication: User authentication is implemented using JWT (JSON Web Tokens).
Super Admin: There can be only one super admin who has access to every feed. The super admin can create other user types, manage their roles, and provide access to feeds. The super admin can perform CRUD operations on feeds and grant delete access to admins for specific feeds.
Admins: Admin users can create and delete basic users, provide access to specific feeds, and delete feeds based on permissions. Admins cannot create/update/delete other admin users.
Basic Users: Basic users can read feed details that they have been granted access to. They cannot access other feeds or user information.
CRUD Operations: Users with appropriate permissions can perform CRUD operations on both users and feeds.
Logging: Only the super admin has access to logs, which can provide insights into system activities.
Technologies Used
Frontend: React.js
Backend: Node.js
Database: SQL Workbench (Assumed relational database)
Authentication: JSON Web Tokens (JWT)

**SETUPS**
1. Clone the Repository: Clone this repository to your local machine.
  bash--
  git clone https://github.com/your-username/your-repo-name.git
2. Backend Setup:
     a. Navigate to the backend directory.
     b. Install backend dependencies.
        bash--cd backend
        npm install
     c. Set up your database configurations in config.js.
     d. Start the backend server.
         bash--npm start
3.Frontend Setup:
    Navigate to the frontend directory.
    Install frontend dependencies.
   bash-- cd frontend
          npm install
   Set up the API endpoint in src/config.js.
   Start the frontend development server.
   bash-- npm start
4.Access the Application:
 Open your browser and navigate to http://localhost:3000 to access the frontend.


**FOLDER STRUCTURE**
backend/: Backend server code and configurations.
frontend/: Frontend React application code.
database/: SQL schema and scripts.
docs/: Additional documentation files.

**MYSQL WORKBENCH SETUP**

Install MySQL Server:
If you haven't already, you need to install MySQL Server on your machine or a remote server. You can download it from the official MySQL website: https://dev.mysql.com/downloads/

During installation, you will set a root password for your MySQL server. Remember this password, as you'll need it to configure MySQL Workbench.

Install MySQL Workbench:
Download and install MySQL Workbench from the official MySQL website: https://dev.mysql.com/downloads/workbench/

Launch MySQL Workbench:
Once installed, launch MySQL Workbench.

Create a New Connection:

In MySQL Workbench, click on the "+" icon next to "MySQL Connections" in the home screen or select "Database" > "Connect to Database" from the top menu.
Connection Setup:

Give your connection a name in the "Connection Name" field.
Fill in the following details:
Hostname: Usually localhost if MySQL is on the same machine. If remote, enter the IP or hostname of the remote server.
Port: The default port for MySQL is 3306.
Username: Use root or another MySQL user you've set up.
Password: Enter the password you set during MySQL Server installation.
Click "Test Connection" to verify that your connection details are correct.
Connect to the Database:

Once the test is successful, click "OK" to close the test window.
Click "OK" again to save the connection settings.
Your new connection should now appear under "MySQL Connections."
Managing Databases and Tables:

Double-click on your connection to open it.
You can create, manage, and query databases and tables using the various tabs and tools in MySQL Workbench.
SQL Development:

Use the "Query" tab to write and execute SQL queries.
You can design, modify, and analyze your database schema using the "Schema" tab.
Remember that MySQL Workbench provides a graphical interface to interact with your MySQL database, making it easier to manage databases, tables, and queries. It's a powerful tool for developers and database administrators.

Note: If you encounter any issues during setup or connection, make sure your MySQL Server is running and that you have the correct host, port, username, and password. Additionally, be cautious when working with databases and running queries to avoid accidental data loss or corruption.







   


