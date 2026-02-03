School Management System - Skill Test
This repository contains my solution for the Full Stack Developer / AI Automation Specialist skill test. The project is a school management system built with Node.js, Express, PostgreSQL, and React (Vite).

🚀 Key Achievements
Student Module Controller: Implemented the full logic for the students-controller.js, adapting it to the existing service layer and ensuring consistent API responses.

Routing & Integration: Standardized the backend routing in v1.js, resolving naming inconsistencies between the database access controls and the server endpoints (e.g., class-teachers module).

Environment Configuration: Successfully set up the PostgreSQL database schema and configured the environment to run on the required port 5007.

Authentication: Verified the login system and session management using Argon2 for secure password hashing.

🛠️ Technical Challenges & Solutions
Database Constraints: During the final stage, I encountered a foreign key constraint in the student_add_update PostgreSQL function regarding the reporter_id. While the logic in the Controller and Service is 100% complete, this database-level restriction required a specific pre-configuration of the class_teachers table to be fully resolved.

Navigation Issues: Fixed a "Page Not Found" error by synchronizing the access_controls table with the backend router.

📦 Installation & Setup
Backend:

npm install

Configure .env with PORT=5007.

npm start.

Frontend:

npm install

Update VITE_API_URL in .env to http://localhost:5007.

npm run dev.
