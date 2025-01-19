
# Quiz Application

## Overview

This is a React-based quiz application where users can take a quiz, navigate through multiple-choice questions (MCQs), and submit their answers to view results. The application uses a backend API built with Express to manage the quiz data and results. The user is required to log in via email before starting the quiz. After completing the quiz, the user can view their score and the correct answers to the questions.

The app leverages various modern technologies such as React, Vite, Tailwind CSS, and Sonner for notifications.

Deployment link: https://cf-quiz-app.vercel.app/

### Key Features:
- Responsive UI
- Exam Logic
- Exam Timer
- Evaluation Page
### Screenshots
![image](https://github.com/user-attachments/assets/612175ec-4994-4f2c-a597-353e2919665d)
![image](https://github.com/user-attachments/assets/90a4e2a2-88ff-45b4-9886-c85a9b8ec748)


### Challenges / Solutions

To evaluate user's answers there are two approaches:
1. Evalutate it in the frontend by passing correct answer along with options - not secure as client gets access to the correct options
2. Evaluate in backend - hard to implement as questions are being fetched from external api rather than server.

#### Solutions
There's two ways to solve this
1. Cryptographic based message signing - sign each question with a securely hashed solution
2. Store questions fetched in a DB .

While Cryptographic based solution is intuitive, the key must be changed on a regular basis. Settled with storing questions in database

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

