# Flight_Finder_MERN_Project

Flight Finder: Navigating Your Air Travel Options
Flight Finder is a full-stack web application built using the MERN stack (MongoDB, Express, React, Node.js). It provides a high-performance, mobile-responsive platform for travelers to search for flights between cities and persistently save their booking history.

1. Project Overview
Purpose: To eliminate friction in air travel discovery by providing a fast, reliable, and user-centric booking interface.

Target User: Frequent travelers looking for an intuitive way to manage their itineraries.

Core Goal: Solving the "Slow UI" and "Data Loss" pain points found in traditional travel portals.

2. Key Features
Dynamic Search: Real-time city filtering through dynamic dropdown menus.

Persistent Bookings: A dedicated "My Bookings" dashboard that saves data to a NoSQL database.

Mobile-First Design: Fully responsive UI built with Bootstrap for use on any device.

Admin Seeding: Specialized routes to automatically populate the system with fresh flight data.

3. Technology Stack
Frontend: React.js (Functional Components, Hooks)

Backend: Node.js & Express.js (RESTful API)

Database: MongoDB (Mongoose ODM)

Styling: Bootstrap & CSS3

Deployment: Render / Vercel

4. System Architecture
The application follows a 3-Tier Architecture:

Presentation Layer: React handles the UI and user interactions.

Application Layer: Node/Express manages business logic and API routing.

Data Layer: MongoDB Atlas stores persistent user and flight records.

5. Setup & Installation
Prerequisites
Node.js (v16 or higher)

npm or yarn

MongoDB Atlas Account

Steps
Clone the Repository:

Bash
git clone https://github.com/your-username/flight-finder.git
cd flight-finder
Install Backend Dependencies:

Bash
cd server
npm install
Install Frontend Dependencies:

Bash
cd ../client
npm install
Environment Variables:
Create a .env file in the /server directory and add:

Code snippet
MONGODB_URI=your_mongodb_connection_string
PORT=5000
Run the Application:

Start Server: cd server && npm start

Start Client: cd client && npm start

6. API Endpoints
Method	Endpoint	Description
GET	/api/flights	Fetch all available flights based on city search.
POST	/api/book	Save a flight selection to the user's dashboard.
GET	/api/seed	Admin route to reset and populate flight data.
7. Folder Structure
Plaintext
flight-finder/
├── client/              # React Frontend
│   ├── public/
│   └── src/
│       ├── components/  # Reusable UI elements
│       └── pages/       # Search and Dashboard views
└── server/              # Node.js Backend
    ├── models/          # Mongoose Schemas
    ├── routes/          # API Route definitions
    └── server.js        # Main entry point
8. Testing & QA
Unit Testing: Verified REST API endpoints via Postman.

Functional Testing: 100% pass rate on core search and booking logic.

UAT: Conducted user acceptance testing based on the project Empathy Map.

9. Future Enhancements
Real-time Integration: Connecting to live Aviation APIs (e.g., Amadeus).

Secure Auth: Implementing JWT (JSON Web Tokens) for user logins.

Payments: Integration with Stripe for financial transactions.
