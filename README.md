# 📝 Online Notes App

A modern, full-stack web application for creating, managing, and organizing your notes with a clean and intuitive interface.

![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-404D59?style=for-the-badge)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

## ✨ Features

- **📝 Create Notes**: Add new notes with title and content
- **🗑️ Delete Notes**: Remove unwanted notes with one click
- **📱 Responsive Design**: Works seamlessly on desktop and mobile devices
- **⚡ Real-time Updates**: Changes reflect immediately without page refresh
- **🎨 Clean UI**: Modern and intuitive user interface
- **🔒 RESTful API**: Well-structured backend API for data management

## 🏗️ Architecture

This project follows a **client-server architecture** with:

- **Frontend**: Vanilla HTML, CSS, and JavaScript
- **Backend**: Node.js with Express.js framework
- **Database**: MongoDB with Mongoose ODM
- **API**: RESTful endpoints for CRUD operations

## 📁 Project Structure

```
Online-Notes-App/
├── backend/
│   ├── config/
│   │   └── db.js
│   ├── models/
│   │   ├── Note.js
│   │   └── User.js
│   ├── routes/
│   │   ├── auth.js
│   │   └── notes.js
│   ├── package.json
│   └── server.js
├── frontend/
│   ├── index.html
│   ├── script.js
│   └── style.css
├── package.json
└── README.md
```

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v14 or higher)
- [MongoDB](https://www.mongodb.com/) (local installation or MongoDB Atlas)
- [Git](https://git-scm.com/)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/Online-Notes-App.git
   cd Online-Notes-App
   ```

2. **Install backend dependencies**
   ```bash
   cd backend
   npm install
   ```

3. **Set up environment variables**
   Create a `.env` file in the `backend` directory:
   ```env
   MONGO_URI=mongodb://localhost:27017/notes-app
   PORT=5000
   JWT_SECRET=your-secret-key
   ```

4. **Start the backend server**
   ```bash
   npm start
   ```
   The server will run on `http://localhost:5000`

5. **Open the frontend**
   - Navigate to the `frontend` directory
   - Open `index.html` in your web browser
   - Or serve it using a local server:
     ```bash
     # Using Python
     python -m http.server 8000
     
     # Using Node.js (if you have http-server installed)
     npx http-server -p 8000
     ```

## 🔧 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| `GET` | `/` | Health check endpoint |
| `GET` | `/notes` | Get all notes |
| `POST` | `/notes` | Create a new note |
| `PUT` | `/notes/:id` | Update a note |
| `DELETE` | `/notes/:id` | Delete a note |

### Example API Usage

```javascript
// Create a note
const response = await fetch('http://localhost:5000/notes', {
  method: 'POST',
  headers: { 'Content-Type': 'application/json' },
  body: JSON.stringify({
    title: 'My Note',
    content: 'This is the content of my note'
  })
});

// Get all notes
const notes = await fetch('http://localhost:5000/notes').then(res => res.json());
```

## 🛠️ Technologies Used

### Backend
- **Node.js** - JavaScript runtime
- **Express.js** - Web application framework
- **MongoDB** - NoSQL database
- **Mongoose** - MongoDB object modeling
- **bcryptjs** - Password hashing
- **jsonwebtoken** - JWT authentication
- **cors** - Cross-origin resource sharing
- **dotenv** - Environment variables

### Frontend
- **HTML5** - Markup language
- **CSS3** - Styling
- **Vanilla JavaScript** - Client-side functionality

## 🎨 Features in Detail

### Note Management
- **Create**: Add new notes with title and content
- **Read**: View all notes in a clean, organized layout
- **Update**: Edit existing notes (API ready, UI implementation pending)
- **Delete**: Remove notes with confirmation

### User Experience
- **Responsive Design**: Adapts to different screen sizes
- **Real-time Updates**: Changes appear immediately
- **Error Handling**: Graceful error management
- **Loading States**: Visual feedback for operations

## 🔮 Future Enhancements

- [ ] User authentication and authorization
- [ ] Note categories and tags
- [ ] Search and filter functionality
- [ ] Rich text editor
- [ ] Note sharing capabilities
- [ ] Dark/Light theme toggle
- [ ] Export notes to different formats
- [ ] Mobile app version

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request


## 👨‍💻 Author

**Ali Haseebuzzaman Siddiqui**
- GitHub: [@AliSidd458](https://github.com/AliSidd458)
- LinkedIn: [Ali Haseebuzzaman Siddiqui](https://www.linkedin.com/in/ali-haseebuzzaman-siddiqui-941b7620a/)



⭐ **Star this repository if you found it helpful!**
