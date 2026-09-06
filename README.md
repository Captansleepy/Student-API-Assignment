# Student API in Express

CSC220 Web Development II - Continued Guided Lab: Middleware & a Rendered Page.

This project continues the previous Student API in Express assignment by adding middleware, JSON body parsing, a POST route, a 404 handler, and EJS rendering.

## Install

```powershell
npm install
```

## Run

```powershell
npm run dev
```

## Required tests

- `http://localhost:3000`
- `http://localhost:3000/api/students`
- `http://localhost:3000/api/students/2`
- `http://localhost:3000/students`
- `http://localhost:3000/wrong-url`

The terminal should also show logger output with the HTTP method, requested URL, and time.

## POST test

Send a POST request to:

```text
http://localhost:3000/api/students
```

with JSON such as:

```json
{
  "id": 6,
  "name": "May",
  "major": "IT"
}
```

Expected status: `201 Created`.

## Project structure

```text
Student-API-Assignment/
├── views/
│   └── students.ejs
├── .gitignore
├── app.js
├── package.json
├── package-lock.json
├── README.md
└── students.json
```

`node_modules/` and `.env` are excluded by `.gitignore`.
