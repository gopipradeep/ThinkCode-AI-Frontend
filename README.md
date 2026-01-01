# ThinkCode AI

A modern, collaborative code editor with real-time execution, AI-powered code analysis, and multi-user collaboration features.

## 🚀 Live Demo

**[https://think-code-ai-frontend.vercel.app/](https://think-code-ai-frontend.vercel.app/)**

## ✨ Features

### 🎯 Core Functionality
- **Multi-Language Support**: Execute code in 9+ programming languages (Python, Java, C++, C, C#, JavaScript, Go, Ruby, PHP)
- **Real-Time Code Execution**: Run code with live terminal output and interactive input handling
- **Monaco Editor Integration**: Professional code editing experience with syntax highlighting
- **Dark/Light Theme**: Toggle between beautiful dark and light themes

### 🤖 AI-Powered Features
- **Code Analysis**: Get detailed insights about your code structure, complexity, and potential improvements
- **Code Explanation**: Contextual explanations that understand both your code and execution results
- **Powered by Gemini AI**: Intelligent analysis with real-time processing

### 👥 Collaboration Features
- **Live Collaboration Sessions**: Share coding sessions with multiple users in real-time
- **Real-Time Chat**: Communicate with collaborators while coding
- **Code Synchronization**: Changes are instantly synced across all connected users
- **Session Sharing**: Generate shareable links for instant collaboration

### 💾 Persistence & Storage
- **Recent Code Auto-Save**: Your last successful execution is automatically saved
- **Firebase Integration**: Secure cloud storage for code persistence
- **User Authentication**: Google Sign-In and Guest mode support

## 🛠️ Tech Stack

### Frontend
- **React 19.1.1** - Modern UI framework
- **Monaco Editor** - VS Code's editor component
- **Firebase** - Authentication and Firestore database
- **WebSocket** - Real-time bidirectional communication
- **DOMPurify** - XSS protection for rendered content

### Backend (Not in this repo)
- WebSocket server for code execution
- Multi-language code runner
- Gemini AI integration for code analysis

## 📦 Installation
```bash
# Clone the repository
git clone https://github.com/yourusername/thinkcode-ai.git

# Navigate to project directory
cd thinkcode-ai

# Install dependencies
npm install

# Start development server
npm start
```

The app will open at `http://localhost:3000`

## 🔧 Configuration

### Firebase Setup
Update `src/firebase.js` with your Firebase configuration:
```javascript
const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_AUTH_DOMAIN",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_STORAGE_BUCKET",
  messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
  appId: "YOUR_APP_ID",
  measurementId: "YOUR_MEASUREMENT_ID"
};
```

### Backend Configuration
The app connects to the backend WebSocket server. Update URLs in `src/ThinkCodeAI.js` if needed:
```javascript
const BACKEND_BASE_URL = 'https://your-backend-url.com';
const WS_URL = 'wss://your-backend-url.com/execute-ws';
```

## 📱 Usage

### Running Code
1. Select your programming language from the dropdown
2. Write or paste your code in the editor
3. Click **Run Code** to execute
4. View output in the Terminal tab
5. Provide input when prompted (for interactive programs)

### AI Features
- **Analyze**: Click to get code quality insights, complexity analysis, and improvement suggestions
- **Explain**: Get detailed explanations of your code's functionality and logic flow

### Collaboration
1. Click the **Account Icon** → **Start Collab Session**
2. Share the generated link with collaborators
3. Code changes sync automatically
4. Use the live chat to communicate
5. Click **Apply Changes** to broadcast your updates

### Saving Code
- Code is automatically saved after successful execution
- Click **Account Icon** → **Recent Code** to load your last saved work

## 🎨 Supported Languages

| Language | Version | Interactive Input |
|----------|---------|-------------------|
| Python | 3.x | ✅ |
| Java | 11+ | ✅ |
| C++ | GCC/G++ | ✅ |
| C | GCC | ✅ |
| C# | .NET Core | ✅ |
| JavaScript | Node.js | ✅ |
| Go | 1.x | ✅ |
| Ruby | 2.x+ | ✅ |
| PHP | 7.x+ | ✅ |

## 🏗️ Project Structure
```
src/
├── App.js                 # Main app component with routing
├── ThinkCodeAI.js        # Primary code editor interface
├── CollabSession.js      # Collaboration session component
├── LoginPage.js          # Authentication UI
├── firebase.js           # Firebase configuration
├── ErrorBoundary.js      # Error handling component
└── index.js              # App entry point
```




## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- Monaco Editor by Microsoft
- Firebase by Google
- Gemini AI by Google
- React community

