# Data Transfer Script: `news` to `kf_docmnt`
This Python script is designed to transfer data from the news table to the kf_docmnt table within a MySQL database. It demonstrates basic database operations using the mysql-connector-python library.

## Prerequisites
  *   Python 3.x: Ensure Python 3.x is installed on your machine.

* MySQL Server: A running MySQL server with a database named NEWSINFO.

 * MySQL Connector/Python: The mysql-connector-python library must be installed. Install it using pip if you haven't already:

bash
Copy code
*                pip install mysql-connector-python
Database Schema

** news Table:
* portalid (int)
* town (varchar)
* news (text)
* date (date)
  
**  kf_docmnt Table:
* portalid (int)
* town (varchar)
* news (text)
* date (date)
Ensure that both tables are correctly set up in your NEWSINFO database to match the schema outlined above.

## Script Overview

The script transfers data from the news table to the kf_docmnt table. It retrieves all rows from the news table and inserts them into the kf_docmnt table.

### How It Works
1. Connect to the Database: Establishes a connection to the MySQL server and selects the NEWSINFO database.
2. Retrieve Data: Executes a query to fetch all rows from the news table.
3. Insert Data: Inserts the fetched rows into the kf_docmnt table.
4. Error Handling: Catches and displays any errors that occur during execution.
5. Resource Management: Ensures that database resources are properly closed after operations.
 ### Instructions
1. Update Database Credentials: Modify the database connection parameters in the script to match your MySQL server settings.
2. Run the Script: Execute the Python script to perform the data transfer.
3.Verify Data: Check the kf_docmnt table to ensure the data has been successfully transferred.
### Error Handling
*  Connection Errors: Handles issues related to connecting to the MySQL server and provides relevant error messages.
* Query Execution Errors: Captures errors that occur during SQL query execution and outputs informative messages.


Contact
For any questions or feedback, please contact sayprincekumar20@gmail.com
