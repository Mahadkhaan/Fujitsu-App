#  Fujitsu Help Desk Ticketing System

A web-based Help Desk Ticket Management System built with **Flask** and **SQLite**, designed for internal use at Fujitsu. The application supports role-based access for both administrators and regular users, enabling secure creation, tracking, and management of IT support tickets.



##  Live Demo

 [Click here to access the deployed app on Heroku](https://ticket-management-fuji-3a9bed13a4ed.herokuapp.com)

---

##  Demo Login Credentials

###  Admin
- **Email:** qaadmin@fujitsu.com  
- **Password:** `Fujitsu123@`

###  Regular User
- **Email:** qauser@fujitsu.com  
- **Password:** `Fujitsu123@`

---

##  Features

###  Modular Codebase
- Clean structure separating routes, templates, models, and config
- Scalable design with room for features like email notifications or ticket statuses
  
---

###  All Users
- Register and log in securely
- Select role (User or Admin) from home screen
- Success/error/validation messages
- Secure logout

###  Regular User
- Create, view, and update personal support tickets
- Filter and view tickets by category
- Add comments/remarks to tickets

###  Admin
- View all tickets (user and admin)
- Create, update, delete any ticket
- Filter tickets by category
- Add comments to any ticket

---

##  Database Design

The system uses a relational database with the following tables:
- `users` – User credentials and roles
- `categories` – Predefined ticket categories
- `tickets` – Main support ticket records
- `comments` – Ticket-specific threaded comments

---

##  Tech Stack

- **Backend:** Python, Flask, SQLAlchemy
- **Frontend:** HTML, CSS, Jinja2, Bootstrap (CDN)
- **Auth:** Flask-Login, Werkzeug Security
- **Database:** SQLite (with Flask-Migrate for migrations)
- **Deployment:** Heroku
- **IDE:** Visual Studio Code

---

###  Comments
- Add remarks or updates to support tickets
- Comment visibility based on ticket access

---

###  Validation & Feedback
- Client-side and server-side validation for all forms
- Flash messages for success, errors, and warnings


##  Installation

To run the app locally:

1. **Clone the repository:**
   
   git clone https://github.com/Mahadkhaan/Fujitsu-App.git
   cd Fujitsu-App

## 2. Set up a virtual environment

python -m venv venv

## 3. Activate it

Windows:

venv\Scripts\activate

macOS/Linux:

source venv/bin/activate

## 4. Install the requirements

pip install -r requirements.txt

## 5.Run the app

flask run

## 6. Open your browser and go to:

http://localhost:5000

## Notes
All dependencies are listed in requirements.txt

The database is pre-populated with sample data (users, tickets, categories)

App uses flash messages for validation feedback

The UI is minimal and responsive via Bootstrap CDN

