🧠 BrainBin

BrainBin is a full-stack note-taking web application designed to help users create, manage, and organize personal notes efficiently.
It focuses on clean UI, fast interactions, and a simple but scalable backend architecture.

## 🌐 Live Demo

Try the application here:
👉 https://brainbin.onrender.com


✨ Features

📝 Create, edit, and delete notes

📂 Organize personal notes in one place

⚡ Fast and responsive user interface

🔒 Secure backend with database integration

🌐 RESTful API architecture

🚦 Rate limiting for API protection

🛠 Tech Stack
Frontend

React

React Router

Axios

Lucide Icons

React Hot Toast

Backend

Node.js

Express.js

MongoDB (Mongoose)

Upstash Redis (rate limiting)

Docker (backend containerization)

dotenv

CORS

📁 Project Structure
BrainBin/
├── frontend/        # React frontend
│   ├── src/
│   ├── public/
│   └── package.json
│
├── backend/         # Express backend
│   ├── models/
│   ├── routes/
│   ├── controllers/
│   ├── config/
│   └── package.json
│
├── .gitignore
└── package.json

⚙️ Installation & Setup
1️⃣ Clone the repository
git clone https://github.com/Sarath-33/BrainBin.git
cd BrainBin

2️⃣ Backend Setup
cd backend
npm install


Create a .env file inside backend:

PORT=5001
MONGO_URI=your_mongodb_connection_string
UPSTASH_REDIS_REST_URL=your_upstash_redis_url
UPSTASH_REDIS_REST_TOKEN=your_upstash_redis_token


Start the backend server:

npm run dev

3️⃣ Frontend Setup
cd ../frontend
npm install
npm run dev


The frontend will run on:

http://localhost:5173

## 🐳 Running with Docker

The backend can also be run inside a Docker container.

### Build the image

```
docker build -t brainbin-backend ./backend
```

### Run the container

```
docker run --env-file backend/.env -p 5001:5001 brainbin-backend
```

The API will be available at:

```
http://localhost:5001
```


🔗 API Overview

RESTful API built using Express

MongoDB used for persistent note storage

Rate limiting implemented using Upstash Redis to prevent abuse

🎯 Purpose of the Project

BrainBin was built to:

Practice full-stack development

Strengthen backend fundamentals (REST APIs, MongoDB, rate limiting)

Build a real-world, scalable application

Improve frontend–backend integration

🚀 Future Improvements

User authentication (JWT)

Note categories & tags

Search and filtering

Rich text editor

Cloud deployment

👨‍💻 Author

Sarath
Aspiring Full-Stack Developer
Focused on building clean, functional, and scalable web applications.

GitHub: https://github.com/Sarath-33

Portfolio: https://withsarath.vercel.app

📄 License

This project is open-source and available under the MIT License.
