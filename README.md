# Campus Hub - Smart University Resource Management

Campus Hub is a comprehensive web application designed to streamline the management of university resources. It serves Students, Lecturers, Managers, and Administrators, providing a unified platform for room booking, fault reporting, and resource tracking.

## 🚀 Key Features

### 🌟 Premium Features (New!)
*   **📊 Analytics Dashboard for Managers:**
    *   Visual insights into recurring facility issues.
    *   Interactive Bar and Pie charts showing fault frequency by building and category.
    *   Helps identify systemic problems for better infrastructure planning.
*   **📅 Interactive Schedule Calendar:**
    *   Visual weekly calendar for Room Requests.
    *   One-click booking system: Hover over an empty slot to instantly create a pre-filled request.
    *   Color-coded status indicators (Green: Approved, Yellow: Pending, Red: Rejected).
*   **🔔 Real-time Notification Center:**
    *   Instant alerts for important actions (e.g., "Room Request Approved", "New Fault Reported").
    *   Bell icon with unread badge count in the navigation bar.
    *   Smart routing: Clicking a notification takes you directly to the relevant action page.

### Core Functionality
*   **User Role Management:**
    *   Secure authentication with role-based access control (Student, Lecturer, Manager, Admin).
    *   Approval workflow for new Manager and Lecturer enrollments.
*   **Room & Lab Management:**
    *   Browse available classrooms and labs.
    *   View real-time availability and capacity.
    *   Lecturers can request rooms for specific classes or events.
*   **Fault Reporting:**
    *   Report maintenance issues (e.g., Broken Projector, WiFi Issues).
    *   Track the status of reported faults from "Open" to "Resolved".
    *   Managers can update status and assign repair tasks.
*   **Library Status:**
    *   Check library occupancy and open/closed status.

## 🛠️ Technology Stack

*   **Frontend:** React, Tailwind CSS, Lucide React (Icons), Recharts (Analytics), Sonner (Toasts).
*   **Backend:** Python Django, Django REST Framework.
*   **Database:** SQLite (Default for development).
*   **State Management:** React Context API for Authentication.

## 📦 Installation & Setup

### Prerequisites
*   Node.js & npm
*   Python 3.8+

### 1. Backend Setup
```bash
cd backend
# Create virtual environment
python -m venv venv
# Activate virtual environment
# Windows:
.\venv\Scripts\Activate
# Mac/Linux:
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Run migrations
python manage.py migrate

# Create superuser (optional)
python manage.py createsuperuser

# Start server
python manage.py runserver
```

### 2. Frontend Setup
```bash
# In the root directory
npm install

# Start development server
npm run dev
```

The application will be available at `http://localhost:5173`.

## 👥 User Roles & Demo Accounts

*   **Manager:** Can approve requests, view analytics, and manage faults.
    *   Email: `demo_manager@test.com`
    *   Password: `password123`
*   **Lecturer:** Can request rooms and report faults.
    *   Email: `demo_lecturer@test.com`
    *   Password: `password123`

## 🤝 Contributing

1.  Fork the repository.
2.  Create a feature branch (`git checkout -b feature/AmazingFeature`).
3.  Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4.  Push to the branch (`git push origin feature/AmazingFeature`).
5.  Open a Pull Request.
