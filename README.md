# Python MySQL Beginners Guide

<br/><br/>

## ! Work in Progress... ! 

<br/><br/>

# Installation
## ◘ installing MySQL
For the database to function, Python requires a MySQL driver to access the MySQL database. In order to install the Python-mysql-connector module, PIP and Python must be preinstalled. Afterward, run the below command in the terminal.
```
> pip install mysql-connector-python
```

```py3
# importing required libraries
import mysql.connector
  
dataBase = mysql.connector.connect(
  host ="localhost",
  user ="user",
  password ="password"
)
 
print(dataBase)
  
# Disconnecting from the server
dataBase.close()
```
