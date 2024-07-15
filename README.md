# Water Usage Management Application

## Overview
This is a water usage management application that allows users to monitor their water consumption, set usage goals, receive real-time data from smart meters, generate usage reports, and receive leak detection alerts.

## Features
- **Monitor Water Usage**: Track daily, weekly, and monthly water usage.
- **Set Usage Goals**: Set personal water usage goals and receive notifications.
- **Real-Time Data Integration**: Integrate with smart meters for real-time data.
- **Generate Usage Reports**: Generate detailed water usage reports.
- **Leak Detection Alerts**: Detect potential water leaks and notify users.

## Project Structure
water_usage_management/
│
├── app.py # Main application file
├── database.py # Database configuration and initialization
├── models.py # Database models
├── notifications.py # Notification system
├── report.py # Report generation logic
├── utils.py # Utility functions
├── requirements.txt # Python dependencies
└── README.md # Project documentation

## Setup Instructions

### Prerequisites
- Python 3.7 or higher
- pip (Python package installer)

### Installation
1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/water_usage_management.git
    cd water_usage_management
    ```

2. **Create and activate a virtual environment** (optional but recommended):
    ```bash
    python3 -m venv venv
    source venv/bin/activate   # On Windows use `venv\Scripts\activate`
    ```

3. **Install dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

### Database Initialization
1. **Initialize the database**:
    ```bash
    python database.py
    ```

### Running the Application
1. **Start the application**:
    ```bash
    python app.py
    ```

The application will be available at `http://127.0.0.1:5000`.

### API Endpoints

- **Monitor Water Usage**: `GET /monitor?user_id=<user_id>`
- **Set Usage Goals**: `POST /set_goal`
  ```json
  {
    "user_id": 1,
    "goal": 500
  }

