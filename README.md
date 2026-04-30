# Learns - Educational Learning Platform

A modern, full-stack learning platform built with React and Firebase. Users can register, log in, explore learning hubs, participate in training-to-placement programs, and manage their profiles.

## 🚀 Features

- **User Authentication** - Secure registration and login with Firebase Authentication
- **LearnHub** - Comprehensive learning content and resources
- **Train to Place** - Training programs focused on job placement
- **User Profiles** - Personalized user profiles with account management
- **Real-time Sync** - Firebase-powered real-time data synchronization
- **Responsive Design** - Built with Tailwind CSS for mobile-first UI
- **Client-side Routing** - Seamless navigation with React Router v7

## 🛠️ Tech Stack

- **Frontend**: React 19.0.0
- **Styling**: Tailwind CSS 4.0.9
- **Routing**: React Router DOM 7.2.0
- **Backend/Database**: Firebase 11.3.1 (Authentication, Firestore, Storage)
- **Testing**: React Testing Library
- **Build Tool**: Create React App / React Scripts 5.0.1

## 📁 Project Structure

```
src/
├── components/
│   ├── home.js           # Landing/Home page
│   ├── login.js          # Login form
│   ├── register.js       # Registration form
│   ├── LearnHub.js       # Learning content hub
│   ├── TrainToPlace.js   # Training & placement programs
│   └── Profile.js        # User profile management
├── App.js                # Main app component with routing
├── App.css               # App-level styles
├── firebaseConfig.js     # Firebase configuration
├── index.js              # React entry point
├── index.css             # Global styles
└── setupTests.js         # Test configuration
```

## 🔧 Installation

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn
- Firebase account with a project

### Setup Steps

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd learns
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Configure Firebase**
   - Create a Firebase project at [Firebase Console](https://console.firebase.google.com)
   - Update `src/firebaseConfig.js` with your Firebase credentials:
   ```javascript
   const firebaseConfig = {
     apiKey: "your-api-key",
     authDomain: "your-auth-domain",
     projectId: "your-project-id",
     storageBucket: "your-storage-bucket",
     messagingSenderId: "your-messaging-sender-id",
     appId: "your-app-id"
   };
   ```

4. **Start the development server**
   ```bash
   npm start
   ```
   The app will open at [http://localhost:3000](http://localhost:3000)

## 📝 Available Scripts

### `npm start`
Runs the app in development mode. The page reloads on changes, and lint errors appear in the console.

### `npm test`
Launches the test runner in interactive watch mode. See [CRA Testing Guide](https://facebook.github.io/create-react-app/docs/running-tests)

### `npm run build`
Creates an optimized production build in the `build/` folder. Files are minified with hashes for caching.

### `npm run eject`
⚠️ **One-way operation** - Exposes all build configuration. Only use if you need full control over webpack, Babel, ESLint, etc.

## 🔐 Authentication Flow

1. User visits the app
2. `App.js` checks authentication state via Firebase
3. Unauthenticated users → Home/Login/Register pages
4. Authenticated users → Full access to LearnHub, TrainToPlace, and Profile

## 🗺️ Route Map

| Path | Component | Status |
|------|-----------|--------|
| `/` | HomePage | Home/Landing |
| `/login` | LoginPage | Authentication |
| `/register` | RegisterPage | Registration |
| `/learn-hub` | LearnHub | Learning Content |
| `/train-to-place` | TrainToPlace | Training Programs |
| `/profile` | Profile | User Profile |
| `*` | Navigate to `/` | Fallback |

## 📦 Dependencies Overview

| Package | Version | Purpose |
|---------|---------|---------|
| react | ^19.0.0 | UI Framework |
| firebase | ^11.3.1 | Backend & Auth |
| react-router-dom | ^7.2.0 | Client-side Routing |
| tailwindcss | ^4.0.9 | Styling |
| react-scripts | 5.0.1 | Build & Dev Tools |

## 🚀 Deployment

### Build for Production
```bash
npm run build
```

The `build` folder is ready to be deployed. See [CRA Deployment Guide](https://facebook.github.io/create-react-app/docs/deployment) for options:
- Vercel
- Netlify
- Firebase Hosting
- GitHub Pages
- Other static hosts

## 🧪 Testing

```bash
npm test
```

Tests run in watch mode. Press `a` to run all tests, `q` to quit.

## 📚 Learn More

- [React Documentation](https://reactjs.org/)
- [Firebase Documentation](https://firebase.google.com/docs)
- [React Router Documentation](https://reactrouter.com/)
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)
- [Create React App Docs](https://facebook.github.io/create-react-app/docs/getting-started)

## 🤝 Contributing

Contributions are welcome! Please follow these steps:
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit changes (`git commit -m 'Add amazing feature'`)
4. Push to branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is private and confidential.

## ❓ Troubleshooting

### Firebase Configuration Issues
- Ensure all environment variables in `firebaseConfig.js` are correct
- Check Firebase Console rules for Firestore and Storage

### Port Already in Use
```bash
PORT=3001 npm start
```

### Build Fails
```bash
# Clear cache and reinstall
rm -rf node_modules package-lock.json
npm install
npm run build
```

## 📧 Support

## 🎯 Key Highlights
- 🔐 Secure Firebase Authentication
- ⚡ Real-time data sync with Firestore
- 📱 Fully responsive (mobile-first design)
- 🚀 Clean modular React architecture

For issues or questions, contact the development team.
