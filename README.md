# Keep - Note Taking Application

A simple and efficient note-taking application built with Node.js, Express, and PostgreSQL.

## Features

- Create new notes
- View all notes
- Delete notes
- Persistent storage with PostgreSQL database

## Prerequisites

- Node.js (v14 or higher)
- PostgreSQL
- npm or yarn

## Environment Variables

Create a `.env` file in the root directory with the following variables:

```env
DB_USER=your_database_user
DB_HOST=your_database_host
DB_NAME=your_database_name
DB_PW=your_database_password
```

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd Keep
```

2. Install dependencies:
```bash
npm install
```

3. Set up the database:
```sql
CREATE TABLE notes (
    id SERIAL PRIMARY KEY,
    title VARCHAR(255) NOT NULL,
    metadata TEXT
);
```

## Running the Application

1. Start the server:
```bash
npm start
```

The server will run on `http://localhost:3001`

## API Endpoints

- `GET /notes` - Retrieve all notes
- `POST /newNote` - Create a new note
- `DELETE /note/:id` - Delete a note by ID

## Project Structure

- `server/` - Backend server code
  - `server.js` - Main server file with Express setup and database operations

## Technologies Used

- Node.js
- Express.js
- PostgreSQL
- pg (Node.js PostgreSQL client)


<img width="1440" alt="Screenshot 2025-03-07 at 3 13 20 PM" src="https://github.com/user-attachments/assets/8519826b-72fd-4eea-896b-8a377d79c71d" />
