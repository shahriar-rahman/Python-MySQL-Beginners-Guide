# Python MySQL Beginners Guide

<br/><br/>

## ! Work in Progress... ! 

<br/><br/>

# Installation
## ◘ Downloading MySQL
* MySQL can be downloaded from the following link: <br/>
[Download MySQL for Python](https://dev.mysql.com/downloads/mysql/) 
* Additionally, the MySQL workbench can be downloaded as well:  <br/>
[Download MySQL Workbench](https://dev.mysql.com/downloads/workbench/)

<br/>

## ◘ Installing MySQL
For the database to function, Python requires a MySQL driver to access the MySQL database. In order to install the Python-mysql-connector module, PIP and Python must be preinstalled. Afterward, run the below command in the terminal.
```
> pip install mysql-connector-python
```
Then, the MySQL server can be connected using the *connect()* function. The code below illustrates a proper testing of the MySQL connection: 
```py3
# Importing all the required libraries
import mysql.connector
  
db = mysql.connector.connect(
  host ="localhost",
  user ="user",
  password ="password"
)
 
print(db)
  
# Disconnecting from the server
dataBase.close()
```
