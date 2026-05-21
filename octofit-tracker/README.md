# Octofit Tracker - Full Stack Application

> A complete fitness tracking application built with React 19, Express.js, TypeScript, and MongoDB

## 🚀 Project Overview

Octofit Tracker is a full-stack web application designed for fitness tracking and goal management. The application is divided into two main parts:

- **Frontend**: React 19 + Vite running on port **5173**
- **Backend**: Express.js + TypeScript running on port **8000**
- **Database**: MongoDB running on port **27017**

## 📋 Prerequisites

- Node.js 16 or higher
- MongoDB (local or Atlas)
- npm or yarn

## 🛠️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/EswarACC/skills-build-applications-w-copilot-agent-mode.git
cd skills-build-applications-w-copilot-agent-mode
git checkout build-octofit-app
```

### 2. Setup Backend

```bash
cd octofit-tracker/backend

# Copy environment variables
cp .env.example .env

# Install dependencies
npm install
```

### 3. Setup Frontend

```bash
cd octofit-tracker/frontend

# Install dependencies
npm install
```

## 🏃 Running the Application

### Start MongoDB (if running locally)

```bash
mongod
```

MongoDB will be accessible at `mongodb://localhost:27017`

### Start the Backend Server

```bash
cd octofit-tracker/backend
npm run dev
```

Backend API will be available at `http://localhost:8000`

### Start the Frontend Development Server

```bash
cd octofit-tracker/frontend
npm run dev
```

Frontend will open automatically at `http://localhost:5173`

## 📡 API Endpoints

### Health Check
- `GET http://localhost:8000/api/health` - Check API health status

### Main API
- `GET http://localhost:8000/api` - API documentation and available endpoints

### Resources (Coming Soon)
- `GET http://localhost:8000/api/users` - List all users
- `GET http://localhost:8000/api/workouts` - List all workouts
- `GET http://localhost:8000/api/goals` - List all fitness goals

## 🗂️ Project Structure

```
octofit-tracker/
├── frontend/                 # React 19 + Vite Application
│   ├── src/
│   │   ├── main.jsx          # Entry point
│   │   ├── App.jsx           # Root component
│   │   ├── App.css           # App styles
│   │   └── index.css         # Global styles
│   ├── index.html
│   ├── vite.config.js        # Vite config (port: 5173)
│   ├── package.json
│   └── README.md
│
└── backend/                  # Node.js + Express + TypeScript
    ├── src/
    │   ├── index.ts          # Express server (port: 8000)
    │   ├── db.ts             # MongoDB connection
    │   └── models/
    │       ├── User.ts       # User schema
    │       ├── Workout.ts    # Workout schema
    │       ├── Goal.ts       # Goal schema
    │       └── index.ts      # Models export
    ├── tsconfig.json
    ├── package.json
    ├── .env.example          # Environment template
    └── README.md
```

## 📦 Technology Stack

### Frontend
- **React 19** - UI library
- **Vite** - Build tool and dev server
- **CSS** - Styling

### Backend
- **Node.js** - JavaScript runtime
- **Express.js** - Web framework
- **TypeScript** - Type-safe JavaScript
- **Mongoose** - MongoDB ODM
- **CORS** - Cross-Origin Resource Sharing
- **dotenv** - Environment configuration

### Database
- **MongoDB** - NoSQL database (port: 27017)

## 🔧 Available Scripts

### Frontend
```bash
cd octofit-tracker/frontend

npm run dev        # Start development server
npm run build      # Create production build
npm run preview    # Preview production build
npm run lint       # Check code quality
```

### Backend
```bash
cd octofit-tracker/backend

npm run dev        # Start development server with auto-reload
npm run build      # Compile TypeScript to JavaScript
npm start          # Run production build
npm run lint       # Check code quality
npm run type-check # Verify TypeScript types
```

## 🌐 Environment Configuration

### Backend `.env` File

Create `octofit-tracker/backend/.env`:

```env
PORT=8000
NODE_ENV=development
DATABASE_URL=mongodb://localhost:27017/octofit-tracker
API_KEY=your_api_key_here
```

## 📱 Features

- ✨ Modern React 19 with hooks
- ⚡ Lightning-fast Vite development
- 🚀 Express.js REST API
- 📘 Full TypeScript support
- 🗄️ MongoDB with Mongoose ODM
- 🔒 CORS security
- 📊 User, Workout, and Goal management (coming soon)

## 🚧 Development Roadmap

- [ ] User authentication and authorization
- [ ] Create/Read/Update/Delete operations for Users
- [ ] Workout logging and tracking
- [ ] Goal setting and progress tracking
- [ ] User dashboard and analytics
- [ ] Advanced filtering and search

## 📝 License

MIT

## 👨‍💻 Author

Built with GitHub Copilot in Agent Mode

---

**Happy Coding!** 🎉

For more information, visit the [GitHub Repository](https://github.com/EswarACC/skills-build-applications-w-copilot-agent-mode)
