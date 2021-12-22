# Event-Planner
Developed with Hung Nguyen and Brandon Luong in CMPE 131. Allows users to login with a created username and password, or login with their Google Account.
Calendar Planner website developed with back-end using Python, Flask, and Javascript FullCalendarAPI. Front-end developed with HTML and CSS. 

Working Demo: https://personal-calendar-1.herokuapp.com/#

## Instructions to Run

### PyCharm (Preferred) 
1. Open Project folder and PyCharm will ask to install all requirements in requirements.txt 
1. Run main.py

## Code and Package Functions 
- [`app`](TaskManagementProject/app)
- [`app/auth.py`](TaskManagementProject/app/auth.py)

    Loads all pages that the website has when signed out (login, signup and homepage). Connects to MongoDB database and handles user login both from Google Authentication and user     created accounts. Loads the calendar of that user when a login is sucessful. If logged in, creates a temporary hidden page with a json file of the events that a user has so       the events can be loaded for that user. To load the events, [`calen.js`](TaskManagementProject/app/static/js/calen.js) reads the json file of the events that a user has into     the calendar. 

- [`app.static`](TaskManagementProject/app/static)

- [`app.templates`](TaskManagementProject/app/templates)
