# 🤖 AI Virtual Assistant 

A full-stack **AI Voice Virtual Assistant** built using the MERN Stack and Google Gemini API.
This assistant can understand user voice/text commands and perform actions like searching Google, playing YouTube videos, telling time/date, opening apps, and answering general questions.

---

## 🚀 Features

* 🎤 Voice-enabled assistant behavior
* 🧠 Natural language understanding using Gemini AI
* 🌐 Google & YouTube search automation
* 🕒 Tell time, date, day, month
* ☁️ Cloudinary image upload support
* 🔐 JWT Authentication system
* 📦 Full MERN stack architecture

---

## 🛠️ Tech Stack

### Frontend

* React.js (Vite)
* Tailwind CSS
* Axios
* Speech Recognition API

### Backend

* Node.js
* Express.js
* MongoDB Atlas
* Mongoose
* JWT Authentication
* Cloudinary
* Google Gemini API

---

## 📂 Project Structure

```
AI-Virtual-Assistant
│
├── frontend/        # React App (UI + Voice assistant)
│
├── backend/         # Node + Express API
│   ├── controllers
│   ├── models
│   ├── routes
│   ├── middlewares
│   └── utils (Gemini Integration)
│
└── README.md
```

---

## ⚙️ Environment Variables

Create a `.env` file inside **backend** folder and add:

```
PORT=8000

MONGODB_URL=your_mongodb_connection_string

JWT_SECRET=your_secret_key

CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret

GEMINI_API_URL=https://generativelanguage.googleapis.com/v1beta/models/gemini-3-flash-preview:generateContent
GEMINI_API_KEY=your_gemini_api_key
```

⚠️ Never upload `.env` to GitHub.

---

## 💻 Installation & Setup

### 1️⃣ Clone the repository

```bash
git clone https://github.com/rajan2365/AI-Virtual-Assistant.git
cd AI-Virtual-Assistant
```

### 2️⃣ Setup Backend

```bash
cd backend
npm install
npm run dev
```

Server will run on:

```
http://localhost:8000
```

### 3️⃣ Setup Frontend

Open new terminal:

```bash
cd frontend
npm install
npm run dev
```

Frontend will run on:

```
http://localhost:5173
```

---

## 🧠 Assistant Capabilities

The assistant converts user speech/text into JSON intent:

```json
{
  "type": "google-search",
  "userInput": "MERN stack tutorial",
  "response": "Here’s what I found on Google"
}
```

### Supported Commands

| Command Type    | Action            |
| --------------- | ----------------- |
| general         | Answer questions  |
| google-search   | Search on Google  |
| youtube-search  | Search on YouTube |
| youtube-play    | Play video/song   |
| get-time        | Tell current time |
| get-date        | Tell today’s date |
| get-day         | Tell current day  |
| get-month       | Tell month        |
| calculator-open | Open calculator   |
| instagram-open  | Open Instagram    |
| facebook-open   | Open Facebook     |
| weather-show    | Show weather      |

---

## 🔐 Security Notes

* `.env` file is ignored using `.gitignore`
* API keys are never exposed in frontend
* JWT authentication implemented

---

## 📸 Future Improvements

* Add chat history
* Add multi-language support
* Deploy on Render / Vercel
* Mobile responsive UI
* Wake-word detection ("Hey Assistant")

---

## 👨‍💻 Author

**Rajan Tripathi**
MERN Stack Developer

---

## ⭐ Support

If you like this project, give it a ⭐ on GitHub 😊
