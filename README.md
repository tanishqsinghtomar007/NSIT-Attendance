SmartAttend — Smart Attendance Management System

SmartAttend is a timetable-driven attendance management platform designed to simplify classroom attendance through QR-based check-ins, real-time monitoring, and automated reporting.

The platform provides dedicated dashboards for students, faculty, and administrators, enabling efficient attendance tracking, lecture management, and centralized academic record-keeping.

✨ Key Features

* QR-Based Attendance: Enables students to mark attendance using lecture-specific QR codes.
* Timetable-Driven Scheduling: Allows faculty to confirm, cancel, or reschedule lectures.
* Real-Time Monitoring: Uses WebSockets to deliver live attendance updates to faculty dashboards.
* Student Dashboard: Displays overall attendance percentages and subject-wise breakdowns.
* Faculty Dashboard: Supports lecture management, QR generation, attendance record editing, and Excel/CSV exports.
* Admin Dashboard: Provides student roster management, subject management, audit logs, and low-attendance alerts.
* Attendance Integrity: Implements database constraints to prevent duplicate attendance records and restrict multiple student submissions from the same device within a session.

🛠 Technology Stack

Component	Technologies
Frontend	Next.js 14, TypeScript, Tailwind CSS, Lucide Icons
Backend	Python, FastAPI, SQLAlchemy, Pydantic
Database	PostgreSQL / SQLite
Authentication	Passlib, Bcrypt, PyJWT
Real-Time Communication	FastAPI WebSockets
Reporting	openpyxl, pandas
QR Generation	Python qrcode
Deployment	Docker, Docker Compose

👥 User Roles

Role	Capabilities
Student	View attendance statistics and access QR-based attendance.
Faculty	Manage lectures, conduct attendance, monitor sessions, and export reports.
Administrator	Manage students and subjects, monitor attendance compliance, and review audit logs.

🚀 Getting Started

Prerequisites

* Python
* Node.js and npm
* Docker and Docker Compose (optional)

1. Start the Backend

From the project root:

.\venv\Scripts\python.exe backend/run.py

Backend: http://localhost:8000

2. Start the Frontend

Open a separate terminal:

cd frontend
npm install
npm run dev

Frontend: http://localhost:3000

Alternative: Docker

If Docker Compose is configured:

docker compose up --build

🔒 Security and Attendance Integrity

SmartAttend incorporates session-based attendance validation, database uniqueness constraints, and device-based restrictions to reduce duplicate submissions and discourage proxy attendance.

These mechanisms improve attendance integrity but do not independently guarantee a student’s physical presence.

Future Scope

* Dynamic QR codes with expiration.
* Automated attendance notifications.
* Advanced analytics and reporting.
* Multi-institution and multi-class support.
* Configurable attendance policies.
* Enhanced authentication and security controls.

📌 Project Status

Phase 1 — Prototype

SmartAttend establishes the foundation for a modern attendance management service, combining timetable-driven workflows, QR-based attendance, role-based dashboards, real-time updates, and automated reporting.

⸻

SmartAttend — Simplifying attendance, empowering institutions.
