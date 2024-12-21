# Country Info Application

This full-stack application provides information about countries, including their borders, population trends, and flags. Built with Node.js (Express) backend and React (Next.js) frontend, this application demonstrates modern web development practices and clean architecture.

## Prerequisites

Before you begin, ensure you have the following installed:
- Node.js (v18 or higher)
- npm (v9 or higher)

## Installation

### 1. Clone the repository:
```bash
git clone <repository-url>
cd country-info
```

### 2. Install backend dependencies:
```bash
cd backend
npm install
```
### 3. Install frontend dependencies:

```bash
cd ../frontend
npm install
```
## Configuration
Backend Configuration
Create a .env file in the backend directory:
```envPORT=3001
NAGER_API_BASE_URL=https://date.nager.at/api/v3
COUNTRIES_NOW_API_BASE_URL=https://countriesnow.space/api/v0.1
```
Frontend Configuration
Create a .env.local file in the frontend directory:
```envNEXT_PUBLIC_API_BASE_URL=http://localhost:3001/api
Running the Application
```

Start the backend server:

```bash
cd backend
npm run dev
```

In a new terminal, start the frontend development server:

```bash
cd frontend
npm run dev
```

Access the application:

Frontend: http://localhost:3000
Backend API: http://localhost:3001/api

## API Endpoints
Backend Routes

- GET /api/countries

  Returns a list of all available countries
  Response: [{ countryCode: string, name: string }]


- GET /api/countries/:code

  Returns detailed information about a specific country
  Parameters: code - Country code (e.g., 'US', 'GB')
  Response: Country details including borders, population data, and flag URL
  
## Technologies Used
Backend

Node.js
Express.js
Axios
Jest (testing)
ESLint & Prettier

##Frontend

Next.js 14
React 18
Tailwind CSS
Recharts
React Testing Library
ESLint & Prettier

## Troubleshooting
Common Issues
