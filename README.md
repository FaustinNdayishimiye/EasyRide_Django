# EasyRide_Django
This system handles  Car Rental process where customer can book, and pay rent. 
# EasyRide_Django
This system handles  Car Rental process where customer can book, and pay rent. 

1. Project Overview (Problem Statement)
# A Car Rental Management System allows customers to:
----------------------------------------------------------

View available cars
Book cars for a specific period
Make payments
Manage bookings

And allows admins to:
-------------------------
Manage cars, customers, bookings, and payments
Track availability, revenue, and usage
#2. User Roles
1️⃣ Admin

Add, update, delete cars
Approve / reject bookings
Manage users
View reports (rentals, income, car usage)

2️⃣ Customer
Register & login
Browse available cars
Book a car
View booking history
Make payments

(Optional later)

3️⃣ Staff / Manager
Handle vehicle handover & return
Update car status

3. Core Features (Functional Requirements)
🔐 Authentication & Authorization

User registration
Login / logout
Role-based access (Admin vs Customer)
Password reset

🚗 Car Management
Car name / model
Brand
Year
Price per day
Availability status
Car image
Fuel type
Transmission type

📅 Booking System

Select rental start date & end date
Check car availability
Auto-calculate total cost
Booking confirmation
Booking status:

Pending
Approved
Active
Completed
Cancelled

💳 Payment (Phase 2 or later)

Record payments
Payment status (Paid / Unpaid)
Payment method (Cash, Mobile Money, Card)

📊 Dashboard & Reports

Total cars
Active bookings
Revenue summary
Most rented cars

4. Non-Functional Requirements

Secure authentication
User-friendly UI
Responsive design (mobile & desktop)
Data validation
Error handling

Performance (avoid double bookings)

5. Database Design (Key Models)
🧑 User (Django Default + Extension)

username
email
role (Admin / Customer)

🚘 Car

id
name
brand
model
year

price_per_day
availability (Boolean)
image
created_at

📄 Booking

id
user (ForeignKey)
car (ForeignKey)
start_date
end_date
total_price
status
created_at

💰 Payment (Optional first version)
booking (OneToOne)
amount
payment_date
payment_method
payment_status


7. Tech Stack
Backend: Django (Python)
Database: SQLite (start) → PostgreSQL (later)

Frontend:
Django Templates
HTML, CSS, Bootstrap / Tailwind
Auth: Django Authentication System
Media: Django media handling (car images)

8. Key Django Concepts You Will Practice
Models & Relationships
Django ORM
Forms & ModelForms
Authentication & Permissions
Class-Based Views / Function-Based Views
Django Admin
Static & Media files
Migrations

9. Development Phases (Very Important)
 Phase 1 – Basic System
===========================

User registration & login
Add cars (Admin)
View cars (Customer)
Book car
Admin approve booking

Phase 2 – Improvements
============================
Availability checking
Booking conflicts prevention
Payment records
Status tracking

 Phase 3 – Advanced
 ===================
 

REST API (Django Rest Framework)
Online payment integration
Email notifications
Deployment (PythonAnywhere / Railway)

10. Minimum Viable Product (MVP)
 -----------------------------
Your MVP should include:
Login & Signup
Car listing
Booking system
Admin approval




DATABASE DESIGN
================

<img width="827" height="820" alt="Database diagram EasyRide" src="https://github.com/user-attachments/assets/60dd7d87-38e6-46b2-abdf-0a9dca8bbeab" />


