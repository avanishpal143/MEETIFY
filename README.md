# MEETIFY

# MERN Stack Video Conferencing App

## Overview
A **MERN Stack Video Conferencing App** that provides:
- **High-quality video and audio calls**
- **Secure authentication and authorization**
- **Real-time chat during video conferences**
- **Screen sharing functionality**
- **Meeting recording support**
- **User-friendly interface with a responsive design**

## Tech Stack

### Frontend:
- **React.js** - For building the user interface
- **Redux/Context API** - For state management
- **Material-UI/Tailwind CSS** - For UI styling
- **Socket.io-client** - For real-time communication
- **WebRTC** - For video and audio streaming

### Backend:
- **Node.js** - For server-side execution
- **Express.js** - For handling API routes
- **MongoDB (with Mongoose)** - For database management
- **JWT (JSON Web Token)** - For secure authentication
- **Socket.io** - For real-time communication
- **Multer** - For handling file uploads (meeting recording storage)
- **FFmpeg** - For processing and storing video recordings

### DevOps & Deployment:
- **Docker** - For containerizing the application
- **Nginx** - For reverse proxy and load balancing
- **AWS/GCP** - For hosting backend services and video storage
- **CI/CD (GitHub Actions/Jenkins)** - For automated testing and deployment

---

## Features

### 1. **User Authentication**
- Secure sign-up, login, and logout
- OAuth (Google, Facebook) authentication support

### 2. **Video Conferencing**
- High-quality video and audio
- Support for multiple participants
- Room-based meetings
- Screen sharing

### 3. **Real-time Chat**
- Text messaging in meetings
- Emojis, file sharing, and message reactions

### 4. **Meeting Recording**
- Record meetings and save them for future use
- Store recordings securely in cloud storage

### 5. **Responsive UI**
- Works seamlessly on desktop, tablet, and mobile

---

## Folder Structure

```
📦 mern-video-conferencing-app
├── 📂 backend
│   ├── 📂 config          # Configuration files (DB, auth, etc.)
│   ├── 📂 controllers     # Controllers for business logic
│   ├── 📂 middleware      # Middleware (auth, error handling, etc.)
│   ├── 📂 models          # Mongoose models (User, Meetings, etc.)
│   ├── 📂 routes          # API routes
│   ├── 📂 services        # WebRTC, recording, and real-time logic
│   ├── 📂 utils           # Utility functions
│   ├── server.js         # Express.js entry point
│   ├── package.json      # Backend dependencies
│   └── .env              # Environment variables
│
├── 📂 frontend
│   ├── 📂 public          # Static assets
│   ├── 📂 src
│   │   ├── 📂 components  # Reusable UI components
│   │   ├── 📂 pages       # React pages (Home, Dashboard, Meeting Room)
│   │   ├── 📂 store       # Redux store (if used)
│   │   ├── 📂 hooks       # Custom React hooks
│   │   ├── 📂 services    # API calls
│   │   ├── 📂 utils       # Helper functions
│   │   ├── App.js        # Main React component
│   │   ├── index.js      # React entry point
│   │   ├── styles.css    # Global styles
│   ├── package.json      # Frontend dependencies
│   └── .env              # Environment variables
│
├── 📂 tests               # End-to-end & unit testing
├── docker-compose.yml     # Docker configuration
├── README.md              # Project documentation
└── .gitignore             # Ignored files
```

---

## Installation & Setup

### 1. **Clone the Repository**
```sh
git clone https://github.com/your-username/mern-video-conferencing-app.git
cd mern-video-conferencing-app
```

### 2. **Set Up Backend**
```sh
cd backend
npm install
```
- Create a `.env` file with:
```env
MONGO_URI=<Your MongoDB URI>
JWT_SECRET=<Your JWT Secret>
SOCKET_PORT=<Port for Socket.io>
```
- Start the backend:
```sh
npm start
```

### 3. **Set Up Frontend**
```sh
cd frontend
npm install
npm start
```

---

## Testing

### **Unit Testing**
- **Backend:** Jest, Supertest
- **Frontend:** Jest, React Testing Library

Run backend tests:
```sh
cd backend
npm test
```

Run frontend tests:
```sh
cd frontend
npm test
```

### **End-to-End Testing**
- **Tool:** Cypress, Puppeteer

Start the application and run:
```sh
npm run test:e2e
```

---

## Deployment

### **Docker Deployment**
1. Build and run the container:
```sh
docker-compose up --build
```

### **Cloud Deployment (AWS/GCP)**
- **Backend:** Deploy using AWS EC2 / GCP Compute Engine
- **Frontend:** Deploy using Netlify / Vercel
- **Database:** Use MongoDB Atlas

---

## Contributing
1. Fork the repository
2. Create a feature branch (`git checkout -b feature-branch`)
3. Commit changes (`git commit -m "Added feature"`)
4. Push to the branch (`git push origin feature-branch`)
5. Open a Pull Request

---

## License
MIT License
