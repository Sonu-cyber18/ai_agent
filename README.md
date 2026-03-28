# Nexus AI - Advanced Agentic Platform

Nexus AI is a powerful, secure, and intelligent platform built with Django. It integrates advanced AI reasoning capabilities with a robust authentication system, providing a secure environment for AI-driven interactions.

## 🚀 Features

- **Advanced AI Reasoning**: Integration with state-of-the-art models for complex problem-solving.
- **Secure Authentication**: 
  - JWT-based authentication for stateless security.
  - Multi-factor authentication support (OTP verification).
  - Secure password recovery system.
- **Administrative Oversight**: Dedicated Overseer dashboard for monitoring and managing AI interactions.
- **Robust Backend**: Built with Django 5.x and PostgreSQL.
- **Email Integration**: Automated email notifications and verification via SMTP.
- **Customizable**: Flexible and modular architecture using Django apps (`accounts`, `agent`).

## 🛠️ Technology Stack

- **Framework**: [Django](https://www.djangoproject.com/)
- **API**: [Django REST Framework](https://www.django-rest-framework.org/)
- **Authentication**: [Simple JWT](https://django-rest-framework-simplejwt.readthedocs.io/)
- **Database**: [PostgreSQL](https://www.postgresql.org/)
- **AI Integration**: Custom agent logic with external API support (e.g., OpenRouter).
- **Styling**: Vanilla CSS with modern aesthetics.

## 📦 Installation

### 1. Clone the Repository
```bash
git clone <repository-url>
cd ai
```

### 2. Set Up Virtual Environment
```bash
python -m venv venv
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Environment Variables
Create a `.env` file in the root directory and add the following:
```env
DEBUG=True
SECRET_KEY=your-secret-key
ALLOWED_HOSTS=localhost 127.0.0.1

DB_NAME=aiagentdb
DB_USER=postgres
DB_PASSWORD=your-db-password
DB_HOST=localhost
DB_PORT=5432

EMAIL_HOST_USER=your-email@gmail.com
EMAIL_HOST_PASSWORD=your-app-password
OPENROUTER_API_KEY=your-api-key
```

### 5. Database Migrations
```bash
python manage.py makemigrations
python manage.py migrate
```

### 6. Run the Development Server
```bash
python manage.py runserver
```

## 🏗️ Project Structure

- `accounts/`: Handles user authentication, custom user model, and OTP logic.
- `agent/`: Contains the core AI reasoning and interaction logic.
- `static/`: Static assets (CSS/JS).
- `templates/`: HTML templates for the frontend.
- `ai/`: Core project settings and configuration.

## 🔒 Security

This project follows best practices for security:
- Sensitive credentials are stored in `.env`.
- JWT tokens for secure API access.
- Throttling enabled to prevent brute-force attacks.
- Robust logging for audit trails.

## 📄 License

[MIT License](LICENSE) (If applicable)

---
Developed with ❤️ by Antigravity AI
