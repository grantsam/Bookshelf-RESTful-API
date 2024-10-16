# Bookshelf RESTful API

This project is a Bookshelf RESTful API built using Node.js and Hapi.js, designed to manage book data with full CRUD operations. The API allows users to create, read, update, and delete books, with additional features like filtering and searching based on book attributes.

## Features

- **Add a new book** to the bookshelf.
- **Retrieve a list of books** with optional query parameters:
  - `name`: Search for books by title (case-insensitive).
  - `reading`: Filter books by their reading status (reading or not).
  - `finished`: Filter books by completion status.
- **Retrieve detailed information** about a specific book.
- **Update the details** of an existing book.
- **Delete a book** from the bookshelf.

## Tech Stack

- Node.js
- Hapi.js framework
- Nanoid for generating unique book IDs

## Installation

Follow these steps to set up and run the Bookshelf RESTful API locally on your machine.

### Prerequisites

- [Node.js](https://nodejs.org/) (version 12.x or higher)
- [npm](https://www.npmjs.com/get-npm) (usually comes with Node.js)

### Steps

**Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/bookshelf-RESTful-API.git
   cd bookshelf-RESTful-API
   npm install
```
The server should now be running on http://localhost:5000.

## Usage

Use tools like Postman or cURL to interact with the API.

**Example of adding a book:**
  ```bash
  curl -X POST http://localhost:5000/books \
  -H "Content-Type: application/json" \
  -d '{
        "name": "The Great Gatsby",
              "year": 1925,
              "author": "F. Scott Fitzgerald",
              "summary": "A story about the Jazz Age in the United States.",
              "publisher": "Scribner",
              "pageCount": 180,
              "readPage": 180,
              "reading": true
      }'
```
**Example of retrieving all books:**
```bash
curl -X GET http://localhost:5000/books




