# Backend - AI Review

This is the backend server for the AI Review project. It is built with Node.js and Express, providing RESTful API endpoints to support the frontend application.

## Table of Contents
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Available Scripts](#available-scripts)
- [Configuration](#configuration)
- [API Endpoints](#api-endpoints)
- [Project Details](#project-details)
- [Development Notes](#development-notes)
- [Contact](#contact)

---

## Project Structure
```
Backend/
├── package.json             # Project dependencies and scripts
├── server.js                # Entry point for starting the server
├── temp.js                  # Temporary or experimental code
└── src/                     # Source code
    ├── app.js               # Express app setup
    ├── controllers/         # Route controllers
    │   └── ai.controller.js # AI-related controller logic
    ├── routes/              # API route definitions
    │   └── ai.routes.js     # AI-related routes
    └── services/            # Business logic/services
        └── ai.service.js    # AI service logic
```

## Getting Started

### Prerequisites
- [Node.js](https://nodejs.org/) (v16 or higher recommended)
- [npm](https://www.npmjs.com/)

### Installation
1. Navigate to the `Backend` directory:
   ```sh
   cd Backend
   ```
2. Install dependencies:
   ```sh
   npm install
   ```

### Running the Server
Start the backend server:
```sh
npm start
```
By default, the server listens on port 3000 (or as configured in `server.js`).

## Available Scripts
- `npm start`: Start the server
- `npm run dev`: Start the server with hot reloading (if using nodemon)
- `npm install`: Install dependencies

## Configuration
- **Express**: Main app logic is in `src/app.js`.
- **CORS**: Enabled for cross-origin requests.
- **JSON Parsing**: Enabled for incoming requests.
- **Routes**: All `/ai` routes are handled by `src/routes/ai.routes.js`.

## API Endpoints
- `GET /` — Health check endpoint, returns `Hello World`.
- `POST /ai/...` — AI-related endpoints (see `src/routes/ai.routes.js` and `src/controllers/ai.controller.js` for details).

## Project Details
- **Controllers**: Handle request/response logic (see `src/controllers/`).
- **Services**: Contain business logic, especially for AI features (see `src/services/`).
- **Routes**: Define API endpoints and route requests to controllers.
- **Modularity**: The codebase is organized for scalability and maintainability.

## Development Notes
- Use `temp.js` for experiments or temporary scripts.
- Update or add environment variables as needed for production.
- For advanced features, consider adding logging, error handling, and environment configuration.

## Contact
For questions or support, please contact the project maintainer.
