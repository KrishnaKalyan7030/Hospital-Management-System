# Hospital Management System

A desktop-based Hospital Management System built with Python, Tkinter and SQLite. It also has a text-to-speech token-calling feature that announces each patient's number and name out loud, so patients who can't easily read a screen still know when it's their turn.

**Author:** Krishna Kalyan

## Features

- Add new patient appointments (name, age, gender, location, time, phone)
- Search for a patient and update or delete their record
- A queue screen that calls out patients one by one using voice

## Tech Stack

- Python
- Tkinter (GUI)
- SQLite (database)
- pyttsx3 (text-to-speech)

## Screenshots

Add Appointment screen:

![Add Appointment Screen](screenshots/add_appointment.png)

Update Appointment screen:

![Update Appointment Screen](screenshots/update_appointment.png)

## Database

All data is stored in a single `appointments` table:

- id
- name
- age
- gender
- location
- schedule_time
- phone

## How to Run

Install the only external dependency:

```
pip install pyttsx3
```

Run the file:

```
python HMS.py
```

It has three screens - Add Appointment, Update/Delete Appointment, and Call Patient. Each one opens after you close the previous window.

## Known Limitations

- The three screens open one after another, not at the same time
- No login system, so anyone using the app can see/edit all records
- The Call Patient screen loads patients only once when it opens, so patients added after won't show up until you restart it

## Possible Improvements

- Combine the three screens into one window
- Move to a proper database like PostgreSQL for multiple users
- Add staff login
- Turn this into a web app
