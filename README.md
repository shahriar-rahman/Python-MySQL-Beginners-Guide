# Python MySQL Beginners Guide

<br/><br/>

### ! Work in Progress... ! 

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
For the database to function, Python requires a MySQL driver to access the MySQL database. In order to install the *Python-mysql-connector* module, **pip** and **Python** must be preinstalled. In **Jupyter Notebook**, the console commands can be executed by the *‘!’* sign before the command within the cell. To install any modules effectively, the *sys* python package is imported `import sys`. Next, the following command is used to confirm the installation:
```
> !{sys.executable} -m pip install mysql-connector-python
```

<br/>

### ◘ Connection Evaluation
The MySQL server can be connected using the *connect()* function. Note that the *username* and *password* fields are user-defined. The code below illustrates a proper evaluation procedure for the MySQL connection: 
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
A more thorough approach, including all the codes and installation, can be explored [here](https://github.com/shahriar-rahman/Python-MySQL-Beginners-Guide/blob/main/notebooks/1-Test-Connection.ipynb).

<br/>

### ◘ Supplementary Resources
* https://jupyter.org/
* https://pypi.org/project/mysql/
* https://pypi.org/project/mysql-connector-python/
* https://dev.mysql.com/downloads/mysql/
* https://dev.mysql.com/downloads/workbench/

<br/><br/>

## License
### ◘ MIT License

Copyright (c) 2023 Shahriar Rahman

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

<br/>

===========================================================================

