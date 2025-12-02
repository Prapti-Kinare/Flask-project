# Fertilizer & Pesticide Stock Management System

· A secure Flask-based web app for managing fertilizer and pesticide inventory  
· Multi-user support with authentication and session management  
· Automated stock alerts for low inventory and expiring products  

## Features
· User authentication with secure registration and login  
· Product management (add, view, update, delete) including:  
  · Product name, type, and category  
  · Quantity and unit of measurement  
  · Manufacturing and expiry dates  
  · Price, supplier, batch number, storage location  
· Automated alerts triggered by database for:  
  · Low stock levels (< 50 units)  
  · Products expiring within 30 days  
· Data validation preventing:  
  · Negative quantities and prices  
  · Adding expired products  
· Activity logging for product changes  
· Search functionality by product name, category, or supplier  
· User data isolation to ensure privacy  

## Tech Stack
· Flask (Python)  
· SQLite with triggers for automation  
· Werkzeug for password hashing  
· HTML templates (Bootstrap assumed)  

## Setup Instructions
· Clone the repo to your local machine  
· Install dependencies with: `pip install flask werkzeug`  
· Update the secret key in `app.py` for security  
· Run the app: `python app.py`  
· Access via `http://127.0.0.1:5000` and register a user  

## Usage
· Register/login to manage your inventory  
· Add and update fertilizer/pesticide products  
· View alerts for stock and expiry management  
· Search through your products quickly  

## Project Structure
· `app.py` - Main Flask application  
· `templates/` - HTML pages  
· `static/` - Static assets like CSS/JS  
· `fertilizerstock.db` - SQLite database (auto-created)  

## Notes
· Change the secret key before production use  
· Routes are protected by login-required decorator  
· Database triggers handle alerts and validations  

## Future Improvements
· Interactive dashboards for stock visualization  
· Export reports as CSV or PDF  
· Role-based access control  
· Email alerts for stock warnings  
