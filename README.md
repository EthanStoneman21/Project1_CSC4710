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
2. At ```C:\xampp\htdocs```, run ```git clone https://github.com/shiyonglu/database_javascript.git``` to copy the whole sample code to the current directory.
3. Now you can access the Frontend via [http://localhost/database_javascript/project1/Frontend/index.html](http://localhost/database_javascript/project1/Frontend/index.html).
4. You can configure parameters directly in dbServices.js and app.js. Here, we achieve this by configuring parameters using the .env file. Configure the MySql database according to ```C:\xampp\htdocs\database_javascript\project1\Backend\dotenv```, that is, to create a database called ```web_app``` and a user ```john``` with password ```1234``` via the Admin interface ```http://localhost/phpmyadmin/```. The user ```john``` will be granted with all priviledges for the ```web_app``` database. To get started, you might also change the dotenv file as follows to only use the root user:
```javascript
PORT=5050
DB_USER=root
PASSWORD=
DATABASE=web_app
DB_PORT=3306
HOST=localhost
```
5. You need to rename dotenv to .env by command ```move dotenv .env```. 
6.  Under the database ```web_app```, create an empty table as follows: 
```SQL
create table names (id INTEGER PRIMARY KEY AUTO_INCREMENT, name VARCHAR(100), date_added DATE);
```
7. Go the Backend directory ```C:\xampp\htdocs\database_javascript\project1\Backend```.
8. npm install express mysql cors nodemon dotenv
9. Start the Backend by running ```npm start```.
10. Feel free to access some of the Backend endpoints directly such as [http://localhost:5050/getAll](http://localhost:5050/getAll). You will only receive JSON data without nice rendering. 
11. Now you can interact with the Frontend [http://localhost/database_javascript/project1/Frontend/index.html](http://localhost/database_javascript/project1/Frontend/index.html).

Finlay, if you need to learn more about nodejs and react: [Learn nodejs by examples](https://github.com/shiyonglu/database_javascript/tree/main/nodejs_examples). [Learn react by examples](https://github.com/shiyonglu/database_javascript/tree/main/react_examples). 

---------------------------------------
Some tips: 
1. In Mac, to see what process runs on port 5000, type ```lsof -i:5000```
3. In Mac, to kill the process on port 5000, type ```kill -9 $(lsof -t -i:5000)```
4. In Windows, to see what process runs on port 5000, type ```netstat -ano | findstr 5000```
5. In Windows, to kill a process id = 40356, type ```taskkill /F /PID 40356```
6. Mac uses port 5000 for AirPlay already, so you need to disable it if you want to use the same port, see [this blog](https://www.reddit.com/r/perl/comments/10p8p39/macos_port_5000_mystery_solved/)
   



