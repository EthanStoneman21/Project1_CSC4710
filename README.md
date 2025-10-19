**Project description**

Consider to create the user table using the following CREATE TABLE stmt (feel free to revise it): 


```SQL
CREATE TABLE Users (
  userid INT AUTO_INCREMENT PRIMARY KEY,
  username VARCHAR(50),
  password VARCHAR(255),
  firstname VARCHAR(50),
  lastname VARCHAR(50),
  salary FLOAT,
  age INT,
  registerday DATE,
  signintime DATETIME
);
```

**How to run the sample code**
1. We will use the Apache web server. Create the first webpage index.html under ```C:\xampp\htdocs>``` (or similar directory where you installed XAMPP) and point your browser to [http://localhost/index.html](http://localhost/index.html). You should see your first webpage. The purpose of this step is to confirm that the Web server is running, and understand the ROOT URL points to the path location: C:\xampp\htdocs or similar directory in your file system. 
2. At ```C:\xampp\htdocs```, run ```git clone https://github.com/EthanStoneman21/Project1_CSC4710.git``` to copy the whole sample code to the current directory.
3. Now you can access the Frontend via [http://localhost/Project1_CSC4710/Frontend/index.html](http://localhost/Project1_CSC4710/Frontend/index.html).
4.  Under the database ```web_app```, create an empty table as follows: 
```SQL
create table names (id INTEGER PRIMARY KEY AUTO_INCREMENT, name VARCHAR(100), date_added DATE);
```
5. Go the Backend directory ```C:\xampp\htdocs\database_javascript\project1\Backend```.
6. npm install express mysql cors nodemon dotenv
7. Start the Backend by running ```npm start```.
8. Feel free to access some of the Backend endpoints directly such as [http://localhost:5050/getAll](http://localhost:5050/getAll). You will only receive JSON data without nice rendering. 
9. Now you can interact with the Frontend [http://localhost/database_javascript/project1/Frontend/index.html](http://localhost/database_javascript/project1/Frontend/index.html).
---------------------------------------



