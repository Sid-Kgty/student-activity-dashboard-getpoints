
---

# getPoints - Student Achievement Dashboard

**getPoints** is a student achievement dashboard that allows students to log in, upload event details, and receive activity points based on their submissions. Teachers can review and assign points for student activities, with all data stored in a MySQL database. This project is built using **ReactJS** for the frontend, **Node.js** for the backend, and **MySQL** for the database.

## Features
- **Student Dashboard**:
  - Login with email and password.
  - Upload event details: event name, description, tasks performed, and certificates.
  - Receive activity points after teacher approval.
  - Email notifications when points are assigned.

- **Teacher Dashboard**:
  - Login with email and password.
  - Review student submissions: event name, description, and certificates.
  - Accept/reject submissions and assign points.

- **Role-Based Access Control**:
  - Admin manages users and settings.
  - Teachers review and approve student submissions.
  - Students can view and submit events.

## Tech Stack
- **Frontend**: ReactJS
- **Backend**: Node.js, Express
- **Database**: MySQL
- **Hosting**:
  - Frontend: Vercel
  - Backend: Railway.app / Render.com
  - Database: PlanetScale / Railway.app

## Project Structure
```
getPoints/
│
├── frontend/          # ReactJS Frontend
│   ├── public/        # Static files
│   ├── src/           # React components and logic
│   ├── package.json   # Frontend dependencies
│
└── backend/           # Node.js Backend
    ├── config/        # Configuration files (e.g., DB config, .env)
    ├── controllers/   # API route handlers
    ├── models/        # Database models (e.g., User, Event)
    ├── routes/        # API routes
    ├── server.js      # Express server setup
    └── package.json   # Backend dependencies
```

## Setup Instructions

### Prerequisites:
- Node.js (v14 or higher)
- MySQL or compatible database service

### 1. Clone the repository:
```bash
git clone https://github.com/Sid-Kgty/getPoints.git
cd getPoints
```

### 2. Frontend Setup:
1. Navigate to the `frontend` folder:
   ```bash
   cd frontend
   ```
2. Install frontend dependencies:
   ```bash
   npm install
   ```
3. Start the React app:
   ```bash
   npm start
   ```

### 3. Backend Setup:
1. Navigate to the `backend` folder:
   ```bash
   cd backend
   ```
2. Install backend dependencies:
   ```bash
   npm install
   ```
3. Set up your MySQL database and create necessary tables (`users`, `events`, `submissions`, `points`).
4. Start the backend server:
   ```bash
   node server.js
   ```

### 4. Environment Variables:
Make sure to create an `.env` file in the `backend` folder for environment-specific configurations like your database credentials.

### 5. Database Configuration:
Create the database `getPointsDB` and set up the necessary tables for storing data about users, events, submissions, and points.

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature-name`)
3. Commit your changes (`git commit -am 'Add feature'`)
4. Push to the branch (`git push origin feature-name`)
5. Open a Pull Request

## License

This project is open-source and available under the [MIT License](LICENSE).

---
