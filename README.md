# Phishing Simulation Platform

## Overview
A comprehensive full-stack web application for phishing simulation and security awareness training, built with a modern, modular architecture.

## Tech Stack
- **Frontend**: React (Vite)
- **Backend**: NestJS
- **Shared Libraries**: TypeScript
- **Containerization**: Docker

## Project Structure
```
packages/
├── frontend/           # React frontend (Vite)
├── management-server/  # NestJS management server
├── simulation-server/  # NestJS simulation server
└── shared/             # Shared TypeScript utilities
```

## Prerequisites
- Node.js (v18+)
- Docker
- Docker Compose

## Local Development Setup

### 1. Clone the Repository
```bash
git clone <repository_url>
cd phishing-platform
```

### 2. Install Dependencies
```bash
npm install
```

### 3. Configure Environment
Copy and modify environment files:
```bash
cp frontend/.env.example frontend/.env
cp management-server/.env.example management-server/.env
cp simulation-server/.env.example simulation-server/.env
```

### 4. Development Servers
- Frontend: `npm run dev:frontend` (http://localhost:5173)
- Management Server: `npm run dev:management` (http://localhost:3000)
- Simulation Server: `npm run dev:simulation` (http://localhost:3001)

## Docker Deployment

### Build and Run
```bash
docker-compose up --build -d
```

### Stop Containers
```bash
docker-compose down
```

## Key Features
- User authentication
- Phishing campaign management
- Simulation email tracking
- Security awareness tracking

## Security
- JWT authentication
- Strong password validation
- Custom error handling

## Contributing
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License
[Your License Here - e.g., MIT]
