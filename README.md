
# 🧑‍💼 Employee CRUD Application

A simple Spring Boot application for managing employee records using a RESTful API and MongoDB as the backend database.

---

## 🚀 Features

- Add new employees (POST)
- Get all employees (GET)
- Get employee by ID (GET)
- Update employee details (PUT)
- Delete employee (DELETE)
- MongoDB integration
- Simple and clean API structure

---

## 🛠️ Tech Stack

- Java 17+
- Spring Boot
- Spring Data MongoDB
- MongoDB
- Maven
- Postman (for API testing)

---

## 📂 Project Structure

```
employee-crud-app/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/example/demo/
│   │   │       ├── controller/
│   │   │       ├── model/
│   │   │       └── repository/
│   │   └── resources/
│   │       └── application.properties
├── pom.xml
└── README.md
```

---

## 📝 API Endpoints

| Method | Endpoint               | Description              |
|--------|------------------------|--------------------------|
| GET    | `/api/employees`       | Get all employees        |
| GET    | `/api/employees/{id}`  | Get employee by ID       |
| POST   | `/api/employees`       | Add new employee         |
| PUT    | `/api/employees/{id}`  | Update existing employee |
| DELETE | `/api/employees/{id}`  | Delete employee          |
| GET    | `/api/employees/ping`  | Check API status         |

---

## ⚙️ Setup Instructions

### 📥 1. Clone the repository
```bash
git clone https://github.com/yourusername/employee-crud-app.git
cd employee-crud-app
```

### 📦 2. Configure MongoDB
Make sure MongoDB is running locally or provide connection details in `application.properties`:

```properties
spring.data.mongodb.uri=mongodb://localhost:27017/employeedb
spring.data.mongodb.database=employeedb
```

### ▶️ 3. Run the app
```bash
docker run -d -p 27017:27017 --name mongo-db mongo
mvn spring-boot:run
```

---

## 📬 Example Request

### Add Employee (POST)
```http
POST /api/employees
Content-Type: application/json

{
  "name": "John Doe",
  "department": "Engineering",
  "salary": 75000
}
```

---

## 🙌 Contributing

Feel free to fork the repo and send pull requests to add new features or fix issues!

---

## 🪪 License

This project is licensed under the MIT License.

---

## 📞 Contact

For help or suggestions: [your-email@example.com]
