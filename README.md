# 👨‍💼 Employee Attendance Tracker

A Spring Boot-based REST API for managing employee attendance data. This system allows employees to check in and check out while storing their records efficiently using a PostgreSQL database.

---

## 🛠️ Features

- Add new employee attendance records
- Update check-in and check-out times
- View all attendance records
- Integration with PostgreSQL
- Uses Spring Boot, Spring Data JPA, and RESTful APIs

---

## 🚀 Technologies Used

- Java 17
- Spring Boot 3
- Spring Web
- Spring Data JPA
- PostgreSQL
- Lombok
- Maven

---

## 🗂️ Project Structure

```
employee-attendance-tracker/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/attendance/
│   │   │       ├── controller/
│   │   │       ├── entity/
│   │   │       ├── repository/
│   │   │       └── EmployeeAttendanceTrackerApplication.java
│   │   └── resources/
│   │       └── application.properties
├── pom.xml
└── README.md
```

---

## ⚙️ Setup Instructions

### ✅ Prerequisites
- Java 17+
- Maven
- PostgreSQL
- IDE (e.g., IntelliJ or Eclipse)
- Git

### 🔧 Configuration

1. Create a PostgreSQL database (e.g., `attendance_db`)
2. Update `application.properties` with your DB credentials:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/attendance_db
spring.datasource.username=your_username
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
```

### ▶️ Run the Project

```bash
# Compile and run
mvn spring-boot:run
```

API will be available at: `http://localhost:8080/attendance`

---

## 📫 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| `POST` | `/attendance` | Add attendance |
| `GET` | `/attendance` | Get all records |
| `PUT` | `/attendance/{id}` | Update check-out time |

---

## 🙌 Contributors

- 👩‍💻 Divya Adabala

---

## 📜 License

This project is licensed under the MIT License - feel free to use, modify, and distribute.

---
