# 🚀 AI Review — Full Stack Platform

Welcome to **AI Review**, a modern, scalable, and AI-powered review platform. This monorepo contains both the lightning-fast React + Vite frontend and the robust Node.js + Express backend. Designed for seamless collaboration, rapid iteration, and future-proof extensibility.

---

## 🗂️ Project Structure
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

# 🌐 Frontend — React + Vite

### ⚡ Quickstart
```sh
cd Frontend
npm install   # or yarn install
npm run dev   # or yarn dev
```
Visit: [http://localhost:5173](http://localhost:5173)

### 🛠️ Scripts
- `dev` — Start development server with hot reload
- `build` — Production build
- `preview` — Preview production build
- `lint` — Lint code with ESLint

### ⚙️ Configuration
- **Vite**: `vite.config.js` — customize dev server, proxy, etc.
- **ESLint**: `eslint.config.js` — code quality rules

### 🧩 Details
- **Entry**: `src/main.jsx` → `App.jsx`
- **Styling**: `src/App.css`, `src/index.css`
- **Assets**: `src/assets/`, `public/`

### 🧹 Linting
```sh
npm run lint
```

### 🚀 Build & Deploy
```sh
npm run build
```
Deploy `dist/` to Vercel, Netlify, or any static host.

---

# 🖥️ Backend — Node.js + Express

### ⚡ Quickstart
```sh
cd Backend
npm install
npm start
```
Default: [http://localhost:3000](http://localhost:3000)

### 🛠️ Scripts
- `start` — Start server
- `dev` — Hot reload (with nodemon)
- `install` — Install dependencies

### ⚙️ Configuration
- **Express**: `src/app.js`
- **CORS**: Enabled
- **JSON**: Body parsing enabled
- **Routes**: `/ai` handled by `src/routes/ai.routes.js`

### 🔗 API Endpoints
- `GET /` — Health check (`Hello World`)
- `POST /ai/...` — AI endpoints (see `src/routes/ai.routes.js`)

### 🧩 Details
- **Controllers**: `src/controllers/`
- **Services**: `src/services/`
- **Routes**: `src/routes/`
- **Temp**: `temp.js` for experiments

### 📝 Dev Notes
- Use `.env` for secrets/config (add as needed)
- Extend with logging, error handling, etc.

---

# 🧑‍💻 Contributing & Support
- Open to PRs, issues, and suggestions!
- Maintainer: **Kunal Roy**  
  📞 9883328028  
  ✉️ k98038751@gmail.com

---

> _AI Review — Built for the future. Powered by modern web technologies._