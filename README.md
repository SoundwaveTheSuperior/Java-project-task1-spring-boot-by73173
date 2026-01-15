# Task 1 – Java Spring Boot Application

## 📌 Project Overview
This project is **Task 1** of the assignment and demonstrates a **basic Java Spring Boot web application**.  
The application includes:
- A REST endpoint
- A dynamic HTML page rendered with **Thymeleaf**
- Static resources (images)
- Basic request handling using HTTP GET methods

The goal of this task is to show understanding of how Spring Boot works, how requests are handled, and how responses are returned to the browser.

-----------------------------------------------------------------------------------------------------------------------------

## 🛠 Technologies Used
- **Java 17**
- **Spring Boot 3**
  - Spring Web
  - Thymeleaf
- **Apache Maven**
- **HTML**
- **Git & GitHub**

-----------------------------------------------------------------------------------------------------------------------------
## 🚀 How the Application Works

### 1️⃣ Application Entry Point
The application starts from the main class:FirstProjectJavaSpring73173Application.java



This class is annotated with `@SpringBootApplication`, which:
- Enables auto-configuration
- Scans components
- Starts the embedded Tomcat server

-----------------------------------------------------------------------------------------------------------------------------

### 2️⃣ Controller Logic
The controller class:MyController.java


Responsibilities:
- Handles incoming HTTP GET requests
- Returns either:
  - A plain text response (REST)
  - A rendered HTML page (Thymeleaf)

-----------------------------------------------------------------------------------------------------------------------------

## 🌐 Available Endpoints & Use Cases

### 🔹 1. Root Endpoint (REST)
- **URL:**http://localhost:8080/

- **HTTP Method:** `GET`
- **Description:**  
Returns a simple text response to confirm the application is running.

-----------------------------------------------------------------------------------------------------------------------------

### 🔹 2. Greeting Page (HTML – Default)
- **URL:**http://localhost:8080/greeting

- **HTTP Method:** `GET`
- **Description:**  
Displays a dynamic HTML page rendered using Thymeleaf with a default greeting message.

-----------------------------------------------------------------------------------------------------------------------------

### 🔹 3. Greeting Page with Parameter (Dynamic)
- **URL Example:**http://localhost:8080/greeting?name=Omar

- **HTTP Method:** `GET`
- **Description:**  
Uses a query parameter (`name`) to personalize the greeting message dynamically.

This demonstrates:
- Request parameter handling
- Dynamic content rendering
- Server-side HTML generation

-----------------------------------------------------------------------------------------------------------------------------

## 🖼 Static Resources
The project includes static resources located in:src/main/resources/static/images


Example:
- `Megatron.jpg`  
This image is served directly by Spring Boot and used in the HTML page.

-----------------------------------------------------------------------------------------------------------------------------

## 📂 Project Structure
src
└── main
├── java
│   └── pl.edu.vistula.first_project_java_spring
│       ├── FirstProjectJavaSpring73173Application.java
│       └── controller
│           └── MyController.java
└── resources
├── static
│   └── images
│       └── Megatron.jpg
├── templates
│   └── greeting.html
└── application.properties




-----------------------------------------------------------------------------------------------------------------------------

## ▶️ How to Run the Application

### Prerequisites
- Java 17 or higher
- Maven (or Maven Wrapper)

### Run on Windows
bash
mvnw.cmd spring-boot:run
-----------------------------------------------------------------------------------------------------------------------------
Run on Linux / macOS
./mvnw spring-boot:run




The application will start at:
http://localhost:8080



