# 🚆 Railway Station Navigation System – Backend
Backend for the **Smart India Hackathon (SIH)** project focused on providing real-time navigation for railway-station facilities. Built using **Node.js + TypeScript** within an intense **8-hour development sprint** during the hackathon.

## 📌 Overview
This backend powers a digital navigation system designed for railway stations.  
The goal is to help passengers **quickly locate essential facilities** inside a station such as:

- Toilets & Restrooms  
- Food Counters  
- Waiting Areas  
- Platforms  
- Ticket Counters  
- Entry & Exit Gates  
- Other Points of Interest (POIs)

The backend exposes REST APIs that allow the frontend to fetch station data, facility locations, and categories in a structured, scalable manner.

Although the system was not fully completed or integrated due to the time constraints of SIH, the backend architecture, core modules, and main APIs were built with production-style standards.

## 🎯 SIH Hackathon Context
This project was developed as part of **Smart India Hackathon (SIH)** under a strict, real-time challenge:

⏱️ **8 hours of continuous coding**  
🧩 Solve a real problem statement  
🤝 Collaborate with a team  
⚙️ Build a working prototype backend + frontend  

Despite the limited time, the backend was built with clean architecture, modular structure, and TypeScript-based type safety.

## 🛠️ Tech Stack
- **Node.js**
- **Express.js**
- **TypeScript**
- **MongoDB / JSON mock data**
- **REST API Architecture**

## 📂 Folder Structure
```
.
├── src/
│   ├── controllers/      # Request handlers
│   ├── routes/           # API route definitions
│   ├── services/         # Business logic
│   ├── models/           # Data models / schemas
│   ├── middleware/       # Validation, error handling, auth
│   ├── config/           # DB, environment configs
│   └── utils/            # Helpers & utilities
├── package.json
├── tsconfig.json
├── README.md
└── .env (ignored)
```

## 🚀 Key Features
✔ Modular Node.js + TypeScript architecture  
✔ API endpoints for facility listings  
✔ Station-wise and category-wise facility filtering  
✔ Scalable folder layout for future development  
✔ Validation middleware for clean data flow  
✔ Lightweight and easy to extend  
✔ Ready for real-time navigation integration  

## 📡 API Endpoints

### GET /stations
Returns list of available stations.

### GET /stations/:stationId
Returns metadata for a specific station.

### GET /stations/:stationId/facilities
Fetch all facilities of a station.

### GET /stations/:stationId/facilities/:type
Fetch facilities filtered by type (toilet, food, platform, exit, etc.)

### POST /stations/:stationId/facilities
Admin-level action to add POIs.

## 🗄️ Sample Facility Schema
```
{
  id: string;
  name: string;
  type: 'toilet' | 'food' | 'platform' | 'exit' | 'waiting' | 'other';
  location: {
    lat: number;
    lng: number;
    floor: number;
  };
  description?: string;
}
```

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository  
```
git clone https://github.com/Praborkar/SIH
cd SIH
```

### 2️⃣ Install Dependencies  
```
npm install
```

### 3️⃣ Create Environment File  
Create `.env`:

```
PORT=5000
MONGO_URI=your_mongodb_url
```

### 4️⃣ Run in Development Mode  
```
npm run dev
```

### 5️⃣ Build & Run  
```
npm run build
npm start
```

## 📈 What’s Completed
- Backend structure  
- Core routes & controllers  
- Facility models  
- Base database design  
- Basic API communication attempt  
- Modular code layout  

## ❗What’s Pending
- Full frontend integration  
- Navigation algorithms  
- Admin dashboard  
- Authentication system  
- Database indexing

## 📎 GitHub Repository
https://github.com/Praborkar/SIH

## 👨‍💻 Contributors
- **Prabor Kar** – Backend (Node.js + TypeScript)

## 📄 License
This project is for educational and hackathon purposes only.
