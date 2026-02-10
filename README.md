> A cutting-edge AI-powered voice-controlled todo application with enterprise-grade architecture and seamless user experience.

[![Version](https://img.shields.io/badge/version-2.0.0-blue.svg)](https://github.com/yourusername/ai-todo-assistant)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![React](https://img.shields.io/badge/React-19.1.1-61DAFB.svg)](https://reactjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.0-3178C6.svg)](https://www.typescriptlang.org/)
[![Vite](https://img.shields.io/badge/Vite-7.1.7-646CFF.svg)](https://vitejs.dev/)
[![Status](https://img.shields.io/badge/status-Production%20Ready-green.svg)](https://github.com/smdspace-dev/AskTo-Do.git)

#  AI Todo Assistant

##  Features (v2.0.0)

###  Enterprise-Ready
- **Data Persistence**: Robust database layer with instant synchronization
- **User Management**: Complete multi-user support with secure authentication
- **Session Management**: Persistent user sessions across browser restarts
- **Error Recovery**: Comprehensive error handling and user feedback

### Core Capabilities
- **AI Voice Assistant**: Natural language processing for task creation and management
- **Smart Task Parser**: Intelligent extraction of task details from voice commands
- **Real-time Synchronization**: All changes saved instantly with immediate feedback
- **Professional UI**: Consistent dark theme with smooth animations

##  Features

## 🛠️ Technology Stack

### Frontend
- **React 19.1.1** - Modern UI library with latest features
- **TypeScript** - Type-safe development
- **Vite 7.1.7** - Lightning-fast build tool
- **Tailwind CSS 3.x** - Utility-first CSS framework

### Voice & AI
- **Web Speech API** - Browser-native speech recognition and synthesis
- **Natural Language Processing** - Custom parser for task extraction
- **Smart Conversation Management** - Context-aware dialogue system with proper reset logic

### Database & Persistence
- **DatabaseService Layer** - Production-ready data persistence layer
- **Multi-User Support** - Complete user isolation and data separation
- **Instant Synchronization** - All changes saved immediately with error recovery
- **Scalable Architecture** - Ready for enterprise database integration

### Authentication & Security
- **Session Management** - Persistent user sessions with secure logout
- **User Isolation** - Complete data separation between users
- **Error Recovery** - Graceful handling of all error scenarios
- **Production Security** - Secure authentication flow with proper validation

### Development Tools
- **ESLint** - Code linting and quality enforcement
- **Prettier** - Code formatting
- **Husky** - Git hooks for quality control
- **Conventional Commits** - Standardized commit messages

## � Installation

### Prerequisites
- Node.js >= 18.0.0
- npm >= 8.0.0 or yarn >= 1.22.0
- Modern browser with Web Speech API support

### Quick Start

```bash
# Clone the repository
git clone https://github.com/smdspace-dev/AskTo-Do.git
cd ai-todo-assistant

# Install dependencies
npm install

# Copy environment configuration
cp .env.example .env.local

# Start development server
npm run dev
```

The application will be available at `http://localhost:5173`

### Environment Configuration

Copy `.env.example` to `.env.local` and customize:

```env
VITE_APP_NAME=AI Todo Assistant
VITE_ENABLE_VOICE_RECOGNITION=true
VITE_ENABLE_SPEECH_SYNTHESIS=true
VITE_DEBUG_MODE=false
```

## � Usage

### Voice Commands

The AI assistant understands natural language. Try these commands:

#### Task Creation
- *"Create a task to buy groceries tomorrow"*
- *"Add a high priority meeting for Friday at 3 PM"*
- *"Remind me to call the doctor next week"*
- *"Schedule a workout session for tomorrow morning"*

#### Task Management
- *"Show me today's tasks"*
- *"What's my schedule for this week?"*
- *"Mark the first task as complete"*
- *"Delete the grocery shopping task"*

#### Advanced Commands
- *"Add multiple tasks: call dentist, pay bills, and submit report"*
- *"Create a work task with high priority to finish the presentation"*
- *"Show me all high priority tasks for this month"*

### Visual Interface

1. **Click the glowing voice button** to start voice interaction
2. **Use the sidebar** to filter tasks by time periods (Today, Tomorrow, Week, Month)
3. **Task cards** display priority colors and categories
4. **Search bar** for quick task filtering
5. **Quick add button** for manual task creation

## 🗄️ Data Storage

### Database Location
Your tasks and user data are securely stored in your browser's local storage using a robust database service layer:

- **Storage Location**: Browser's local storage (`aiTodoApp_` prefix)
- **Data Persistence**: All data persists across browser sessions
- **User Isolation**: Each user has completely separate data storage
- **Data Security**: Data remains local to your device
- **Backup Capability**: Use the browser's export/import features for data backup

### Data Management
- **Automatic Saving**: All changes save instantly without manual intervention
- **Error Recovery**: Built-in error handling and data validation
- **Clear Tasks**: Use the "Clear Tasks" button to remove all tasks (with confirmation)
- **User Sessions**: Login sessions persist across browser restarts

### Storage Structure
```javascript
// User data: aiTodoApp_users
// User tasks: aiTodoApp_tasks_{userId}
// Current session: aiTodoApp_currentUser
```

## 🏗️ Project Structure

```
src/
├── components/           # React components
│   ├── AIVoiceAssistant.jsx    # Main application component
│   ├── TaskCreationModal.jsx   # Task creation interface
│   ├── SmartTaskParser.jsx     # AI-powered task parsing
│   ├── TaskEditModal.jsx       # Task editing interface
│   ├── AuthModal.jsx           # User authentication
│   └── ErrorBoundary.jsx       # Error handling
├── services/             # Business logic and data services
│   └── DatabaseService.js      # Production data persistence layer
├── utils/                # Utility functions
│   └── conversationManager.js  # AI conversation logic
├── types/                # TypeScript type definitions
└── assets/              # Static assets and styles
```

## 🧪 Development

### Available Scripts

```bash
# Development
npm run dev              # Start development server
npm run build           # Build for production
npm run preview         # Preview production build

# Code Quality
npm run lint            # Run ESLint
npm run lint:fix        # Fix ESLint issues
npm run format          # Format code with Prettier
npm run type-check      # TypeScript type checking

# Testing
npm run test            # Run tests
npm run test:coverage   # Run tests with coverage

# Utilities
npm run clean           # Clean build directory
npm run build:analyze   # Analyze bundle size
```

### Code Standards

- **TypeScript** for type safety
- **ESLint** for code quality
- **Prettier** for consistent formatting
- **Conventional Commits** for commit messages
- **Component-driven development** with proper separation of concerns

### Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/amazing-feature`
3. Make your changes following our coding standards
4. Commit with conventional commit format: `git commit -m "feat: add amazing feature"`
5. Push to the branch: `git push origin feature/amazing-feature`
6. Open a Pull Request

## � Configuration

### Browser Compatibility

- Chrome 25+ (recommended)
- Firefox 44+
- Safari 14.1+
- Edge 79+

**Note:** Voice features require HTTPS in production or localhost in development.

### Performance Optimization

- **Code splitting** for optimal bundle size
- **Lazy loading** of components
- **Memoization** for expensive computations
- **Efficient state management** with minimal re-renders

## 📱 Browser Support

| Feature | Chrome | Firefox | Safari | Edge |
|---------|--------|---------|--------|------|
| Speech Recognition | ✅ | ✅ | ✅ | ✅ |
| Speech Synthesis | ✅ | ✅ | ✅ | ✅ |
| Local Storage | ✅ | ✅ | ✅ | ✅ |
| CSS Grid/Flexbox | ✅ | ✅ | ✅ | ✅ |

## 🐛 Troubleshooting

### Common Issues

**Voice not working:**
- Ensure microphone permissions are granted
- Check if HTTPS is enabled (required for voice features)
- Verify browser support for Web Speech API

**Tasks not saving:**
- Check browser storage availability and quota
- Ensure no browser extensions are blocking data persistence
- Try the "Clear Tasks" button and recreate tasks

**UI not loading:**
- Clear browser cache
- Check for JavaScript errors in console
- Verify all dependencies are installed

## � Production Deployment

### Build for Production
```bash
npm run build
```

### Deploy to Static Hosting
The application is production-ready and can be deployed to any static hosting service:

- **Vercel**: `vercel --prod`
- **Netlify**: Drag and drop the `dist/` folder
- **GitHub Pages**: Upload `dist/` contents
- **Firebase Hosting**: `firebase deploy`

### Environment Requirements
- **HTTPS Required**: Voice features require secure context
- **Modern Browser**: Chrome 25+, Firefox 44+, Safari 14.1+
- **Microphone Access**: Required for voice input functionality

### Production Features
- ✅ Optimized build with code splitting
- ✅ Minified and compressed assets
- ✅ Service worker ready (if needed)
- ✅ Cross-browser compatibility
- ✅ Mobile responsive design
- ✅ Error boundary protection

## �📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Web Speech API** for browser-native voice capabilities
- **React Team** for the amazing framework
- **Tailwind CSS** for the utility-first CSS framework
- **Vite** for the blazing-fast development experience

## 📞 Support

- 📧 Email: contact.thousif+github@gmail.com
- 💬 Issues: [GitHub Issues](https://github.com/Thousifibrahim/AskTo-Do/issues)

---

<div align="center">

**Made with ❤️ by THousifibrahim**

[⭐ Star this repo](https://github.com/Thousifibrahim/AskTo-Do.git) if you find it helpful!

</div>
