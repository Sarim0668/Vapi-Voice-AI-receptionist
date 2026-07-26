# 🏥 AI Voice Receptionist for Hospitals

An AI-powered voice receptionist built using **Vapi**, **FastAPI**, and **SQLite** that automates hospital appointment management through natural voice conversations.

The assistant can interact with patients over voice, understand their requests, and perform appointment-related actions in real time.

---

## ✨ Features

- 📅 Book hospital appointments
- ❌ Cancel existing appointments
- 📋 Retrieve appointments for a specific date
- 🗣️ Natural voice conversations using Vapi
- ⚡ FastAPI REST backend
- 💾 SQLite database integration
- ✅ Request validation using Pydantic
- 🔄 Real-time API responses

---

## 🛠 Tech Stack

- Vapi AI
- FastAPI
- Python
- SQLite
- SQLAlchemy
- Pydantic
- Uvicorn

---

## Project Architecture

```
Patient
    │
    ▼
Vapi Voice Assistant
    │
    ▼
FastAPI Backend
    │
    ▼
SQLite Database
```

---

## API Endpoints

### Schedule Appointment

```
POST /schedule_appointment/
```

Creates a new appointment for a patient.

---

### Cancel Appointment

```
POST /cancel_appointment/
```

Cancels all appointments for a patient on a selected date.

---

### List Appointments

```
GET /list_appointments/
```

Returns all active appointments for a selected day.

---

### List Appointments (Vapi)

```
POST /list_appointments/
```

Returns appointments when called directly by the Vapi assistant.

---

## Database

The project stores appointment records including:

- Patient Name
- Appointment Reason
- Appointment Time
- Cancellation Status
- Creation Timestamp

---

## Example Voice Commands

- "Book an appointment for tomorrow at 3 PM."
- "Cancel my appointment for Friday."
- "Do I have any appointments today?"
- "Show today's appointments."

---

## Future Improvements

- Doctor availability management
- Multi-doctor scheduling
- SMS & Email confirmations
- WhatsApp notifications
- Google Calendar integration
- Authentication
- PostgreSQL support
- Patient history
- Dashboard for hospital staff

---

## Installation

Clone the repository

```bash
git clone https://github.com/yourusername/vapi-hospital-agent.git
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run the backend

```bash
python backend.py
```

The API will start on

```
http://127.0.0.1:4444
```

---

## Author

**Muhammad Sarim**

Computer Science Student | AI Automation Developer | Building AI-powered workflow and voice automation solutions.
