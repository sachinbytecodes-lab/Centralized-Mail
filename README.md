# Centralized Mail System

A Django-based centralized email management system designed to manage email recipients, reusable email templates, campaigns, and email communication from a single platform.

The project is currently under development. The initial version focuses on building the core Django architecture, authentication, recipient management, email templates, and campaign management.

## 🚀 Project Overview

Organizations often manage emails using multiple tools and manual processes. This project aims to provide a centralized platform where authorized users can create email campaigns, manage recipients, reuse email templates, and monitor email activity.

The system is being developed using **Python and Django**, with a lightweight frontend based on **Bootstrap and HTMX**.

## 🛠️ Technology Stack

* **Backend:** Python, Django
* **Database:** SQLite
* **Frontend:** HTML, Bootstrap, HTMX
* **Email:** SMTP
* **Incoming Email:** IMAP *(planned)*
* **Background Tasks:** Celery + Redis *(planned)*
* **Version Control:** Git, GitHub

## ✨ Initial Features

The initial development version includes:

* User authentication
* Role-based user structure
* Recipient management
* Email template management
* Campaign creation
* Basic email sending through SMTP
* Django-based admin interface

## 🔮 Planned Features

The following features will be implemented in later development stages:

* Role-based access control with detailed permissions
* Campaign approval workflow
* Background email processing using Celery and Redis
* Email delivery and failure tracking
* Reply tracking using IMAP
* Bounce detection
* Email activity and campaign logs
* Audit logging
* Dashboard and email statistics
* Search and filtering
* Improved HTMX-based interactions



## ⚙️ Getting Started

### 1. Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd centralized-mail-system
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

Activate the virtual environment.

**Windows:**

```bash
venv\Scripts\activate
```

**macOS/Linux:**

```bash
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure environment variables

Create a `.env` file in the project root.

Example:

```env
SECRET_KEY=your-secret-key
DEBUG=True

EMAIL_HOST=your-smtp-server
EMAIL_PORT=587
EMAIL_HOST_USER=your-email
EMAIL_HOST_PASSWORD=your-password
EMAIL_USE_TLS=True
```

Do not commit the `.env` file to GitHub.

### 5. Run migrations

```bash
python manage.py migrate
```

### 6. Create an admin user

```bash
python manage.py createsuperuser
```

### 7. Start the development server

```bash
python manage.py runserver
```

Open:

```text
http://127.0.0.1:8000/
```

## 📌 Current Development Status

**Status:** 🚧 In Development

### Completed

* [ ] Django project setup
* [ ] Database configuration
* [ ] User authentication
* [ ] User roles
* [ ] Recipient management
* [ ] Email templates
* [ ] Campaign management
* [ ] SMTP integration

### Planned

* [ ] Campaign approval workflow
* [ ] Celery + Redis integration
* [ ] Background email processing
* [ ] Email status tracking
* [ ] IMAP integration
* [ ] Reply tracking
* [ ] Bounce detection
* [ ] Audit logging
* [ ] Dashboard analytics
* [ ] Testing
* [ ] Deployment

## 🔐 Security

The project will use Django's built-in security features along with environment variables for sensitive configuration.

Sensitive credentials such as SMTP passwords and Django secret keys should never be committed to the repository.

## 🎯 Project Goals

The main goals of this project are to:

* Practice real-world Django application development
* Understand role-based access control
* Learn email integration using SMTP and IMAP
* Implement background task processing
* Work with database-driven workflows
* Build a maintainable backend architecture
* Develop a practical full-stack Python application

## 📄 License

This project is currently intended for educational and portfolio purposes.
