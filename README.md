# Student API in Express

CSC220 Web Development II - Guided Lab: Student API in Express.

## Install

```powershell
npm install
```

This installs Express and nodemon and refreshes `package-lock.json` with the complete dependency tree.

## Run

Development mode:

```powershell
npm run dev
```

Or normal mode:

```powershell
npm start
```

## Required browser tests

1. `http://localhost:3000`
2. `http://localhost:3000/api/students`
3. `http://localhost:3000/api/students/2`
4. `http://localhost:3000/api/students/99`
5. `http://localhost:3000/api/students?major=IT`

## Expected results

- Home page: welcome page and available routes.
- All students: all 5 students as JSON.
- Student ID 2: Boon, major CS.
- Student ID 99: HTTP 404 with `{ "error": "Student not found" }`.
- Major IT filter: Alice and Cherry only.

## Push to the assignment repository

From the folder that contains `student-api-express`:

```powershell
git clone https://github.com/Captansleepy/Student-API-Assignment.git
cd Student-API-Assignment
```

Copy the `student-api-express` folder into the cloned repository, then run:

```powershell
git add student-api-express
git status
git commit -m "Complete Student API in Express assignment"
git push origin main
```

Before committing, confirm `node_modules/` is not listed by `git status`.

## Git ignore

The project `.gitignore` excludes:

```text
node_modules/
.env
```
