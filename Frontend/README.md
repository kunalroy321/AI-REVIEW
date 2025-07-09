# Frontend - AI Review

This is the frontend application for the AI Review project. It is built using React and Vite, providing a fast and modern development experience.

## Table of Contents
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Available Scripts](#available-scripts)
- [Configuration](#configuration)
- [Project Details](#project-details)
- [Linting](#linting)
- [Assets](#assets)
- [Build & Deployment](#build--deployment)
- [Contact](#contact)

---

## Project Structure
```
Frontend/
├── eslint.config.js         # ESLint configuration for code linting
├── index.html               # Main HTML file
├── package.json             # Project dependencies and scripts
├── README.md                # Project documentation
├── vite.config.js           # Vite configuration
├── public/                  # Static assets
│   └── vite.svg             # Example static asset
└── src/                     # Source code
    ├── App.css              # App-level CSS
    ├── App.jsx              # Main React component
    ├── index.css            # Global CSS
    ├── main.jsx             # Entry point for React
    └── assets/              # Image and static assets
        └── react.svg        # Example asset
```

## Getting Started

### Prerequisites
- [Node.js](https://nodejs.org/) (v16 or higher recommended)
- [npm](https://www.npmjs.com/) or [yarn](https://yarnpkg.com/)

### Installation
1. Navigate to the `Frontend` directory:
   ```sh
   cd Frontend
   ```
2. Install dependencies:
   ```sh
   npm install
   # or
   yarn install
   ```

### Running the Development Server
Start the app in development mode with hot reloading:
```sh
npm run dev
# or
yarn dev
```
The app will be available at [http://localhost:5173](http://localhost:5173) by default.

## Available Scripts
- `npm run dev` / `yarn dev`: Start the development server
- `npm run build` / `yarn build`: Build the app for production
- `npm run preview` / `yarn preview`: Preview the production build
- `npm run lint` / `yarn lint`: Run ESLint to check for code issues

## Configuration
- **Vite**: Configuration is in `vite.config.js`. You can customize server port, proxy, and other Vite options here.
- **ESLint**: Linting rules are defined in `eslint.config.js`.

## Project Details
- **React**: The app is built using React (see `src/App.jsx` and `src/main.jsx`).
- **Styling**: CSS files are located in `src/` for both global and component-level styles.
- **Assets**: Place images and static files in `src/assets/` or `public/`.
- **Entry Point**: The app starts from `src/main.jsx` which renders `App.jsx`.

## Linting
To maintain code quality, run ESLint:
```sh
npm run lint
# or
yarn lint
```
You can adjust linting rules in `eslint.config.js`.

## Build & Deployment
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

## Contact
For questions or support, please contact the project maintainer.
