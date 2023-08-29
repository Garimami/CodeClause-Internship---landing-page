# CodeClause-Internship---landing-page
Simple Gym landing page
In this project i created a simple landing page of gym .

language used
Php, javascript, html,css.

code editor:- visual studio code.

server side :- Xampp.

Installation
1.Open XAMPP Control Panel

2.Next to the Apache module click Start

3.Next to the MySQL module click Start

4.Navigate to XAMPPs installation folder (C:\xampp) Open the htdocs folder

Edit the file zip resgitration.php file in the includes folder and update the configuration information (like your email address, Database login etc). The script will create the table in the database when you submit the registration form the first time.
6.Upload the entire 'source' folder to your in your editor/or your website.

7.You can customize the forms and scripts as required.

Documentation
index.php
This script displays the registration form. When the user submits the form, it show the succuesful registration.

2.connection.php

-> after index.php we have to create our MySQL server Database and a Table according to our requirements. We connect our MySQL server Database using PHP mysqli_connect() function which takes four arguments, i.e. our “servername”, “username”, “password” and “database”. for checking the databse you can go for CREATE TABLE IF NOT EXISTS Fitness plus ( id int(11) NOT NULL AUTO_INCREMENT, username varchar(50) NOT NULL, password varchar(255) NOT NULL, email varchar(100) NOT NULL, PRIMARY KEY (id) ) ENGINE=InnoDB AUTO_INCREMENT=2 DEFAULT CHARSET=utf8;

JS.PHP
Running code in response to certain events occurring on a web page. We used a click event in our example above to detect when the label is clicked and then run the code that updates the text label.

Style.php
using style.php we can give a creative look to our website and web designing.

5.signup.php

This PHP code is a server-side script that handles user registration for a website or web application.

include('connection.php');: This line includes the connection.php file, which likely contains the code to establish a connection to the MySQL database. This is necessary for the script to interact with the database.

if (isset($_POST['submit'])) {: This condition checks if the form has been submitted. It assumes that the form has an input element with the name attribute set to "submit," and when the user submits the form, this condition will be true, and the code inside the block will be executed.

mysqli_real_escape_string(): This function is used to escape special characters in a string to prevent SQL injection attacks. It is used to sanitize the user input received from the registration form before using it in SQL queries.

$username, $email, $password, $cpassword: These variables store the values entered by the user through the registration form. They are obtained using the $_POST superglobal array, assuming the form elements have the appropriate name attributes.

Duplicate Username and Email Check: The script checks if the entered username and email already exist in the database. It does this by querying the database and counting the number of rows returned with matching usernames and emails. If either the username or the email is already in use, the registration process is stopped, and an appropriate alert message is displayed.

Password Matching Check: The script checks if the entered password and confirmed password match. If they match, the script proceeds to hash the password using password_hash() function before inserting the user's data into the database.

password_hash(): This function securely hashes the password before storing it in the database. Password hashing is crucial for security, as it prevents storing plaintext passwords, making it harder for attackers to retrieve the original password.

Database Insertion: After all checks are passed, the script constructs an SQL query to insert the user's data (username, email, and hashed password) into the signup1 table in the database.

header("Location: welcome.php");: If the registration is successful, the script redirects the user to the welcome.php page.

Alert Messages: If there is an issue with the registration (e.g., duplicate username or email, password mismatch), the script shows alert messages using JavaScript and redirects the user back to the index.php page (presumably where the registration form is located).

Authors
@octokatherine
Color Reference
Color	Hex
Example Color	#0a192f#0a192f
Example Color	#f8f8f8#f8f8f8
Example Color	#00b48a#00b48a
Example Color	#00d1a0#00d1a0
🔗 Links
github link:- https://github.com/Garimami/CodeClause-Internship---landing-page
