# 🎤 Air Assist PWA

**A Professional Voice-Powered AI Assistant with Advanced Bluetooth Audio Support**

Air Assist is a cutting-edge Progressive Web App (PWA) that transforms your device into a powerful voice-controlled AI assistant. With enterprise-grade Bluetooth audio integration, real-time voice recognition, and seamless cross-platform compatibility, Air Assist delivers a premium conversational AI experience.

[![Live Demo](https://img.shields.io/badge/Live%20Demo-air--assist--app.vercel.app-blue?style=for-the-badge&logo=vercel)](https://air-assist-app.vercel.app)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
[![PWA](https://img.shields.io/badge/PWA-Ready-purple?style=for-the-badge&logo=pwa)](https://web.dev/progressive-web-apps/)

## ✨ Key Features

### 🎧 **Advanced Bluetooth Audio Support**
- **Universal Bluetooth Compatibility**: Works with AirPods, Sony, Bose, JBL, Beats, Jabra, J55, and any Bluetooth audio device
- **Dual Audio Channels**: Simultaneous Bluetooth microphone input and speaker output
- **Real-time Audio Monitoring**: Visual audio level indicators with professional-grade feedback
- **Device Auto-Detection**: Automatic recognition and configuration of Bluetooth devices
- **Cross-Platform Optimization**: Platform-specific audio handling for Windows, macOS, iOS, and Android
- **Mobile Bluetooth Support**: Enhanced mobile browser compatibility with system audio routing

### 🗣️ **Intelligent Voice Recognition**
- **Real-time Speech Processing**: Instant voice command recognition with Web Speech API
- **Continuous Listening Mode**: Hands-free operation with voice activation
- **Multi-language Support**: Supports multiple languages and accents
- **Noise Cancellation**: Advanced audio processing for clear voice input
- **Voice Command History**: Track and review previous voice interactions
- **Microphone Testing**: Built-in audio testing tools for troubleshooting

### 🤖 **AI-Powered Conversations**
- **OpenAI GPT Integration**: Powered by state-of-the-art language models
- **Context-Aware Responses**: Maintains conversation context for natural interactions
- **Real-time Processing**: Instant AI responses with minimal latency
- **Conversation Memory**: Persistent chat history across sessions
- **Dual AI Provider Support**: OpenAI and n8n webhook integration
- **Custom Prompts**: Tailored AI responses for specific use cases

### 📱 **Progressive Web App Excellence**
- **Cross-Platform Compatibility**: Works on Windows, macOS, iOS, Android, and Linux
- **Offline Capability**: Core functionality available without internet connection
- **Native App Experience**: Install on any device for app-like performance
- **Responsive Design**: Optimized for desktop, tablet, and mobile devices
- **Push Notifications**: Stay updated with important alerts and responses
- **Service Worker**: Advanced caching and offline functionality

## 🚀 Quick Start

### 📋 Prerequisites

- **Node.js** (v16 or higher) - [Download here](https://nodejs.org/)
- **npm** or **yarn** package manager
- **OpenAI API Key** - [Get yours here](https://platform.openai.com/api-keys)
- **Modern Browser** - Chrome, Edge, Firefox, or Safari
- **Bluetooth Device** (optional) - For enhanced audio experience

### ⚡ One-Command Setup

```bash
# Clone and setup everything
git clone https://github.com/your-username/air-assist-pwa.git
cd air-assist-pwa/frontend
npm install
npm run dev:full
```

**That's it!** The app will be running at `http://localhost:5173` with the backend at `http://localhost:3001`.

## 🛠️ Detailed Installation Guide

## Setup Instructions

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/air-assist-pwa.git
cd air-assist-pwa
```

### 2️⃣ Install Dependencies

```bash
cd frontend
npm install
```

### 3️⃣ Environment Configuration

Create a `.env` file in the `frontend` directory:

```bash
cp .env.example .env
```

Edit the `.env` file and add your configuration:

```env
# 🤖 OpenAI API Configuration
VITE_OPENAI_API_KEY=your_openai_api_key_here
OPENAI_API_KEY=your_openai_api_key_here

# 🖥️ Server Configuration
PORT=3001
NODE_ENV=development

# 🌐 API Configuration
VITE_BACKEND_URL=http://localhost:3001
VITE_WEBSOCKET_URL=ws://localhost:3001/openai-realtime

# 🔗 n8n Integration (Optional)
VITE_DEFAULT_N8N_URL=https://your-n8n-instance.com/webhook/air

# 📱 App Configuration
VITE_APP_NAME=Air Assist
VITE_DEBUG_MODE=true
```

> **🔒 Security Note**: Never commit your `.env` files to version control. They're already included in `.gitignore`.

### 4️⃣ Running the Application

#### 🚀 Development Mode (Recommended)

**Option 1: Full Development Setup (One Command)**
```bash
cd frontend
npm run dev:full
```

**Option 2: Separate Terminals**
```bash
# Terminal 1: Backend Server
cd frontend
npm run server:dev

# Terminal 2: Frontend Development Server
cd frontend
npm run dev
```

#### 🌐 Access URLs
- **Frontend**: http://localhost:5173
- **Backend API**: http://localhost:3001
- **Live Demo**: https://air-assist-app.vercel.app

#### 🏗️ Production Build

```bash
cd frontend
npm run start
```

This builds the frontend and starts the production server.

## 🎧 Bluetooth Setup Guide

### 🖥️ Desktop Setup (Windows/Mac/Linux)

1. **Pair Your Device**: Connect your Bluetooth headphones/earbuds to your computer
2. **Set as Default**: Make your Bluetooth device the default audio device in system settings
3. **Open Air Assist**: Launch the app in Chrome or Edge (recommended)
4. **Scan Devices**: Click "Scan Audio Devices" button
5. **Auto-Selection**: App automatically detects and selects your Bluetooth device
6. **Test Microphone**: Use the built-in microphone test feature

### 📱 Mobile Setup (iOS/Android)

#### 🍎 iOS Safari
1. **Pair Device**: Settings → Bluetooth → Connect your headphones
2. **Enable Audio**: Tap "i" next to device → Enable "Use for Audio"
3. **Set Default**: Control Center → Audio controls → Select Bluetooth device
4. **Install PWA**: Safari → Share → "Add to Home Screen" (recommended)
5. **Test Voice**: Use the microphone test in app settings

#### 🤖 Android Chrome
1. **Pair Device**: Settings → Connected devices → Bluetooth → Connect headphones
2. **Enable Audio**: Tap gear icon → Enable "Phone calls" and "Media audio"
3. **Set Default**: Settings → Sound → Advanced → Set Bluetooth as default
4. **Install PWA**: Chrome → Menu → "Add to Home screen" (recommended)
5. **Test Voice**: Use the microphone test in app settings

### 🎯 Supported Bluetooth Devices

✅ **Tested and Verified**:
- Apple AirPods (all models)
- Sony WH-1000XM series
- Bose QuietComfort series
- JBL headphones and earbuds
- Beats headphones
- Jabra Elite series
- Samsung Galaxy Buds
- J55 TWS earbuds
- Any Bluetooth audio device with microphone

## 🔧 Configuration & Settings

### 🤖 OpenAI API Configuration

1. **Get API Key**: Visit [OpenAI Platform](https://platform.openai.com/api-keys)
2. **Add to Environment**: Update your `.env` file with the API key
3. **In-App Setup**: The app will prompt you to enter the API key in settings
4. **Verify Connection**: Test the AI functionality with a voice command

### 🔗 n8n Integration (Optional)

1. **Setup n8n**: Deploy your n8n instance
2. **Create Webhook**: Set up a webhook endpoint for Air Assist
3. **Configure URL**: Add the webhook URL in app settings
4. **Test Integration**: Verify the connection works properly

### ⚙️ Advanced Settings

- **Voice Recognition Language**: Configure speech recognition language
- **AI Model Selection**: Choose between different OpenAI models
- **Audio Quality**: Adjust microphone and speaker settings
- **Conversation History**: Enable/disable chat persistence
- **Debug Mode**: Enable detailed logging for troubleshooting

## 🔒 Security & Privacy

### ✅ Security Features
- **Environment Variables**: API keys stored securely in `.env` files
- **Git Protection**: All sensitive files excluded from version control
- **Client-Side Security**: No API keys exposed in frontend code
- **HTTPS Ready**: Production deployment uses secure connections
- **Local Processing**: Voice recognition happens locally when possible

### 🛡️ Privacy Considerations
- **Voice Data**: Processed locally via Web Speech API
- **Conversation History**: Stored locally in browser storage
- **API Calls**: Only sent to configured AI providers
- **No Tracking**: No analytics or user tracking implemented
- **Offline Mode**: Core functionality works without internet

### ⚠️ Production Recommendations
- Use HTTPS/WSS for all connections
- Implement proper authentication for multi-user deployments
- Regular security updates and dependency management
- Monitor API usage and implement rate limiting

## 🌐 Browser Compatibility

### ✅ Fully Supported
- **Chrome/Chromium** (Windows, Mac, Linux, Android)
- **Microsoft Edge** (Windows, Mac)
- **Chrome Mobile** (Android)

### ⚠️ Limited Support
- **Firefox** (Limited Bluetooth support, full voice recognition)
- **Safari** (Limited Web Speech API, basic Bluetooth)
- **Safari Mobile** (iOS - Enhanced with PWA installation)

### 📱 Mobile Optimization
- **PWA Installation**: Recommended for better audio access
- **System Audio Routing**: Optimized for mobile Bluetooth limitations
- **Responsive Design**: Touch-friendly interface for all screen sizes

## 🔧 Troubleshooting Guide

### 🎤 Voice Recognition Issues

**Problem**: Speech recognition not working
- ✅ **Check Permissions**: Ensure microphone access is granted
- ✅ **Test Microphone**: Use the built-in microphone test feature
- ✅ **Browser Support**: Use Chrome or Edge for best results
- ✅ **Quiet Environment**: Reduce background noise
- ✅ **Clear Speech**: Speak clearly and at normal volume

**Problem**: Voice commands not recognized
- ✅ **Language Settings**: Check speech recognition language
- ✅ **Internet Connection**: Voice recognition requires internet
- ✅ **Microphone Quality**: Ensure good audio input quality

### 🎧 Bluetooth Audio Issues

**Problem**: Bluetooth device not detected
- ✅ **Device Pairing**: Ensure device is paired with your computer/phone
- ✅ **Default Device**: Set Bluetooth device as default audio device
- ✅ **Browser Compatibility**: Use Chrome/Edge for best Bluetooth support
- ✅ **Rescan Devices**: Click "Scan Audio Devices" button
- ✅ **Device Reset**: Disconnect and reconnect Bluetooth device

**Problem**: Audio output works but microphone doesn't
- ✅ **Communication Device**: Set Bluetooth device as default communication device
- ✅ **Mobile Setup**: Follow platform-specific mobile setup instructions
- ✅ **PWA Installation**: Install as PWA on mobile for better audio access
- ✅ **System Settings**: Check system audio settings for microphone permissions

### 🤖 AI Integration Issues

**Problem**: OpenAI API errors
- ✅ **API Key**: Verify your OpenAI API key is correct
- ✅ **Account Credits**: Check your OpenAI account has sufficient credits
- ✅ **Rate Limits**: Ensure you haven't exceeded API rate limits
- ✅ **Network**: Check internet connection and firewall settings

**Problem**: No AI responses
- ✅ **Backend Running**: Ensure the backend server is running
- ✅ **Environment Variables**: Check `.env` file configuration
- ✅ **CORS Settings**: Verify CORS is properly configured
- ✅ **Console Errors**: Check browser console for error messages

### 🌐 Connection Issues

**Problem**: Backend connection fails
- ✅ **Server Running**: Ensure backend is running on correct port (3001)
- ✅ **Port Conflicts**: Check if port 3001 is available
- ✅ **Firewall**: Check firewall settings aren't blocking connections
- ✅ **Environment URLs**: Verify VITE_BACKEND_URL is correct

### 📱 Mobile-Specific Issues

**Problem**: App doesn't work well on mobile
- ✅ **PWA Installation**: Install as PWA for better performance
- ✅ **Browser Choice**: Use Chrome on Android, Safari on iOS
- ✅ **System Audio**: Set Bluetooth device as system default
- ✅ **Permissions**: Grant all requested permissions

### 🔧 Environment & Setup Issues

**Problem**: Environment variables not loading
- ✅ **File Location**: Ensure `.env` file is in `frontend` directory
- ✅ **File Permissions**: Check file is readable
- ✅ **Syntax Errors**: Verify no syntax errors in `.env` file
- ✅ **Server Restart**: Restart the development server
- ✅ **Variable Names**: Ensure variables start with `VITE_` for frontend

**Problem**: Dependencies installation fails
- ✅ **Node Version**: Ensure Node.js v16 or higher
- ✅ **Clear Cache**: Run `npm cache clean --force`
- ✅ **Delete node_modules**: Remove and reinstall dependencies
- ✅ **Network Issues**: Check internet connection and npm registry access

## 🛠️ Development Guide

### 📁 Project Structure

```
air-assist-pwa/
├── 📁 frontend/                    # Main application directory
│   ├── 📁 src/
│   │   ├── 📄 App.jsx             # Main React application
│   │   ├── 📄 App.css             # Application styles
│   │   ├── 📄 main.jsx            # React entry point
│   │   └── 📁 components/         # React components
│   ├── 📁 public/                 # Static assets
│   │   ├── 📄 manifest.json       # PWA manifest
│   │   └── 🖼️ icons/              # App icons
│   ├── 📁 api/                    # Serverless API functions
│   │   └── 📄 openai-proxy.js     # OpenAI API proxy
│   ├── 📄 server.js               # Express server for development
│   ├── 📄 package.json            # Dependencies and scripts
│   ├── 📄 vite.config.js          # Vite configuration
│   ├── 📄 .env                    # Environment variables (not in git)
│   └── 📄 .env.example            # Environment template
├── 📄 README.md                   # This file
├── 📄 LICENSE                     # MIT License
└── 📄 .gitignore                  # Git ignore rules
```

### 🔧 Available Scripts

```bash
# Development
npm run dev              # Start frontend development server
npm run server:dev       # Start backend server with nodemon
npm run dev:full         # Start both frontend and backend

# Production
npm run build            # Build for production
npm run preview          # Preview production build
npm run start            # Build and start production server

# Utilities
npm run lint             # Run ESLint
npm run server           # Start backend server
```

### 🎯 Key Technologies

- **Frontend**: React 19, Vite, PWA
- **Backend**: Express.js, Node.js
- **AI Integration**: OpenAI GPT API
- **Audio**: Web Speech API, Web Audio API, Web Bluetooth API
- **Styling**: CSS3, Responsive Design
- **Deployment**: Vercel (Frontend), Serverless Functions

### 🔄 Development Workflow

1. **Setup**: Clone repo and install dependencies
2. **Environment**: Configure `.env` file with API keys
3. **Development**: Run `npm run dev:full` for full stack development
4. **Testing**: Test voice recognition and Bluetooth functionality
5. **Building**: Run `npm run build` for production build
6. **Deployment**: Deploy to Vercel or your preferred platform

### 🧪 Testing Guidelines

- **Voice Recognition**: Test with different accents and languages
- **Bluetooth Audio**: Test with various Bluetooth devices
- **Cross-Platform**: Test on Windows, Mac, iOS, Android
- **Browser Compatibility**: Test on Chrome, Edge, Firefox, Safari
- **PWA Functionality**: Test installation and offline capabilities
- **API Integration**: Verify OpenAI and n8n integrations work

## 🤝 Contributing

We welcome contributions! Here's how to get started:

### 🚀 Quick Contribution Guide

1. **Fork** the repository
2. **Clone** your fork: `git clone https://github.com/your-username/air-assist-pwa.git`
3. **Create** a feature branch: `git checkout -b feature/amazing-feature`
4. **Make** your changes and test thoroughly
5. **Commit** with descriptive messages: `git commit -m "✨ Add amazing feature"`
6. **Push** to your branch: `git push origin feature/amazing-feature`
7. **Submit** a Pull Request

### 📋 Contribution Guidelines

- **Code Style**: Follow existing code patterns and ESLint rules
- **Testing**: Test your changes across different browsers and devices
- **Documentation**: Update README.md if you add new features
- **Commits**: Use descriptive commit messages with emojis
- **Issues**: Check existing issues before creating new ones

### 🎯 Areas for Contribution

- 🎧 **Bluetooth Support**: Enhance device compatibility
- 🗣️ **Voice Recognition**: Improve accuracy and language support
- 🤖 **AI Integration**: Add new AI providers or features
- 📱 **Mobile Experience**: Enhance mobile browser compatibility
- 🎨 **UI/UX**: Improve design and user experience
- 🔧 **Performance**: Optimize loading and response times
- 📚 **Documentation**: Improve guides and tutorials

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

### 📞 Support & Community

- **Issues**: [GitHub Issues](https://github.com/your-username/air-assist-pwa/issues)
- **Discussions**: [GitHub Discussions](https://github.com/your-username/air-assist-pwa/discussions)
- **Live Demo**: [air-assist-app.vercel.app](https://air-assist-app.vercel.app)

---

**Made with ❤️ by the Air Assist team**

*Transform your voice into intelligent conversations with Air Assist PWA!*
