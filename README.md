# Django Internship Assignment -- WhatBytes

## Overview

This Django application is built to demonstrate user authentication with email or username and password. It includes pages for login, signup, forgot password, change password, dashboard, and profile. The application restricts access to certain pages based on authentication status.

## Features

1. **Login Page**: Allows users to log in with username/email and password.
2. **Sign Up Page**: Enables new users to register with a username, email, and password.
3. **Forgot Password Page**: Sends a password reset link to the user's email.
4. **Change Password Page**: Allows authenticated users to change their password.
5. **Dashboard**: Displays a greeting message to authenticated users and provides navigation links.
6. **Profile Page**: Displays user information and allows navigation back to the dashboard or logout.

## Setup Instructions

### Prerequisites

- Python 3.6 or higher
- Django 3.0 or higher

### Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/suraj5621/BreadcrumbsDjango-Internship-Assignment---WhatBytes.git
   cd BreadcrumbsDjango-Internship-Assignment---WhatBytes

2  **Create and activate a virtual environment:**
    
     python -m venv .venv
     On linux or macOS, use source .venv/bin/activate   
     On Windows, use `.venv\Scripts\activate`

3  **Install Django:**
     
    pip install django

4  **Apply migrations:**
     
    python manage.py migrate

5  **Run the development server:**
     
    python manage.py runserver

6  **Access the application:**
     
    Open your web browser and go to http://127.0.0.1:8000/accounts/login

### Configuration
    Email Backend Configuration
    For actual email sending, configure the email settings in settings.py:
        EMAIL_BACKEND = 'django.core.mail.backends.smtp.EmailBackend'
        EMAIL_HOST = 'your_smtp_host'
        EMAIL_PORT = your_smtp_port
        EMAIL_USE_TLS = True
        EMAIL_HOST_USER = 'your_email@example.com'
        EMAIL_HOST_PASSWORD = 'your_email_password'


    For local testing, you can use the console backend:
        EMAIL_BACKEND = 'django.core.mail.backends.console.EmailBackend'


    




    
