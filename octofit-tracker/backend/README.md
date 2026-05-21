# Octofit Tracker - Backend API

Express.js backend API for the Octofit Tracker fitness application, built with Node.js and TypeScript.

## Getting Started

### Prerequisites
- Node.js 18 or higher
- npm or yarn

### Installation

```bash
npm install
```

### Development

Run the development server with automatic reload:

```bash
npm run dev
```

The API will be available at `http://localhost:3001`

### Build

Compile TypeScript to JavaScript:

```bash
npm run build
```

### Production

Build and start the production server:

```bash
npm run build
npm start
```

### Type Checking

Check TypeScript types without emitting:

```bash
npm run type-check
```

### Linting

Check code quality:

```bash
npm run lint
```

## Project Structure

```
backend/
├── src/
│   ├── index.ts          # Entry point and main server
│   ├── routes/           # API route handlers
│   ├── controllers/      # Business logic
│   ├── models/           # Data models and types
│   ├── middleware/       # Custom middleware
│   └── utils/            # Utility functions
├── dist/                 # Compiled JavaScript (generated)
├── tsconfig.json         # TypeScript configuration
├── package.json          # Dependencies and scripts
├── .env.example          # Environment variables template
├── .eslintrc.cjs         # ESLint configuration
└── README.md             # This file
```

## API Endpoints

### Health Check
- `GET /api/health` - Check API health status

### Main API
- `GET /api` - API documentation and available endpoints

### Resources (Coming Soon)
- `GET /api/users` - List all users
- `GET /api/workouts` - List all workouts
- `GET /api/goals` - List all fitness goals

## Environment Variables

Copy `.env.example` to `.env` and configure:

```bash
cp .env.example .env
```

- `PORT` - Server port (default: 3001)
- `NODE_ENV` - Environment (development/production)
- `DATABASE_URL` - Database connection string
- `API_KEY` - API authentication key

## Technologies

- **Express.js** - Web framework
- **TypeScript** - Type-safe JavaScript
- **CORS** - Cross-Origin Resource Sharing
- **dotenv** - Environment configuration
- **ESLint** - Code linting
- **tsx** - TypeScript execution for development

## Features

- ✨ TypeScript for type safety
- 🚀 Express.js with CORS support
- 🔧 Development server with auto-reload (tsx watch)
- 📝 Comprehensive error handling
- 🎯 RESTful API structure
- 📦 Production build optimization

## License

MIT
