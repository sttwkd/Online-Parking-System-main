# Online-Parking-System-main
# Online Parking System

## Overview
The **Online Parking System** is a web-based application designed to provide users with a convenient platform to search, book, and manage parking spaces online. Built using modern web technologies, this system streamlines parking space management and enhances user experience.

## Features
- **User Registration and Login**: Secure authentication for users.
- **Parking Space Booking**: Real-time availability and booking of parking slots.
- **Admin Dashboard**: Manage parking spaces, bookings, and user data.
- **Responsive Design**: Accessible on various devices, including desktops, tablets, and smartphones.

## Technologies Used
- **Backend**: Spring Boot (Java)
- **Frontend**: HTML, CSS, JavaScript
- **Database**: MySQL
- **Tools**: Maven (for dependency management), IntelliJ IDEA/VS Code (IDE)

## System Architecture
1. **Frontend**: Provides an interactive and user-friendly interface.
2. **Backend**: Handles business logic, API endpoints, and data processing.
3. **Database**: Stores user information, parking data, and booking details.

## Installation and Setup
### Prerequisites
- JDK 11 or higher
- MySQL Server
- Maven

### Steps to Run the Project
1. **Clone the Repository**
   ```
   git clone https://github.com/yourusername/Online-Parking-System-main.git
   cd Online-Parking-System-main
   ```

2. **Set Up the Database**
   - Create a MySQL database named `online_parking_system`.
   - Import the provided SQL file (`database.sql`) to set up tables and initial data.

3. **Configure Database Properties**
   - Update `application.properties` (located in `src/main/resources`) with your MySQL credentials:
     ```
     spring.datasource.url=jdbc:mysql://localhost:3306/online_parking_system
     spring.datasource.username=your_username
     spring.datasource.password=your_password
     spring.jpa.hibernate.ddl-auto=update
     ```

4. **Build and Run the Application**
   ```
   mvn clean install
   mvn spring-boot:run
   ```

5. **Access the Application**
   - Open your browser and navigate to `http://localhost:8080`.

## Folder Structure
```
Online-Parking-System-main/
├── src/
│   ├── main/
│   │   ├── java/       # Backend logic (Spring Boot controllers, services, and models)
│   │   ├── resources/  # Configuration files and static resources
│   │   └── webapp/     # HTML, CSS, and JS files
├── pom.xml             # Maven configuration file
└── README.md           # Project documentation
```

## Usage
1. **User Login**: Users can log in or register to access the system.
2. **Booking a Slot**: Select a parking slot, choose a time, and confirm the booking.
3. **Admin Access**: Admins can manage parking spaces and view all bookings.

## Future Enhancements
- Integration with payment gateways.
- Real-time notifications for booking status.
- Mobile application for on-the-go access.

## Contributors
- [Your Name] - Developer

## License
This project is licensed under the MIT License. See the LICENSE file for details.

---
**Note**: Replace placeholders like `your_username` and `your_password` with actual values before deployment.

