# Multi-Tenant SaaS Task & Workflow Management System

A backend-focused SaaS application designed to help organisations manage workspaces, projects, tasks, and team collaboration through secure REST APIs.

## Features

- Organisation and workspace management
- Project and task creation
- Task assignment and deadline tracking
- Role-Based Access Control (RBAC)
- Organisation-level data isolation
- Task filtering and status management
- Background task processing
- API authentication using JWT

## Tech Stack

- **Language:** Python
- **Backend:** Django REST Framework
- **Database:** PostgreSQL
- **Authentication:** JWT
- **Task Queue:** Celery
- **Caching and Message Broker:** Redis
- **Testing:** Pytest
- **Containerisation:** Docker

## Core Modules

1. **Authentication:** User registration, login, and token-based authentication.
2. **Organisations:** Create and manage separate organisation workspaces.
3. **Projects:** Organise tasks under individual projects.
4. **Tasks:** Create, assign, update, and track tasks.
5. **Permissions:** Control access based on user roles.
6. **Notifications:** Process task-related notifications asynchronously.

## Project Structure

```text
saas-task-workflow-management/
│
├── config/
├── apps/
│   ├── users/
│   ├── organisations/
│   ├── projects/
│   └── tasks/
│
├── tests/
├── requirements.txt
├── .env.example
├── .gitignore
├── Dockerfile
└── README.md
```

## Setup

```bash
git clone <repository-url>
cd saas-task-workflow-management

python -m venv venv
```

Activate on Windows:

```bash
venv\Scripts\activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run database migrations:

```bash
python manage.py migrate
```

Start the development server:

```bash
python manage.py runserver
```

## Project Status

🚧 In Development

## Future Improvements

- Team invitation system
- Advanced analytics dashboard
- Email notifications
- API rate limiting
- Automated testing and CI/CD
- Cloud deployment
