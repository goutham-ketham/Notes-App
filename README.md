# Notes App – React Native

A simple and user-friendly mobile notes application built using **React Native, Expo, TypeScript, and SQLite**. The application allows users to create, view, edit, and delete notes, with data stored locally on the device using SQLite.

## Features

- **Create Notes:** Add new notes with a title and content.
- **View Notes:** Display all saved notes in an organized list.
- **Edit Notes:** Update the title and content of existing notes.
- **Delete Notes:** Remove unwanted notes.
- **Local Database:** Store notes locally using SQLite.
- **Persistent Storage:** Retain notes even after closing and reopening the application.
- **Dark Theme:** Clean dark-themed user interface with red accent colors.
- **Empty State:** Display a helpful message when no notes are available.

## Tech Stack

- **React Native** – Mobile application development.
- **Expo** – Development and application tooling.
- **TypeScript** – Type-safe development.
- **Expo SQLite** – Local database management.
- **Expo Router** – Application navigation.
- **React Hooks** – State management and lifecycle handling.

## Project Structure

```text
Notes-App/
│
├── .claude/
├── .vscode/
├── app/
│   └── Application screens and navigation
│
├── assets/
│   └── Images and other static resources
│
├── db/
│   └── Database configuration and operations
│
├── .gitignore
├── AGENTS.md
├── app.json
├── bun.lock
├── eslint.config.js
├── expo-env.d.ts
├── package.json
├── README.md
└── tsconfig.json
```

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/goutham-ketham/Notes-App.git
```

### 2. Navigate to the Project Directory

```bash
cd Notes-App
```

### 3. Install Dependencies

```bash
npm install
```

### 4. Start the Application

```bash
npx expo start
```

Run the application using an Android emulator, iOS simulator, or Expo Go.

## Database

This application uses **Expo SQLite** for local data storage.

The SQLite database contains a `notes` table with the following fields:

| Column | Description |
|---|---|
| id | Unique identifier for each note |
| title | Title of the note |
| content | Main content of the note |
| createdAt | Date and time when the note was created |

Database operations include:

- `addNote()` – Insert a new note.
- `getNotes()` – Retrieve all saved notes.
- `updateNote()` – Update an existing note.
- `deleteNote()` – Delete a note.
- `initDatabase()` – Initialize the database and create the notes table.

## Future Improvements

- Add search functionality to find notes quickly.
- Implement note categories and tags.
- Add light and dark theme switching.
- Support note pinning and favorites.
- Add cloud synchronization and backup.

## License

This project is developed for learning and educational purposes.
