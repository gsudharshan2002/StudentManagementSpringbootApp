# 🧑‍🎓 Student Management System - Spring Boot

A simple RESTful API built using **Spring Boot** to perform **CRUD operations** on student data. The API can be tested using **Postman** and uses **MySQL** as the database.

---

## 📦 Tech Stack

- Java
- Spring Boot
- MySQL
- Spring Data JPA
- Postman (for API testing)

---

## 🚀 How to Run

### 1. Clone the project
```bash
git clone https://github.com/your-username/student-management.git cd student-management

```
--
### 2. Configure application.properties

Make sure your file is located at:
src/main/resources/application.properties
```bash
spring.datasource.url=jdbc:mysql://localhost:3306/your_database_name
spring.datasource.username=your_db_username
spring.datasource.password=your_db_password

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

### 3.Run the project

Use Spring Tool Suite (STS) or run from the terminal:
```bash
./mvnw spring-boot:run
```
## 📡 API Endpoints

| Method | Endpoint                   | Description            |
|--------|----------------------------|------------------------|
| GET    | `/students`                | Get all students       |
| POST   | `/student/add`             | Add a new student      |
| GET    | `/students/{id}`           | Get student by ID      |
| PUT    | `/students/update/{id}`    | Update student by ID   |
| DELETE | `/students/delete/{id}`    | Delete student by ID   |



### 🔁 Example Request Body for POST/PUT
```json
{
  "name": "John Doe",
  "email": "john@example.com"
}
```

## 📬 Testing with Postman

#### 1.Start the Spring Boot application.

#### 2.Open Postman.

#### 3.Use the listed endpoints to test the following:

>- GET all students

>- POST a new student

>- GET a student by ID

>- PUT to update a student

>- DELETE a student by ID


## ✅ Features
 - Add new student

- View all students

- Get student by ID

- Update student details

- Delete student record

## Project structure


        student-management/
        ├── src/
        │   ├── main/
        │   │   ├── java/com/example/studentmanagement/
        │   │   │   ├── controller/
        │   │   │   ├── model/
        │   │   │   ├── repository/
        │   │   │   ├── service/
        │   │   │   └── StudentManagementApplication.java
        │   │   └── resources/
        │   │       └── application.properties
        ├── README.md
        ├── pom.xml






