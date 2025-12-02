🏥 Hospital Management System – Java & MySQL
A desktop-based Hospital Management System built using Java (Swing + AWT) and MySQL, featuring complete CRUD operations, room management, patient management, and user login authentication.

🚀 Features
🔐 Authentication System
Login screen with username & password
Secure validation using MySQL
Java Swing GUI
Error alerts for incorrect login
🧑‍⚕️ Patient Management
Add new patient
Update patient details
Discharge patient
View all patient records
🏨 Room Management
Check room availability
Room pricing details
Search room information
Live room status from database
🚑 Ambulance Management
Track ambulance details
Availability checking

Display ambulance list using DbUtils table model
🏬 Department Management
Add / view hospital departments
SQL-powered dynamic table display
📊 Database Integration
MySQL database connectivity
JDBC + MySQL Connector/J
SQL-powered forms and tables
Clean separation of src/, bin/, lib/, and icon/ folders

📁 Project Folder Structure
<img width="491" height="533" alt="Screenshot 2025-12-03 at 1 00 13 AM" src="https://github.com/user-attachments/assets/9adaabe1-f97c-4f44-9b99-99fad95d5a62" />



🛠️ Technologies Used
Component	Technology
Frontend	Java Swing, AWT
Backend	Java
Database	MySQL
Integration	JDBC
IDE	VS Code / IntelliJ / Eclipse
OS	macOS / Windows / Linux


🗄️ Database Setup (MySQL)
Run these SQL commands before starting the app:

create database hospital_management_system;
use hospital_management_system;
create table patient_info
(
ID varchar(20),
Number varchar(40),
Name varchar(20),
Gender varchar(20),
Patient_Disease varchar(20),
Room_Number varchar(20),
Time varchar(100),
Deposite varchar(20)
);
select * from login
select * from patient_info;

create table Room
(
room_no varchar(20),
Availability varchar(20),
Price varchar(20),
Room_type varchar(100)
);
select * from Room;

insert into Room values("100","Availabil","500","G Bed 1");
insert into Room values("101","Availabil","500","G Bed 2");
insert into Room values("102","Availabil","500","G Bed 3");
insert into Room values("103","Availabil","500","G Bed 4");
insert into Room values("200","Availabil","1500","Private Room");
insert into Room values("201","Availabil","1500","Private Room");
insert into Room values("202","Availabil","1500","Private Room");
insert into Room values("203","Availabil","1500","Private Room");
insert into Room values("300","Availabil","3500","ICU Bed 1");
insert into Room values("301","Availabil","3500","ICU Bed 2");
insert into Room values("302","Availabil","3500","ICU Bed 3");
insert into Room values("303","Availabil","3500","ICU Bed 4");
insert into Room values("304","Availabil","3500","ICU Bed 5");
insert into Room values("305","Availabil","3500","ICU Bed 6");

create table department(Department varchar(100),Phone_no varchar(20));
select * from department; 

insert into department values("Surgical department","123456789");
insert into department values("Nursing department","123456789");
insert into department values("operation Theater complex (OT)","123456789");
insert into department values("paramedical department","123456789");

create table EMP_INFO(Name varchar(20),Age varchar(20),Phone_Number varchar(20),salary varchar(20),Gmail varchar(40),Aadhar_Number varchar(20));
select * from EMP_INFO;
insert into EMP_INFO values("Doctors1","30","123456789","50000","gr@gmail.com","123456789101");
insert into EMP_INFO values("Doctors2","30","123456789","50000","gr@gmail.com","123456789101");

-- Fix 'Occupaid' typo
UPDATE Room SET Availability = 'Occupied' WHERE Availability = 'Occupaid';

-- Fix 'Availabl' typo
UPDATE Room SET Availability = 'Available' WHERE Availability = 'Availabil';
SET SQL_SAFE_UPDATES = 0;
SET SQL_SAFE_UPDATES = 1;

create table Ambulance(Name varchar(20),Gender varchar(20),Car_name varchar(20),Available varchar(20),Location varchar(20));
drop table Ambulance;
insert into Ambulance values("av","Male","ZEN","Available","area 16");
select * from Ambulance;

▶️ How to Run the Project
1️⃣ Compile all Java files
javac -cp "lib/*" -d bin src/Hospital/management/system/*.java
2️⃣ Run the application
java -cp "bin:lib/*" Hospital.management.system.Login

👨‍💻 Author
Lakshya Karamchandani
B.Tech CSE
Agra, India



