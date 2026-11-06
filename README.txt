========================================================================
ROOMFINDER MAHARASHTRA - STUDENT PROJECT (HTML, CSS, JAVASCRIPT)
University Final Year Project by Abhirathod
========================================================================

FILES INCLUDED IN THIS ZIP:
1. index.html   --> Complete frontend layout, modals, search, and navbar
2. style.css    --> Clean, responsive CSS styling (identical to live app)
3. script.js    --> App logic, filtering, modals, and backend API integration
4. backend_sample.py (Optional) --> Ready-to-run Python Flask backend example

------------------------------------------------------------------------
HOW TO RUN THE PROJECT:
------------------------------------------------------------------------
Option A: DIRECT BROWSER RUN (No server needed)
Simply double-click "index.html" in any browser (Chrome, Edge, Firefox).
Everything works instantly with offline demonstration data!

Option B: WITH LIVE SERVER OR VS CODE
1. Open this folder in Visual Studio Code.
2. Right click "index.html" and select "Open with Live Server".

------------------------------------------------------------------------
HOW TO CONNECT YOUR BACKEND:
------------------------------------------------------------------------
In "script.js", at lines 15-25:

const CONFIG = {
  API_BASE_URL: 'http://localhost:5000/api', // <-- Change to your backend URL
  USE_BACKEND: true,                          // <-- Set to true
};

Endpoints expected by the frontend:
- GET  /api/properties   --> Returns JSON array of property objects
- POST /api/properties   --> Adds a new property listing
- POST /api/visits       --> Records a scheduled room visit
- GET  /api/visits       --> Retrieves visit bookings

*Note: If your backend is offline, the app automatically falls back to 
pre-loaded demonstration data so your university viva/exam never fails!
