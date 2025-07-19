# SkyGrid 

SkyGrid is a community-driven web platform designed to support the FPV (First Person View) drone community by helping users discover and share FPV flying spots, stores, and club racing locations through an interactive map interface.

---

##  Features

- **Interactive Map** with filterable layers for:
  - FPV Flying Spots
  - Drone Stores
  - FPV Racing Clubs
-  **User Authentication** with secure login/registration
-  **Location Submissions** with moderation workflow
-  **Admin & Moderator Tools** for approving or rejecting locations
-  **Search and Sort** features for finding places easily
-  Built using **Flask**, **SQLite**, **HTML/CSS**, and **JavaScript**

---

##  Installation Instructions

**Prerequisites:**
- Python 3.11 or later
- Git installed
- (Recommended) A virtual environment

**Step-by-step Setup:**

1. Clone the repository:

   `git clone https://github.com/natebecks/SKYGRID.git`

   `cd SKYGRID`

2. (Optional) Create and activate a virtual environment:

   - On macOS/Linux:

     `python -m venv .venv`

     `source .venv/bin/activate`

   - On Windows:

     `python -m venv .venv`

     `.venv\Scripts\activate`

3. Install all required dependencies:

   `pip install -r requirements.txt`

4. Launch the application:

   `python app.py`

5. Open your browser and go to:

   `http://127.0.0.1:5000`

---

##  How to Use

- Register or log in to access full features.
- Use the map to explore FPV flying spots, clubs, and stores.
- Submit your own locations via the “Add Location” form.
- A moderator will review your submission before it appears on the map.
- Moderator users can log in and access the `/moderator` dashboard.

---

## License Information

MIT License

You are free to use, modify, and distribute this software, provided you include the original license.

---

##  Acknowledgements

- Flask (Python web framework)
- Leaflet.js (for interactive maps)
- Google Maps API (for interactive maps)
- OpenWeather API (for live weather)
- SQLite (database)
- ChatGPT (debugging and code review)
- Teachers, classmates, and online forums for development support

---

##  Author Details

**Name:** Nate B  
**Email:** blueyabby28@gmail.com
**GitHub:** https://github.com/natebecks  
**Project Type:** HSC Major Design Project (Software Engineering)

---

## Directory Structure

<pre>

SKYGRID/
├── __pycache__/
├── .venv/
├── instance/
│   └── skygrid.db
├── static/
│   ├── icons/
│   ├── favicon.png
│   └── layout.css
├── templates/
│   ├── additions.html
│   ├── club_details.html
│   ├── index.html
│   ├── list.html
│   ├── login.html
│   ├── map.html
│   ├── moderator_additions.html
│   ├── moderator_requests.html
│   ├── moderator_support.html
│   ├── moderator.html
│   ├── spot_details.html
│   ├── store_details.html
│   └── support.html
├── .gitignore
├── app.py
├── createmapdb.py
├── createmoddb.py
├── createuserdatabase.py
├── mapbase.db
├── models.py
├── moderatorbase.db
├── SKYGRID.code-workspace
└── userbase.db

  ---

## Additional Details

- Submissions are validated before database insertion.
- Role-based access control ensures that only moderators access approvals.
- Flash messages are used for user feedback (success, error).
- Flask sessions store login state securely.
- You must change the Flask secret key from `"123"` in production.
- The project was created with scalability and future deployment in mind.
- APP IS NOT SECURE DO NOT PUT IMPORTANT INFORMATION IN

