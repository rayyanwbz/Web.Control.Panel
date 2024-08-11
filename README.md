# Web.Control.Panel
This project introduces an intuitive web interface for controlling robot movement. Users can easily command the robot to move forward, backward, left, or right, as well as bring it to a stop. For convenient tracking and analysis, all commands are automatically logged with timestamps in a secure database.

Features
Control Interface:
Forward: Moves the robot forward. Backward: Moves the robot backward. Left: Turns the robot left. Right: Turns the robot right. Stop: Stops the robot immediately.
![WhatsApp Image 2024-08-11 at 18 37 59](https://github.com/user-attachments/assets/41b287eb-680b-46f3-8863-cab3ea5def21)

Database Integration:
Each command is recorded in a MySQL database with a timestamp. The database allows tracking of the command history for analysis. Screenshots Control Panel

Database

Usage

Setting Up:
Ensure you have a web server running Deploy the HTML and PHP files to your web server.

Database Configuration:
Set up a MySQL database.

Use the following SQL schema to create the commands table:
sql
CREATE TABLE commands ( id int(11) NOT NULL AUTO_INCREMENT, direction varchar(50) NOT NULL, timestamp datetime NOT NULL, PRIMARY KEY (id) ) ENGINE=InnoDB DEFAULT CHARSET=utf8;

Running the Control Panel:
Navigate to the web page in your browser. Use the directional buttons to control the robot. The commands will be logged in the database. Technology Stack Frontend: HTML, CSS Backend: PHP Database: MySQL
![WhatsApp Image 2024-08-11 at 18 40 05](https://github.com/user-attachments/assets/7045839d-6b71-44de-ab0a-730f62c23a1b)
