# 🎬 OMDB Movie Explorer

OMDB Movie Explorer is a full-stack movie and series discovery application powered by the **OMDB API**.  
It includes a custom backend service and a responsive frontend UI for searching, browsing, and viewing detailed movie information.

---

## 🚀 Project Overview

This project contains **two main components**:

---

## 1️⃣ Backend Web Service

- Fetches data from the OMDB API  
- Implements **response caching** (Redis or In-Memory)  
- Supports cache expiry & max size  
- Follows **REST API best practices**  
- Runs locally  
- Secure OMDB API key handling using environment variables  

---

## 2️⃣ Frontend UI Layer

- 🔎 Search movies/series by title  
- 🖼️ Results grid with posters, titles and release years  
- 📘 Detailed info view (Plot, Director, Actors, Ratings)  
- ⭐ Favorites system (optional)  
- 📱 Fully responsive for mobile and desktop  

---

## 📁 Folder Structure

```
omdb-movie-explorer/
│
├── backend/
│   ├── src/
│   ├── controllers/
│   ├── routes/
│   ├── cache/
│   ├── package.json
│   └── ...
│
├── frontend/
│   ├── src/
│   ├── public/
│   ├── components/
│   ├── package.json
│   └── ...
│
└── README.md
```

---

## 🔗 API Endpoints (Example)

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/search?query=title` | Search for movies or series |
| GET | `/api/details?id=imdbID` | Get detailed movie info |
| POST | `/api/favorites` | Add a movie to favorites (optional) |
| DELETE | `/api/favorites/:id` | Remove from favorites |

---

## 🛠️ How to Run Locally

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/omdb-movie-explorer.git
cd omdb-movie-explorer
```

---

### 2️⃣ Backend Setup

Create a `.env` file:
```
OMDB_API_KEY=your_api_key_here
```

Install backend dependencies:
```bash
cd backend
npm install
```

Run backend:
```bash
npm start
```

Backend runs on **http://localhost:5000**

---

### 3️⃣ Frontend Setup

Install frontend dependencies:
```bash
cd frontend
npm install
```

Run frontend:
```bash
npm start
```

Frontend runs on **http://localhost:3000**

---

## 🧠 Evaluation Criteria

- Code quality  
- REST API structure  
- UI/UX  
- Caching performance  
- Extensibility & modularity  

---

## 🌟 Future Enhancements

- Dark mode  
- Genre-based filtering  
- Infinite scrolling  
- Offline support  
- Local storage favorites  

---

## 📜 License

This project is licensed under the **MIT License**.

---

## 🙌 Author

Developed as part of a full-stack engineering assignment using the public OMDB API.

