# Bus Reservation System

A Java-based Bus Reservation System developed using Spring Boot, Spring Data JPA, Hibernate, and MySQL. The project provides a structured backend for managing bus information, searching available buses, and handling reservation-related operations.

## Technologies Used

- **Programming Language:** Java
- **Framework:** Spring Boot
- **ORM:** Spring Data JPA, Hibernate
- **Database:** MySQL
- **Build Tool:** Maven
- **Server:** Embedded Apache Tomcat

## Project Architecture

The application follows a layered architecture:

1. **Controller Layer:** Handles incoming HTTP requests and manages application endpoints.
2. **Service Layer:** Contains business logic for reservation management and related operations.
3. **Repository Layer:** Manages database operations using Spring Data JPA.
4. **Model Layer:** Defines the entities and their relationships.

## Key Features

- Bus management and reservation operations.
- Search for available buses.
- MySQL database integration.
- Data persistence using Spring Data JPA and Hibernate.
- Layered application architecture.

## Project Structure

```text
Bus-Reservation-System/
├── src/
│   └── main/
│       ├── java/
│       └── resources/
├── .mvn/
├── mvnw
├── mvnw.cmd
├── pom.xml
├── .gitignore
└── README.md
```

## Prerequisites

- Java JDK 17
- MySQL Server
- Maven (or the included Maven Wrapper)
- IDE such as Eclipse, STS, or IntelliJ IDEA

## Database Configuration

1. Create a MySQL database named `narasimha`.
2. Open `src/main/resources/application.properties`.
3. Configure your database connection:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/narasimha
spring.datasource.username=${DB_USERNAME:root}
spring.datasource.password=${DB_PASSWORD:}
```

Set the `DB_PASSWORD` environment variable to your local MySQL password before running the application.

## How to Run

1. Clone the repository:

```bash
git clone https://github.com/narasimha8088/Bus-Reservation-System.git
```

2. Navigate to the project directory:

```bash
cd Bus-Reservation-System
```

3. Run the application on Windows:

```powershell
.\mvnw.cmd spring-boot:run
```

4. Open the application in your browser:

http://localhost:8081

## Future Improvements

- Add user authentication and authorization.
- Improve bus search and filtering.
- Enhance reservation management.
- Add payment integration.

## Acknowledgement

This project is based on an existing Bus Reservation System codebase. Credit goes to the original repository: [aihikcse/Bus-Reservation-System](https://github.com/aihikcse/Bus-Reservation-System).

Further modifications and improvements should be documented as the project evolves.