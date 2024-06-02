# Library Management System

A simple CRUD application for managing a library. This project demonstrates the use of Spring Boot, Spring Data JPA, and H2 Database for building a backend system.

## Features

-   Add, update, delete, and view books.
-   Simple REST API for book management.
-   In-memory H2 database for data storage.

## Technologies Used

-   Java 22
-   Spring Boot
-   Spring Data JPA
-   H2 Database
-   Lombok

## Getting Started

### Prerequisites

-   JDK 22 or higher
-   Maven

### Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/library.git
    ```
2. Navigate to the project directory:
    ```sh
    cd library
    ```
3. Build the project:
    ```sh
    mvn clean install
    ```
4. Run the application:
    ```sh
    mvn spring-boot:run
    ```

### Using the API

The application runs on `http://localhost:8080`.

#### Endpoints

-   `GET /api/books` - Retrieve all books
-   `GET /api/books/{id}` - Retrieve a book by ID
-   `POST /api/books` - Add a new book
-   `PUT /api/books/{id}` - Update an existing book
-   `DELETE /api/books/{id}` - Delete a book

### Example JSON for Adding/Updating a Book

```json
{
    "title": "Example Book",
    "author": "Author Name",
    "publicationYear": 2021
}
```

### H2 Console

The H2 database console is available at `http://localhost:8080/h2-console`.

-   JDBC URL: `jdbc:h2:mem:testdb`
-   Username: `sa`
-   Password: (leave blank)

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
