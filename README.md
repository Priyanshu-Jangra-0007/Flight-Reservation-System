✈️ Airport Management System
A full-stack web-based airport management system built using Java (Servlets, JSP, DAO, JDBC) for the backend and HTML, CSS, JavaScript for the frontend. The application supports user authentication, flight bookings, profile management, and admin operations — all connected to a MySQL database using JDBC.

🛠️ Tech Stack
Frontend

HTML5, CSS3, JavaScript
JSP (JavaServer Pages)
Backend

Java Servlets
JDBC with DAO pattern
Apache Maven (for project management)
MySQL (Relational Database)
Build Tool

Maven
📁 Project Structure
AirportManagementSystem/
├── src/
│   └── main/
│       ├── java/
│       │   └── com/
│       │       └── example/
│       │           └── airport/
│       │               ├── dao/
│       │               │   └── FlightDao.java
│       │               ├── model/
│       │               │   ├── Flight.java
│       │               │   └── User.java
│       │               ├── servlets/
│       │               │   ├── FlightServlet.java
│       │               │   └── UserServlet.java
│       │               └── utils/
│       │                   └── DatabaseConnection.java
│       ├── resources/
│       │   └── db.properties
│       └── webapp/
│           ├── WEB-INF/
│           │   └── web.xml
│           ├── static/
│           ├── index.jsp
│           ├── login.jsp
│           ├── register.jsp
│           ├── user-dashboard.jsp
│           ├── user-profile.jsp
│           ├── flight-booking.jsp
│           ├── payment.jsp
│           └── admin-dashboard.jsp
├── pom.xml
└── README.md
🔐 Features
👥 User Module
User Registration & Login
View and Edit Profile
Book Flights
Make Payments
View Booking History
🛫 Admin Module
Admin Login
Add / Delete / View Flights
View All Bookings & Users
Dashboard Summary
📦 Database Configuration
Create a MySQL database and update your db.properties:

db.url=jdbc:mysql://localhost:3306/airport_db
db.username=root
db.password=yourpassword
⚙️ How to Run
Clone the Repository

bash
Copy
Edit
git clone https://github.com/Rishankgupta08/Flight-Reservation-System.git
cd Flight-Reservation-System/AirportManagementSystem
Configure MySQL

Create a new database airport_db

Import tables using your SQL schema (add SQL file to repo if needed)

Update db.properties

Located in src/main/resources/db.properties

Build the Project

mvn clean install

Deploy on Apache Tomcat

Export WAR file from target/ and deploy on your local Tomcat server
