Military Asset Management System (MAMS)

📌 Overview

The Military Asset Management System (MAMS) is a secure, role-based platform designed to help military personnel track, manage, and optimize the movement, assignment, and expenditure of critical assets (vehicles, weapons, ammunition, etc.) across multiple bases.

🔹 Key Features:
✔ Dashboard – Real-time asset metrics (opening/closing balances, net movements, assignments, expenditures).

✔ Purchases – Record & track new asset acquisitions.

✔ Transfers – Manage asset movements between bases with full history.

✔ Assignments & Expenditures – Assign assets to personnel & log usage.

✔ Role-Based Access Control (RBAC) – Secure permissions for Admins, Base Commanders, and Logistics Officers.

🚀 Technologies Used

Frontend
React (Component-based UI)

Tailwind CSS (Styling & Responsive Design)

Axios (API Communication)

React Router (Navigation)

Backend
Node.js (Runtime)

Express.js (API Framework)

JWT (JSON Web Tokens) (Authentication)

SQLITE (Relational Database)

Database (SQLITE Schema)
Users, Roles, UserRoles (RBAC Management)

Bases (Military base locations)

Assets, EquipmentTypes (Inventory tracking)

Purchases, Transfers, Assignments, Expenditures (Transaction logs)

AuditLogs (Security & accountability)

🔧 Installation & Setup
Prerequisites
Node.js (v16+)

npm / yarn

SQLITE

Backend Setup
Clone the repository:

bash
git clone https://github.com/ibrahim9492/Kristalball-Assignment.git
Install dependencies:

bash
npm install
Set up environment variables (.env):

env
PORT=5000
JWT_SECRET=your_jwt_secret
DATABASE_URL=sqlite:///mams.db
Run migrations (if using an ORM like Sequelize):

bash
npx sequelize-cli db:migrate
Start the server:

bash
npm start
Frontend Setup
Navigate to the frontend directory:

Install dependencies:

bash
npm install
Start the React app:

bash
npm run dev
Open in browser:

text
http://localhost:5173

🔐 Role-Based Access Control (RBAC)

Role	Permissions
Admin	Full system access (manage users, roles, all bases).
Base Commander	View & manage assets for assigned base(s). Approve transfers.
Logistics Officer	Record purchases, transfers, assignments, and expenditures for assigned base(s).

📊 Database Schema Overview
https://via.placeholder.com/600x400?text=MAMS+Database+Schema (Placeholder: Actual ER diagram to be added)

Key Tables
Assets – Tracks inventory (current balance, location, status).

Purchases – Logs new asset acquisitions.

Transfers – Records movements between bases.

Assignments – Links assets to personnel.

Expenditures – Logs asset usage (e.g., ammunition spent).

📈 Features in Detail
1. Dashboard
Filterable metrics (date range, base, equipment type).

Net Movement Breakdown (Purchases + Transfers In - Transfers Out).

2. Purchases Page
Add new assets with supplier details.

View historical purchases with filters.

3. Transfer Page
Initiate & track asset movements between bases.

Full audit trail for accountability.

4. Assignments & Expenditures
Assign assets to personnel.

Log expended resources (training, combat, etc.).

📜 License
This project is licensed under MIT License.

