<div align="center">

# 🤖 EchoMind
### AI-Powered Customer Care Assistant

<img src="https://img.shields.io/badge/React-19-blue?logo=react" />
<img src="https://img.shields.io/badge/Vite-Frontend-646CFF?logo=vite" />
<img src="https://img.shields.io/badge/Node.js-Express-339933?logo=node.js" />
<img src="https://img.shields.io/badge/FastAPI-Python-009688?logo=fastapi" />
<img src="https://img.shields.io/badge/PostgreSQL-Database-336791?logo=postgresql" />
<img src="https://img.shields.io/badge/Prisma-ORM-2D3748?logo=prisma" />
<img src="https://img.shields.io/badge/PyTorch-AI-EE4C2C?logo=pytorch" />

**An intelligent AI-powered customer care platform built using a scalable Microservice Architecture.**

</div>

---

# ✨ Features

- 🤖 AI-powered Intent Prediction
- 🎙️ Voice & Emotion Analysis
- 🧠 Semantic Memory Search
- 📈 Continuous Learning (Hindsight Training)
- 💬 Customer Conversation Logging
- 📊 Analytics & Performance Metrics
- ⚡ FastAPI + PyTorch ML Engine
- 🌐 React + Vite Frontend
- 🗄️ PostgreSQL Database
- 🔄 Node.js API Gateway

---

# 🏗️ System Architecture

```text
                        +----------------------+
                        |    React Frontend    |
                        |     (Vite + React)   |
                        +----------+-----------+
                                   |
                                   |
                        HTTP Requests
                                   |
                    +--------------v--------------+
                    |     Node.js API Gateway     |
                    |   Express + Prisma ORM      |
                    +-------+------------+---------+
                            |            |
                 PostgreSQL |            | HTTP
                            |            |
              +-------------v--+    +----v----------------+
              |   PostgreSQL   |    |   Python ML Service |
              |   Database     |    | FastAPI + PyTorch   |
              +----------------+    +---------------------+
```

---

# 📂 Project Structure

```text
EchoMind/
│
├── frontend/          # React + Vite UI
│
├── node_backend/      # Express API Gateway
│   ├── Prisma
│   ├── Controllers
│   ├── Routes
│   └── PostgreSQL
│
├── ml_service/        # FastAPI + PyTorch
│   ├── NLP Models
│   ├── Emotion Detection
│   ├── Vector Search
│   └── AI Training
│
└── README.md
```

---

# 🚀 Getting Started

Run all **three services simultaneously** using separate terminals.

---

## 1️⃣ Backend Gateway (Node.js)

Responsible for:

- Database operations
- Authentication
- API Gateway
- Communication with ML Service

```bash
cd node_backend

npm install
```

Configure your `.env`

```env
DATABASE_URL="postgresql://user:password@localhost:5432/dbname?schema=public"
```

Push database schema

```bash
npx prisma db push
```

Run server

```bash
npm run dev
```

Runs on:

```
http://localhost:3000
```

---

## 2️⃣ AI ML Service

The intelligence behind EchoMind.

Features:

- Intent Prediction
- Emotion Detection
- Vector Search
- Model Retraining

```bash
cd ml_service

python -m venv venv
```

Activate environment

Windows

```bash
venv\Scripts\activate
```

Linux / macOS

```bash
source venv/bin/activate
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run server

```bash
python app.py
```

Runs on:

```
http://localhost:8000
```

---

## 3️⃣ Frontend

```bash
cd frontend

npm install

npm run dev
```

Runs on:

```
http://localhost:5173
```

---

# 🔗 API Endpoints

| Method | Endpoint | Service | Description |
|----------|-----------------------------|----------------|--------------------------------|
| GET | `/health` | Node + Python | Check application health |
| POST | `/api/predict` | Python | Intent prediction |
| POST | `/api/voice/analyze` | Python | Voice emotion analysis |
| POST | `/api/memory/search` | Python | Semantic memory retrieval |
| POST | `/api/hindsight/train` | Python | Retrain AI model |
| POST | `/api/hindsight/feedback` | Node.js | Save user feedback |
| GET | `/api/hindsight/logs` | Node.js | Retrieve conversation history |
| GET | `/api/metrics` | Node + Python | AI & Database metrics |

---

# 🛠️ Tech Stack

## Frontend

- React
- Vite
- JavaScript
- CSS

## Backend

- Node.js
- Express.js
- Prisma ORM
- PostgreSQL

## AI Service

- Python
- FastAPI
- PyTorch
- NumPy
- Scikit-learn

---

# ⚙️ Default Ports

| Service | Port |
|----------|------|
| Frontend | **5173** |
| Node API Gateway | **3000** |
| Python ML Service | **8000** |
| PostgreSQL | **5432** |

---

# 🌟 Microservice Flow

```text
User
 │
 ▼
React Frontend
 │
 ▼
Node.js API Gateway
 │
 ├────────────► PostgreSQL
 │
 ▼
FastAPI ML Service
 │
 ▼
PyTorch Models
 │
 ▼
Prediction Response
 │
 ▼
React Frontend
```

---

# 💡 Future Enhancements

- 🔐 JWT Authentication
- 🌍 Multi-language Support
- 📞 Real-time Voice Calls
- 📈 AI Dashboard
- ☁️ Docker Deployment
- ☸️ Kubernetes Support
- 🤖 LLM Integration
- 📡 WebSocket Streaming

---

<div align="center">

## ⭐ If you like this project, don't forget to star the repository!

**Made with ❤️ using React, Node.js, FastAPI, PostgreSQL & PyTorch**

</div>