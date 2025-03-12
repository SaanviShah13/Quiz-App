# Quiz App

## 📌 Overview
The **Quiz App** is an interactive web application that allows users to take quizzes, track their scores, and improve their knowledge. This project includes a backend for managing quiz data and user progress.

## 🚀 Features
- User authentication & session management
- Create, read, update, and delete quizzes
- Multiple-choice questions with instant feedback
- Score tracking and leaderboard system
- Responsive UI for mobile and desktop

## 🛠️ Tech Stack
- **Frontend**: React.js / HTML, CSS, JavaScript
- **Backend**: Node.js, Express.js
- **Database**: MongoDB / PostgreSQL (Specify which one you're using)
- **Authentication**: JWT (JSON Web Tokens)
- **Other Dependencies**: (e.g., Mongoose, Sequelize, bcrypt, dotenv, etc.)

## 📂 Project Structure
```
Quiz-App/
│-- src/
│   ├── components/    # Reusable UI components
│   ├── pages/         # Page views (Quiz, Results, etc.)
│   ├── services/      # API call functions
│   ├── assets/        # Images, icons, styles
│-- backend/
│   ├── controllers/   # Business logic
│   ├── models/        # Database models
│   ├── routes/        # API routes
│   ├── middleware/    # Authentication & validation
│   ├── config/        # Database and environment configurations
│-- server.js          # Entry point of the backend
│-- .env               # Environment variables
│-- package.json       # Project dependencies
│-- README.md          # Project documentation
```

## 🔧 Installation & Setup

1. **Clone the repository**
   ```sh
   git clone https://github.com/SaanviShah13/Quiz-App.git
   cd Quiz-App
   ```

2. **Install dependencies**
   ```sh
   npm install
   ```

3. **Set up environment variables**
   - Create a `.env` file in the root directory and add the necessary configurations:
   ```env
   PORT=5000
   DATABASE_URL=<your_database_url>
   JWT_SECRET=<your_secret_key>
   ```

4. **Run the backend server**
   ```sh
   npm start
   ```
   The backend will run on `http://localhost:5000`.

5. **Run the frontend** (if applicable)
   ```sh
   cd client
   npm start
   ```
   The frontend will run on `http://localhost:3000`.

## 📡 API Endpoints
| Method | Endpoint           | Description            | Authentication |
|--------|------------------|------------------------|---------------|
| POST   | `/api/auth/register` | Register a new user | ❌ |
| POST   | `/api/auth/login` | User login & token generation | ❌ |
| GET    | `/api/quizzes` | Get all quizzes | ✅ |
| POST   | `/api/quizzes` | Create a new quiz | ✅ |
| GET    | `/api/quizzes/:id` | Get quiz details | ✅ |
| POST   | `/api/quizzes/:id/submit` | Submit quiz answers | ✅ |

**✅ = Requires authentication (JWT Token)**

## 🛠️ Future Enhancements
- Add support for different quiz formats (true/false, matching, etc.)
- Implement a timer for quizzes
- Gamification features (badges, streaks)
- Social sharing for scores



