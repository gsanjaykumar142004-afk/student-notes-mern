# Student Notes — MERN CRUD App

A two-tier full-stack notes management application built with MongoDB, Express, React (Vite), and Node.js.

## Candidate Details
- **Name:** G.Sanjay kumar
- **Student ID:** 2026201011
- **GitHub Repository:** <https://github.com/gsanjaykumar142004-afk/student-notes-mern>

## Tech Stack
- **Frontend:** React (Vite) + Axios
- **Backend:** Node.js + Express
- **Database:** MongoDB (via Mongoose)

## Project Structure
```
student-notes-mern/
|-- server/       # Express + MongoDB backend
|-- client/       # Vite + React frontend
|-- screenshots/  # Proof-of-functionality screenshots
```

## Prerequisites
- Node.js (v18+ recommended)
- MongoDB running locally on the default port (`mongodb://localhost:27017`)

## Setup & Run Instructions

### 1. Clone and enter the project
```bash
git clone <https://github.com/gsanjaykumar142004-afk/student-notes-mern.git>
cd student-notes-mern
```

### 2. Start the backend server
```bash
cd server
npm install
npm start
```
The server starts on **http://localhost:5000** and connects to `mongodb://localhost:27017/notes_db`.

### 3. Start the frontend client
Open a new terminal:
```bash
cd client
npm install
npm run dev
```
The React app starts on **http://localhost:5173**.

### 4. Use the app
Open http://localhost:5173 in your browser. You can:
- Add a note (title + content)
- View all notes, newest first
- Delete a note

## API Endpoints
| Method | Endpoint          | Description                     |
|--------|-------------------|----------------------------------|
| POST   | `/api/notes`      | Create a new note (201 Created) |
| GET    | `/api/notes`      | Get all notes, newest first     |
| DELETE | `/api/notes/:id`  | Delete a note by ID             |

## Notes
- CORS is enabled on the server to allow requests from `http://localhost:5173`.
- Loading and empty states are handled on the client ("No notes yet — add one above!").
- Screenshots demonstrating CRUD functionality are in the `screenshots/` folder.
