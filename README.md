# Student Management REST API

Lab Assignment 2 — Web Dev III (Node.js & Express Backend)

## Requirements Covered

- Express.js server setup
- REST API design
- Student CRUD operations
- Custom logger middleware
- Modular routing
- Error handling and HTTP status codes
- In-memory Array/JSON data
- Postman testing

## Restrictions

This project intentionally does **not** use:
- MongoDB
- MySQL
- Mongoose

Student records are stored in `data/students.js`.

## Project Structure

```text
student-management-rest-api/
├── app.js
├── package.json
├── README.md
├── middleware/
│   └── logger.js
├── routes/
│   └── studentRoutes.js
└── data/
    └── students.js
```

## Setup

Make sure Node.js is installed.

```bash
npm install
npm start
```

The server runs at:

```text
http://localhost:3000
```

## API Endpoints

| Method | Endpoint | Purpose |
|---|---|---|
| GET | `/students` | Get all students |
| GET | `/students/:id` | Get one student |
| POST | `/students` | Add a student |
| PUT | `/students/:id` | Update a student |
| DELETE | `/students/:id` | Delete a student |

## POST Example

URL:

```text
POST http://localhost:3000/students
```

JSON body:

```json
{
  "name": "Neha",
  "course": "BTech"
}
```

## PUT Example

URL:

```text
PUT http://localhost:3000/students/1
```

JSON body:

```json
{
  "name": "Rahul Sharma",
  "course": "BTech"
}
```

## Status Codes

- `200` — Success
- `201` — Created
- `400` — Bad Request
- `404` — Not Found
- `500` — Internal Server Error


