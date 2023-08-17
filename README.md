# Python MySQL Beginners Guide

<br/><br/>

## ! Work in Progress... ! 

<br/><br/>

## Installation
### ◘ Software and Package Specification
* **Python**~=3.11.3
* **jupyter**~=1.0.0
* **mysql-connector-python**~=8.1.0

<br/>

### ◘ Downloading MySQL
* *MySQL* can be downloaded from the following link: <br/>
[Download MySQL for Python](https://dev.mysql.com/downloads/mysql/) 
* Additionally, the *MySQL workbench* can be downloaded as well:  <br/>
[Download MySQL Workbench](https://dev.mysql.com/downloads/workbench/)

<br/>

### ◘ Installing MySQL
For the database to function, Python requires a MySQL driver to access the MySQL database. In order to install the Python-mysql-connector module, PIP and Python must be preinstalled. Afterward, run the below command in the terminal. In Jupyter, the console commands can be executed by the ‘!’ sign before the command within the cell. To install any modules effectively, the *sys* python package is imported `import sys`. Next the following command is used to confirm the installation, 
```
> !{sys.executable} -m pip install mysql-connector-python
```
Then, the MySQL server can be connected using the *connect()* function. Note that the *username* and *password* fields are user-defined. The code below illustrates proper evaluation procedure of the MySQL connection: 
```py3
# Importing required libraries
import mysql.connector
  
db = mysql.connector.connect(
  host ="localhost",
  user ="user",
  password ="user"
)
 
print(db)
  
# Disconnecting from the server
db.close()
```
Therefore, the output will be displayed as follows:
```py3
<mysql.connector.connection.MySQLConnection object at 0x000002653D8DF3A0>

```
