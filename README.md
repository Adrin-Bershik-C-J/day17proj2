# 🏨 Hostel Management System - Spring Boot

A **Spring Boot** project demonstrating **filtering**, **sorting**, and **pagination** using a hostel management system example.  
The system manages **Wardens**, **Rooms**, and **Students**, and supports flexible queries through a REST API.

---

## 📂 Project Structure

```
Directory structure:
└── adrin-bershik-c-j-day17proj2/
    ├── mvnw
    ├── mvnw.cmd
    ├── pom.xml
    ├── src/
    │   ├── main/
    │   │   ├── java/
    │   │   │   └── com/
    │   │   │       └── springboot/
    │   │   │           └── day14proj2/
    │   │   │               ├── Day14proj2Application.java
    │   │   │               ├── controller/
    │   │   │               │   └── StudentController.java
    │   │   │               ├── dto/
    │   │   │               │   └── StudentResponseDTO.java
    │   │   │               ├── entity/
    │   │   │               │   ├── Room.java
    │   │   │               │   ├── Student.java
    │   │   │               │   └── Warden.java
    │   │   │               ├── mapper/
    │   │   │               │   └── StudentMapper.java
    │   │   │               ├── repository/
    │   │   │               │   ├── RoomRepository.java
    │   │   │               │   ├── StudentRepository.java
    │   │   │               │   └── WardenRepository.java
    │   │   │               └── service/
    │   │   │                   └── StudentService.java
    │   │   └── resources/
    │   │       └── application.properties
    │   └── test/
    │       └── java/
    │           └── com/
    │               └── springboot/
    │                   └── day14proj2/
    │                       └── Day14proj2ApplicationTests.java
    └── .mvn/
        └── wrapper/
            └── maven-wrapper.properties

```

---

## 🚀 Features

- **Filter Students** by:
  - ID
  - Name
  - Age
  - Room Number
  - Fee Payment Status
- **Sort Students** with pagination support.
- **Entity Relationships**:
  - `Warden` ↔ `Room` (One-to-Many)
  - `Room` ↔ `Student` (One-to-Many)
- **CommandLineRunner** for sample data initialization.
- Uses **MapStruct** for DTO mapping.

---

## 🛠️ Tech Stack

- **Java 17+**
- **Spring Boot 3**
- **Spring Data JPA**
- **PostgreSQL**
- **MapStruct**
- **Lombok**

---

## ⚙️ Setup & Run

### 1️⃣ Clone the repository
```bash
git clone https://github.com/Adrin-Bershik-C-J/day17proj2.git
cd day17proj2
```
### Configure Database
- spring.datasource.url=jdbc:postgresql://localhost:5432/day14proj2
- spring.datasource.username=postgres
- spring.datasource.password=YOUR_PASSWORD
