# Little Lemon Backend Project
This repository contains a project developed for the Meta Back-End Developer Professional Certificate, designed to handle reservations and user registration functionalities.

## Prerequisites

### Python Version
Ensure that your system is running:
```sh
Python 3.12.1
```

### Pip Installation
To set up pip, execute:
```sh
python get-pip.py
```

### Required Libraries
Install Django and additional libraries by running:
```sh
pip install django psycopg2 Pillow djangorestframework djangorestframework_simplejwt python-dotenv drf-yasg
```

## Project Setup and Execution

### Step 1: Database Migrations
Before launching the project, apply all migrations to set up the database schema:
```sh
python manage.py makemigrations
python manage.py migrate
```

### Step 2: Start the Development Server
You can now start the local development server by running:
```sh
python manage.py runserver
```

### Step 3: Running Tests
For testing the functionalities, use the following command:
```sh
python manage.py test
```

## Available API Endpoints

### 1. **Booking Management:**
   - To view all bookings or create a new booking:
     - `GET /api/bookings/`
     - `POST /api/bookings/`
   - To manage a specific booking (retrieve, update, or delete):
     - `GET /api/bookings/<booking_id>/`
     - `PUT /api/bookings/<booking_id>/`
     - `DELETE /api/bookings/<booking_id>/`

### 2. **User Registration:**
   - Register a new user with the system:
     - `POST /api/registration/`

