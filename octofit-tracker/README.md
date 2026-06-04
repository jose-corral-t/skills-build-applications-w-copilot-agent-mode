# OctoFit Tracker

A modern multi-tier fitness tracking application built with React 19, Vite, Node.js/Express, and MongoDB.

## Architecture

- **Frontend**: React 19 + Vite (Port 5173)
- **Backend**: Node.js + Express + TypeScript (Port 8000)
- **Database**: MongoDB (Port 27017)

## Project Structure

```
octofit-tracker/
├── frontend/          # React 19 + Vite application
│   ├── src/
│   ├── index.html
│   ├── vite.config.ts
│   ├── tsconfig.json
│   └── package.json
├── backend/           # Express + TypeScript API
│   ├── src/
│   ├── tsconfig.json
│   └── package.json
└── README.md
```

## Setup Instructions

### Prerequisites
- Node.js (v18+)
- MongoDB (running on port 27017)

### Frontend Setup
```bash
cd frontend
npm install
npm run dev
```
The frontend will be available at `http://localhost:5173`

### Backend Setup
```bash
cd backend
npm install
npm run dev
```
The backend API will be available at `http://localhost:8000`

### Verify Setup
- Health check: `http://localhost:8000/api/health`

## Environment Variables

Copy `.env.example` to `.env` and update as needed:

```env
VITE_API_URL=http://localhost:8000
PORT=8000
MONGODB_URI=mongodb://localhost:27017/octofit-tracker
```

## Available Scripts

### Frontend
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build

### Backend
- `npm run dev` - Start development server with ts-node
- `npm run build` - Compile TypeScript to JavaScript
- `npm start` - Run compiled backend

## Technologies

- React 19
- Vite
- TypeScript
- Express.js
- Mongoose
- MongoDB
