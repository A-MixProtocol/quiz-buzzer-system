## Quiz Buzzer System

## Description

This is a **Software/Web App Quiz Buzzer System** designed for real-time quiz competitions. Teams use smartphones to press a buzzer, and the system automatically logs the order of presses. The operator/projector displays the press order, and points are awarded based on correct answers.

## Features

* Real-time buzzer press tracking
* Automatic press order queue
* Operator interface for marking correct/wrong answers
* Scoreboard tracking
* Works over local Wi-Fi or internet (optional)

## Technologies Used

* Python 3
* Flask (Backend)
* Flask-SocketIO (Real-time communication)
* HTML, CSS, JavaScript (Frontend)

Project Structure

```
quiz_buzzer_system/
├─ app.py             # Flask backend
├─ templates/
│    ├─ team.html     # Team buzzer page
│    └─ operator.html # Operator/projector page
├─ static/
│    └─ main.js       # JS for real-time updates
└─ requirements.txt   # Python dependencies
```

## Setup Instructions

1. Clone the repository:

```bash
git clone <repository-url>
```

2. Install dependencies:

```bash
pip install flask flask-socketio
```

3. Run the app:

```bash
python app.py
```

4. Open the provided URL on:

   * Smartphones (for team buzzer interface)
   * Tablet or projector (for operator interface)

## How to Use

1. Operator starts a question → buzzers unlocked
2. Teams press buzzer → system logs press order
3. Operator marks first team as Correct or Wrong
4. Points are updated automatically and next team gets chance if needed
