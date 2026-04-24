# Job Hunt Agent

An intelligent job search assistant that analyzes resumes and finds relevant job opportunities.

## Features

- User authentication with JWT
- Resume upload and AI-powered analysis
- Job matching based on skills, experience, and location
- Email notifications for new job matches
- Responsive web interface

## Tech Stack

- Frontend: Next.js with TypeScript and Tailwind CSS
- Backend: Node.js with Express
- Database: MongoDB
- Authentication: JWT

## Setup

1. Install Node.js and MongoDB
2. Clone the repository
3. Install dependencies:

   ```bash
   # Frontend
   cd frontend
   npm install

   # Backend
   cd ../backend
   npm install
   ```

4. Set up environment variables in backend/.env:

   ```
   MONGODB_URI=mongodb://localhost:27017/jobhunt
   JWT_SECRET=your_secret_key
   EMAIL_USER=your_email@gmail.com
   EMAIL_PASS=your_email_password
   ```

5. Start the backend:

   ```bash
   cd backend
   npm run dev
   ```

6. Start the frontend:

   ```bash
   cd frontend
   npm run dev
   ```

7. Open http://localhost:3000

## API Endpoints

- POST /api/auth/register - User registration
- POST /api/auth/login - User login
- POST /api/resume/upload - Upload and analyze resume
- POST /api/jobs/match - Get job matches
- POST /api/notifications/preference - Set notification preferences

## Deployment

The application can be deployed to platforms like Vercel (frontend) and Heroku/AWS (backend).