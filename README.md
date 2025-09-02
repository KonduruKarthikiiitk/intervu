# Intervu.Prep 🚀

A comprehensive AI-powered interview preparation platform that generates personalized interview questions and provides detailed concept explanations using Google's Gemini AI.

## ✨ Features

- 🤖 **AI-Powered Question Generation**: Generate interview questions based on role, experience level, and focus topics
- 📚 **Concept Explanations**: Get detailed explanations for any interview question with AI assistance
- 📌 **Smart Question Management**: Pin important questions, add notes, and organize your study material
- 🎨 **Modern UI/UX**: Beautiful, responsive design with smooth animations
- 🔐 **User Authentication**: Secure login and registration with JWT
- 📱 **Mobile Responsive**: Perfect experience on all devices
- ⚡ **Real-time Updates**: Instant feedback and loading states
- 📸 **Profile Management**: Upload and manage profile images

## 🛠️ Tech Stack

### Frontend

- **React 18** - Modern React with hooks
- **Vite** - Fast build tool and dev server
- **Tailwind CSS** - Utility-first CSS framework
- **Framer Motion** - Smooth animations
- **React Router** - Client-side routing
- **Axios** - HTTP client
- **React Hot Toast** - Beautiful notifications

### Backend

- **Node.js** - JavaScript runtime
- **Express.js** - Web framework
- **MongoDB** - NoSQL database
- **Mongoose** - MongoDB ODM
- **JWT** - Authentication
- **Multer** - File uploads
- **Google Gemini AI** - AI question generation

## 🚀 Quick Start

### Prerequisites

- Node.js (v16 or higher)
- MongoDB (local or cloud)
- Google Gemini API key

### 1. Clone the Repository

```bash
git clone <repository-url>
cd INTERVIEW_PREPAI
```

### 2. Backend Setup

```bash
cd backend

# Install dependencies
npm install

# Create environment file
cp .env.example .env
# Edit .env with your configuration

# Start the server
npm start
```

### 3. Frontend Setup

```bash
cd frontend/interview-prep-ai

# Install dependencies
npm install

# Create environment file
echo "VITE_API_BASE_URL=http://localhost:8000" > .env

# Start development server
npm run dev
```

### 4. Environment Configuration

#### Backend (.env)

```env
MONGO_URI=mongodb://localhost:27017/interview-prep-ai
JWT_SECRET=your-super-secret-jwt-key
GEMINI_API_KEY=your-gemini-api-key
PORT=8000
```

#### Frontend (.env)

```env
VITE_API_BASE_URL=http://localhost:8000
```

## 📁 Project Structure

```
INTERVU/
├── backend/                 # Node.js/Express backend
│   ├── config/             # Database and environment config
│   ├── controllers/        # Route controllers
│   ├── middlewares/        # Custom middlewares
│   ├── models/             # MongoDB models
│   ├── routes/             # API routes
│   ├── uploads/            # File uploads
│   └── utils/              # Utility functions
└── frontend/
    └── interview-prep-ai/  # React frontend
        ├── src/
        │   ├── components/ # Reusable components
        │   ├── Pages/      # Page components
        │   ├── context/    # React context
        │   └── utils/      # Frontend utilities
        └── public/         # Static assets
```

## 🔧 API Endpoints

### Authentication

- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - User login
- `GET /api/auth/profile` - Get user profile
- `POST /api/auth/upload-image` - Upload profile image

### Sessions

- `POST /api/sessions/create` - Create interview session
- `GET /api/sessions/my-sessions` - Get user sessions
- `GET /api/sessions/:id` - Get session by ID
- `DELETE /api/sessions/:id` - Delete session

### Questions

- `POST /api/questions/add` - Add questions to session
- `PUT /api/questions/:id/pin` - Toggle pin status
- `PUT /api/questions/:id/note` - Update question note

### AI

- `POST /api/ai/generate-questions` - Generate interview questions
- `POST /api/ai/generate-explanation` - Generate concept explanation

## 🎯 Key Features Explained

### AI Question Generation

The platform uses Google's Gemini AI to generate personalized interview questions based on:

- **Role**: The position you're applying for
- **Experience Level**: Your years of experience
- **Focus Topics**: Specific areas you want to focus on
- **Question Count**: Number of questions to generate

### Concept Explanations

Get detailed explanations for any interview question:

- **Beginner-friendly explanations**
- **Code examples when relevant**
- **Real-world applications**
- **Best practices and tips**

### Question Management

- **Pin Important Questions**: Mark questions for quick access
- **Add Personal Notes**: Add your own insights and notes
- **Organize by Topics**: Questions are organized by focus areas
- **Track Progress**: Monitor your interview preparation progress

## 🎨 UI/UX Features

### Modern Design

- **Clean and Minimal**: Focus on content, not distractions
- **Consistent Color Scheme**: Professional and accessible
- **Smooth Animations**: Enhanced user experience
- **Responsive Layout**: Works on all screen sizes

### Interactive Elements

- **Hover Effects**: Visual feedback on interactions
- **Loading States**: Clear indication of ongoing processes
- **Toast Notifications**: Success and error feedback
- **Expandable Sections**: Show/hide detailed information

## 🔒 Security Features

- **JWT Authentication**: Secure token-based authentication
- **Password Hashing**: Bcrypt for password security
- **Input Validation**: Server-side validation
- **CORS Configuration**: Proper cross-origin settings
- **File Upload Security**: Secure file handling

## 🚀 Deployment

### Backend Deployment

1. Set up MongoDB (MongoDB Atlas recommended)
2. Configure environment variables
3. Deploy to platforms like:
   - Heroku
   - Railway
   - DigitalOcean
   - AWS

### Frontend Deployment

1. Build the project: `npm run build`
2. Deploy to platforms like:
   - Vercel
   - Netlify
   - GitHub Pages
   - AWS S3

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Google Gemini AI** for providing the AI capabilities
- **Tailwind CSS** for the beautiful styling framework
- **React Community** for the amazing ecosystem
- **Open Source Contributors** for various libraries used

## 📞 Support

If you have any questions or need help:

- Create an issue in the repository
- Contact the development team
- Check the documentation

---

**Happy Interview Preparation! 🎉**
