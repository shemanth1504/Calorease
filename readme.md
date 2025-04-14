# Calorease

**Calorease** is a fitness and diet tracking web application designed to help users log and monitor their workouts, dietary intake, and weight trends effectively.  

---

## Features

### User Management
- **Signup:** Users can create an account with personal details such as Name, Email, Date of Birth, Weight, and Height.
- **Login:** Secure login with validation for incorrect credentials.
- **Profile Management:** Update personal details (except email), view weight history, and delete accounts.

### Fitness Tracking
- Log workouts with details like Workout Name, Duration, Calories Burned, and Date.
- View, edit, or delete workout entries.

### Dietary Tracking
- Log meals with details like Meal Name, Calories, Protein, Serving Quantity, and Date.
- View, edit, or delete meal entries.

### Visualization
- **Bar Graph:** Display calories burned over time from workouts.
- **Pie Chart:** Show protein and calorie breakdown for meals.
- **Line Graph:** Track weight progression over time.

### Secure Logout
- Users can log out securely, clearing the session and redirecting to the Home Page.

---

## Deployment and Installation Guide

### Technical Specifications
- **Operating System:** Windows 10/11, macOS 13+, or Linux (Ubuntu 20.04+).
- **Frontend:** React.js, Node.js (v14.0+).
- **Backend:** Express.js, MySQL (Database).
- **Others:** NPM (v6.0+), MySQL Workbench or Command-Line Client.

---

### Steps to Deploy/Install

#### Prerequisites
- Ensure **Node.js** and **npm** are installed. [Download Node.js](https://nodejs.org)
- Install **Git**. [Download Git](https://git-scm.com/downloads)

#### Installation Steps
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/naveenaduri/calorease.git
   cd calorease

2. **Set Up Backend:**
   - Navigate to the `backend` directory:
     ```bash
     cd backend
     ```
   - Install the required dependencies:
     ```bash
     npm install
     ```

3. **Set Up Frontend:**
   - Navigate to the `frontend` directory:
     ```bash
     cd ../frontend
     ```
   - Install the required dependencies:
     ```bash
     npm install
     ```

4. **Set Up the Database:**
   - Launch **MySQL Command Line Client** and log in.
   - Create a new database:
     ```sql
     CREATE DATABASE final_project_ssdi;
     ```
   - Create and configure a database user:
     ```sql
     CREATE USER 'ssdi_backend_user'@'host' IDENTIFIED BY 'Qwerty567@';
     GRANT ALL PRIVILEGES ON final_project_ssdi.* TO 'ssdi_backend_user'@'host';
     ```
     Replace `host` with your MySQL host (e.g., `localhost`).
   - Import the database dump:
     ```bash
     SOURCE /path-to-calorease-repository/final_project_ssdi.sql;
     ```

---  