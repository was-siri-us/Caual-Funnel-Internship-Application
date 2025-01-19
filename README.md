
# Quiz Application

## Overview

This is a React-based quiz application where users can take a quiz, navigate through multiple-choice questions (MCQs), and submit their answers to view results. The application uses a backend API built with Express to manage the quiz data and results. The user is required to log in via email before starting the quiz. After completing the quiz, the user can view their score and the correct answers to the questions.

The app leverages various modern technologies such as React, Vite, Tailwind CSS, and Sonner for notifications.

### Key Features:
- Responsive UI
- Exam Logic
- Exam Timer
- Evaluation PAge
---

## Installation Guide

### Prerequisites
- Node.js (>=14)
- npm or yarn
- Express.js for the backend
- Sonner for notifications

### Steps

1. **Clone the repository**:
   ```bash
   git clone <repository_url>
   cd <repository_folder>
   ```

2. **Backend Setup (Express API)**:
   - Navigate to the backend directory and install dependencies:
     ```bash
     cd backend
     npm install
     ```

3. **Frontend Setup (React + Vite)**:
   - Navigate to the frontend directory and install dependencies:
     ```bash
     npm install
     ```

4. **Environment Variables**:
   - Create a `.env` file at the root of the project for both frontend and backend.
   - For the frontend, define the `VITE_API_URL` to point to the backend API.

   Example for the frontend `.env`:
   ```env
   VITE_API_URL=http://localhost:5000
   ```

5. **Run the Development Servers**:
   - **Backend**:
     ```bash
     cd backend
     npm run dev
     ```
   - **Frontend**:
     ```bash
     npm run dev
     ```

6. **Access the Application**:
   - Open your browser and navigate to `http://localhost:5173`.

---

