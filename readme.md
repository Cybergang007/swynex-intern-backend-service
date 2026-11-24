# swynex-intern-backend-service
# Intern Backend Service

A simple backend API service built using Node.js, Express.js, and TypeScript.

## Features

- REST API using Express.js
- Health-check endpoint
- Environment variable configuration using dotenv
- JSON response handling
- 404 error handling
- TypeScript support

## Technologies Used

- Node.js
- Express.js
- TypeScript
- dotenv
- npm

## Project Structure

```text
intern-backend-service/
├── src/
│   └── server.ts
├── .env.example
├── .gitignore
├── package.json
├── tsconfig.json
└── README.md
```

## Installation and Setup

### 1. Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd intern-backend-service
```

### 2. Install dependencies

```bash
npm install
```

### 3. Configure environment variables

Create a `.env` file using:

```bash
cp .env.example .env
```

For Windows PowerShell:

```powershell
Copy-Item .env.example .env
```

### 4. Start the development server

```bash
npm run dev
```

Server runs at:

`http://localhost:3000`

## API Endpoints

### GET /

Returns a welcome message.

### GET /health

Checks whether the backend service is running.

Example response:

```json
{
  "status": "ok",
  "service": "intern-backend-service",
  "environment": "development",
  "timestamp": "2026-01-01T00:00:00.000Z"
}
```

## Environment Variables

| Variable | Description | Default |
|---|---|---|
| PORT | Server port | 3000 |
| NODE_ENV | Application environment | development |

## Build and Production

Build the TypeScript project:

```bash
npm run build
```

Start the compiled server:

```bash
npm start
```

## Testing

Open the following URL in your browser:

`http://localhost:3000/health`

A successful response returns HTTP 200.

## Author
RITHIK R
Developed as part of an internship backend API development task.
