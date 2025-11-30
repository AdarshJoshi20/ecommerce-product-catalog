## E-Commerce Product Catalog (Full-Stack Spring Boot & React)

## Overview

This project is a **full-stack e-commerce product catalog** designed to efficiently display and manage product information. It serves as a robust foundation for an online store, featuring a scalable RESTful API backend built with **Spring Boot** and a dynamic, interactive frontend built with **React**.

##  Key Features Implemented

The application successfully implements the following core functionalities:

1.  **Full-Stack Data Flow:** Seamless integration between the React client and the Spring Boot API, ensuring real-time data retrieval.
2.  **Robust Data Persistence:** Utilizes **Spring Data JPA** and **Hibernate** for mapping and managing `Product` and `Category` entities in a relational **MySQL** database.
3.  **Real-Time Search Functionality:** Allows users to instantly search the product catalog by keyword across product names.
4.  **Dynamic Filtering and Sorting:** Enables users to filter products by category and sort the displayed list by price (low-to-high or high-to-low).
5.  **CORS Handling:** Properly configured the backend to manage Cross-Origin Resource Sharing (CORS), allowing the independent frontend and backend services to communicate securely.
6.  **Data Seeding:** Implemented a `CommandLineRunner` to automatically populate the database with initial dummy data upon application startup, ensuring a working demo environment.

##  Technology Stack

Backend API: Spring Boot 3 (Java) for building scalable RESTful services.
Frontend UI: React framework bundled with Vite for a fast, component-based user interface.
Database: MySQL used for data storage, managed via Spring Data JPA and Hibernate.
Styling: Bootstrap CSS for responsive design and professional styling.
Build Tools: Maven (Backend dependency management) and Node.js/npm (Frontend environment).

##  Getting Started (How to Run Locally)

### Prerequisites

You need the following installed on your system:

   **Java Development Kit (JDK 17+)**
   **Node.js (LTS version) & npm**
   **MySQL Server**

### 1\. Clone the Repository

```bash
git clone [YOUR_REPO_LINK]
cd [REPO_FOLDER_NAME]
```

### 2\. Backend Setup (Spring Boot API)

1.  Navigate to the backend folder (e.g., `cd backend`).
2.  **Configure Database:** Open the `src/main/resources/application.properties` file and update the following settings to match your local MySQL configuration:
    ```properties
    spring.datasource.url=jdbc:mysql://localhost:3306/ecommerce_db
    spring.datasource.username=YOUR_USERNAME
    spring.datasource.password=YOUR_PASSWORD
    spring.jpa.hibernate.ddl-auto=update
    ```
3.  **Run Application:** Use your IDE (IntelliJ) or the command line to start the Spring Boot application:
    ```bash
    mvn clean install
    mvn spring-boot:run
    ```
    The API should start running on `http://localhost:8080`.

### 3\. Frontend Setup (React Client)

1.  Navigate to the frontend folder (e.g., `cd frontend`).
2.  **Install Dependencies:**
    ```bash
    npm install
    ```
3.  **Start Development Server:**
    ```bash
    npm run dev
    ```
    The application will open in your browser, usually at `http://localhost:5173` or `http://localhost:3000`.
