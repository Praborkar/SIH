🚆 SIH Railway Navigation System – Backend

Backend for a Smart India Hackathon project focused on mapping and navigating railway-station facilities in real time.

📌 Project Overview

This backend powers a railway-station navigation system designed to help passengers quickly locate station facilities such as:

Toilets & Restrooms

Food Counters & Shops

Platforms

Waiting Areas

Entry & Exit Gates

Other Station Services

The goal was to build an API-driven backend that allows the frontend to fetch facility locations, station details, and navigation-relevant data.

This project was developed during the Smart India Hackathon (SIH) under a strict 8-hour development window, as part of an on-spot problem statement.

🛠️ Tech Stack

Node.js

Express.js

TypeScript

🚀 Features

✔ Modular Node.js + TypeScript backend
✔ API endpoints for station facilities
✔ Geo-location & category-based filtering
✔ Validation middleware
✔ Scalable folder structure
✔ Ready for frontend integration

📡 API Endpoints (Sample)
GET /stations/:id/facilities

Returns all facilities (toilets, food, platforms, exits, etc.) for a given station.

GET /stations/:id/facilities/:type

Filter facilities by category.

POST /stations/:id/facilities

Add a new facility (admin use).

⚠️ Hackathon Context

This backend was developed during SIH with an 8-hour coding window.
Due to time limitations:

Backend was not fully completed

Full frontend integration was not possible

However, the architecture, base models, and API structure were completed and functional

Despite the constraints, the project demonstrates the core backend architecture and the approach taken under time pressure.

📎 GitHub Repository

👉 https://github.com/Praborkar/SIH

👨‍💻 Contributors

Prabor Kar – Backend (Node.js/TypeScript)

.
.
.
.

📝 License

This project is for educational and hackathon purposes only.
MongoDB (or your DB used)

REST API Architecture
