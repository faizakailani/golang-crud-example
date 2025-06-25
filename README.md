# golang-crud-example
A simple RESTful API built with Golang that demonstrates basic CRUD (Create, Read, Update, Delete) operations using native Go features. This project is intended as a learning resource and portfolio piece to showcase backend development skills using Go.

✨ Features
  - Create a new data entry
  - Get all data
  - Get a single data by ID
  - Update data by ID
  - Delete data by ID

🛠 Tech Stack
  - Language: Go (Golang)
  - Framework: Native Go
  - Database: MySQL
  - Tooling: Postman (for testing)

🗃️ Database
This project uses MySQL to store data. You can also modify it to use PostgreSQL or SQLite as needed.

  - 📦 Requirements
    - MySQL server installed (e.g., via XAMPP, MAMP, or native installation)
    - A tool like MySQL Workbench / phpMyAdmin (optional)

  - 🧰 Steps to Setup MySQL:
    - Start MySQL Server (XAMPP)
    - Create the database
      ```
      CREATE DATABASE go_crud_db;
      ```
    - Create the table
      Sample Table Structure
      ```
      CREATE TABLE users (
        id INT AUTO_INCREMENT PRIMARY KEY,
        name VARCHAR(100) NOT NULL,
        email VARCHAR(100) UNIQUE NOT NULL,
        created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
      );
      ```

🚀 Getting Started
Clone the repository:
```
git clone https://github.com/faizakailani/golang-crud-example.git
cd golang-crud-example
```

Run the project:
`go run main.go`

📝 Example Endpoints
GET    /users
GET    /user/{id}
POST   /user
PUT    /user/{id}
DELETE /user/{id}
