# Pixel Grid Project

<img width="614" height="582" alt="Pixel Grid App" src="https://github.com/user-attachments/assets/e4664557-457d-45c1-97f3-81b1833ba1ac" />

## Overview

This project was developed as the final milestone of my Full Stack learning path on Mimo. It represents my first complete application built with both frontend and backend fully integrated.

The Pixel Grid is a simple interactive canvas where users can select a color and paint individual cells. Every action is persisted in a database, making the application state consistent and dynamic.

This project marks an important transition in my development journey: moving from isolated exercises to building a functional system that connects UI, server logic, and data persistence.

---

## Tech Stack

Frontend:
- React (Vite)
- CSS

Backend:
- Node.js
- Express

Database:
- SQLite (better-sqlite3)

---

## Features

- Interactive pixel grid (20x20)
- Color selection toolbar
- Click-to-paint functionality
- Persistent state using SQLite
- Backend API handling grid updates
- Full frontend-backend communication via HTTP

---

## How It Works

1. The frontend fetches the grid data from the backend (`/grid`).
2. Each cell is rendered based on its position (x, y) and stored color.
3. When a user clicks a cell:
   - The selected color is sent to the backend (`/setGridColor`)
   - The database is updated
   - The updated grid is returned
4. The frontend re-renders with the new state

---

## Challenges Faced

This project was not just about writing code, but about understanding how different parts of a system interact. Some key challenges included:

- Setting up a local Node.js environment correctly (PATH issues, execution policies)
- Understanding why `.jsx` files cannot be executed directly by Node
- Configuring Vite and fixing module resolution errors
- Debugging frontend not rendering due to incorrect entry files
- Handling CORS and JSON parsing in Express
- Ensuring the backend server was actually running and accessible
- Fixing database initialization errors ("directory does not exist")
- Structuring the project into frontend and backend properly
- Connecting UI interactions to backend logic in a reliable way

Each of these issues required investigation, testing, and iteration. Solving them helped build a deeper understanding of full stack development beyond tutorials.

---

## Project Structure
