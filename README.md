# AI Review - Full Stack Project

This repository contains both the frontend and backend for the AI Review project. The frontend is built with React and Vite, while the backend is powered by Node.js and Express. Together, they provide a modern, scalable platform for AI-powered review workflows.

## Table of Contents
- [Project Overview](#project-overview)
- [Project Structure](#project-structure)
- [Frontend](#frontend)
  - [Getting Started](#getting-started-frontend)
  - [Available Scripts](#available-scripts-frontend)
  - [Configuration](#configuration-frontend)
  - [Project Details](#project-details-frontend)
  - [Linting](#linting-frontend)
  - [Build & Deployment](#build--deployment-frontend)
- [Backend](#backend)
  - [Getting Started](#getting-started-backend)
  - [Available Scripts](#available-scripts-backend)
  - [Configuration](#configuration-backend)
  - [API Endpoints](#api-endpoints)
  - [Project Details](#project-details-backend)
  - [Development Notes](#development-notes)
- [Contact](#contact)

---

## Project Overview
AI Review is a full stack application designed to streamline review processes using AI. The frontend provides a fast, interactive UI, while the backend exposes RESTful APIs for AI-powered features.

## Project Structure
```
AI-review/
├── Backend/                 # Node.js + Express backend
│   ├── package.json
│   ├── server.js
│   ├── temp.js
│   └── src/
│       ├── app.js
│       ├── controllers/
│       │   └── ai.controller.js
│       ├── routes/
│       │   └── ai.routes.js
│       └── services/
│           └── ai.service.js
├── Frontend/                # React + Vite frontend
│   ├── eslint.config.js
│   ├── index.html
│   ├── package.json
│   ├── README.md
│   ├── vite.config.js
│   ├── public/
│   │   └── vite.svg
│   └── src/
│       ├── App.css
│       ├── App.jsx
│       ├── index.css
│       ├── main.jsx
│       └── assets/
│           └── react.svg
├── package.json             # (optional) Monorepo root
└── README.md                # Project documentation
```

---

# Frontend

## Getting Started (Frontend)
### Prerequisites
- [Node.js](https://nodejs.org/) (v16 or higher recommended)
- [npm](https://www.npmjs.com/) or [yarn](https://yarnpkg.com/)

### Installation
```sh
cd Frontend
npm install
# or
yarn install
```

### Running the Development Server
```sh
npm run dev
# or
yarn dev
```
The app will be available at [http://localhost:5173](http://localhost:5173) by default.

## Available Scripts (Frontend)
- `npm run dev` / `yarn dev`: Start the development server
- `npm run build` / `yarn build`: Build the app for production
- `npm run preview` / `yarn preview`: Preview the production build
- `npm run lint` / `yarn lint`: Run ESLint to check for code issues

## Configuration (Frontend)
- **Vite**: Configuration is in `vite.config.js`. You can customize server port, proxy, and other Vite options here.
- **ESLint**: Linting rules are defined in `eslint.config.js`.

## Project Details (Frontend)
- **React**: The app is built using React (see `src/App.jsx` and `src/main.jsx`).
- **Styling**: CSS files are located in `src/` for both global and component-level styles.
- **Assets**: Place images and static files in `src/assets/` or `public/`.
- **Entry Point**: The app starts from `src/main.jsx` which renders `App.jsx`.

## Linting (Frontend)
To maintain code quality, run ESLint:
```sh
npm run lint
# or
yarn lint
```
You can adjust linting rules in `eslint.config.js`.

## Build & Deployment (Frontend)
To create a production build:
```sh
npm run build
# or
yarn build
```
The output will be in the `dist/` folder. You can deploy this folder to any static hosting service (e.g., Vercel, Netlify, GitHub Pages).

To preview the production build locally:
```sh
npm run preview
# or
yarn preview
```

---

# Backend

## Getting Started (Backend)
### Prerequisites
- [Node.js](https://nodejs.org/) (v16 or higher recommended)
- [npm](https://www.npmjs.com/)

### Installation
```sh
cd Backend
npm install
```

### Running the Server
```sh
npm start
```
By default, the server listens on port 3000 (or as configured in `server.js`).

## Available Scripts (Backend)
- `npm start`: Start the server
- `npm run dev`: Start the server with hot reloading (if using nodemon)
- `npm install`: Install dependencies

## Configuration (Backend)
- **Express**: Main app logic is in `src/app.js`.
- **CORS**: Enabled for cross-origin requests.
- **JSON Parsing**: Enabled for incoming requests.
- **Routes**: All `/ai` routes are handled by `src/routes/ai.routes.js`.

## API Endpoints
- `GET /` — Health check endpoint, returns `Hello World`.
- `POST /ai/...` — AI-related endpoints (see `src/routes/ai.routes.js` and `src/controllers/ai.controller.js` for details).

## Project Details (Backend)
- **Controllers**: Handle request/response logic (see `src/controllers/`).
- **Services**: Contain business logic, especially for AI features (see `src/services/`).
- **Routes**: Define API endpoints and route requests to controllers.
- **Modularity**: The codebase is organized for scalability and maintainability.

## Development Notes
- Use `temp.js` for experiments or temporary scripts.
- Update or add environment variables as needed for production.
- For advanced features, consider adding logging, error handling, and environment configuration.

---

# Contact
For questions or support, please contact the project maintainer.