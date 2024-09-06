# Book Management System

This project is a Spring Boot REST API for managing books. It provides endpoints to add, update, retrieve, and delete books.

## Features

- Retrieve all books (`GET /api/books`)
- Retrieve a book by its ID (`GET /api/books/{id}`)
- Add a new book (`POST /api/books`)
- Update an existing book (`PUT /api/books/{id}`)
- Delete a book (`DELETE /api/books/{id}`)

## Setup Instructions

1. Clone or download the project.
2. Open the project in your preferred IDE (e.g., IntelliJ or Eclipse).
3. Run the application using `mvn spring-boot:run` or run the `main` method in `DemoApplication.java`.
4. The application will run at `http://localhost:8080/`.

## Testing Instructions

Please use **Postman** or a similar tool to test the API endpoints:

- **GET** `/api/books` - Retrieve all books.
- **GET** `/api/books/{id}` - Retrieve a specific book by its ID.
- **POST** `/api/books` - Add a new book. Include the book details in the request body as JSON.
- **PUT** `/api/books/{id}` - Update an existing book. Include updated details in the request body.
- **DELETE** `/api/books/{id}` - Delete a book by its ID.

### Example for Adding a New Book in Postman:
1. Use the `POST` method.
2. Set the URL to `http://localhost:8080/api/books`.
3. In the **Body** tab, select `raw` and `JSON`, then provide the book details:
   ```json
   {
       "title": "1984",
       "author": "George Orwell",
       "publicationYear": 1949
   }
