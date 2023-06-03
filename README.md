#### VISHWESHVARAN M - 20EUIT167

# COVID VACCINATION BOOKING - CONSOLE APPLICATION DOCUMENTATION

## DESCRIPTION:
  The Covid Vaccination Booking application is a console application made using Java (JDBC) and MySql. Eclipse IDE is used to create this application. It provides functionalities to book a slot for vaccination, view the bookings made by the user etc. 
  •	This application automatically creates a database named "covidvaccinationbooking" in the local host having a default port number 3306 and uses that database.
  
  •	The program also creates 3 tables in that database named Vaccine details, User, and User Bookings.
  
  •	The default admin username is "admin" and password is "admin" - case sensitive.

The console application has two users:

#### Type of Users:

  •	Admin

  •	Users


## ADMIN USE CASES:
•	Login

•	Add Vaccination Center

•	Remove Vaccination Center

•	Get Dosage Details

•	Logout

## USER USE CASES:
•	User Sign-up

•	User Login

•	Get vaccination center details (Center name and working hours)

•	Apply for a vaccination slot

•	View user bookings

•	Logout


## HOW TO RUN THIS APPLICATION?
•	Install Java and MySql

•	Install a Java IDE (Eclipse, NetBeans etc)

•	Install mysql-connector-java.jar file to connect Java with MySql

•	Create a Java project with a class named “covidVaccinationBooking”.

•	Add mysql-connector-java.jar as referenced library to the Java project

•	Copy this code to the main file

•	Run java code


## ADMIN USE CASES:

•	The admin must first login using default username and password (username and password are case sensitive).

•	Then it will show a list of actions that an admin can do.

_1)	Add Vaccination Center_
  - The admin can add new vaccination centers by providing the center name, starting and ending time of the center (working hours), dosage details includes the                  name of the vaccine present in the center, and the number of slots available as inputs. The details are stores in the “vaccine details” table.

_2)	Remove Vaccination Center_
  - The admin can remove the existing vaccination center by providing the center name as input. The details of the center are removed from the “vaccine details” table.
 
_3)	Get Dosage Details_
  - The admin can get the dosage details, i.e., the names of the vaccine available in the center. The required output is displayed from the “vaccine details” table.


## USER USE CASES:

### USER SIGN-UP:
  • The user can sign-up by providing the username and the password as input. It is stored in the user table. And the user is requested to login.

### USER LOGIN:
•	The user can login by using their username and password. If the username is present in the user table, then the password is validated and the user is logged in.

•	Then it will show a list of actions that a user can do.

_1)	Get vaccination center details (Center name and working hours)_
  - The user can get the working hours of the vaccination center by providing the center’s name as input. The output is fetched from the vaccine details table.

_2)	Apply for a vaccination slot:_
  - The user can apply for a slot in the available centers by selecting the required center and the vaccine name. The slot is booked and the username and details is inserted in the userbookings table, if the slot is available.
 
_3)	View user bookings_:
  - The user can view their vaccination slot booking made by them. The data is fetched from the userbookings table and displayed.
