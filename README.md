# SIH Project - Environmental Reporting Platform

A React-based web application for reporting environmental issues with Firebase authentication, geo-tagged image uploads, and awareness content.

## Features

- 🔐 **Firebase Authentication** - Email/password login and registration
- 📍 **Geo-tagged Reporting** - Upload images with GPS coordinates
- 🏠 **Dashboard** - User-friendly home page with navigation
- 📊 **Report Dumping** - Submit environmental issues with descriptions
- 🌱 **Awareness Page** - Educational content about environmental issues
- 📱 **Responsive Design** - Works on desktop and mobile devices

## Pages

1. **Login/Register Page** - User authentication
2. **Home Page** - Dashboard with feature overview
3. **Report Dumping Page** - Upload geo-tagged images and descriptions
4. **Awareness Page** - Static educational content

## Setup Instructions

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn
- Firebase project

### 1. Install Dependencies

```bash
npm install
```

### 2. Firebase Configuration

1. Create a new Firebase project at [Firebase Console](https://console.firebase.google.com/)
2. Enable Authentication with Email/Password
3. Create a Firestore database
4. Enable Storage for image uploads
5. Copy your Firebase configuration and update `src/firebase.js`:

```javascript
const firebaseConfig = {
  apiKey: "your-api-key",
  authDomain: "your-project.firebaseapp.com",
  projectId: "your-project-id",
  storageBucket: "your-project.appspot.com",
  messagingSenderId: "123456789",
  appId: "your-app-id"
};
```

### 3. Run the Application

```bash
npm start
```

The application will open at `http://localhost:3000`

## Project Structure

```
src/
├── components/
│   ├── Auth.css
│   ├── Awareness.css
│   ├── Home.css
│   ├── Navbar.css
│   ├── ReportDumping.css
│   ├── Awareness.js
│   ├── Home.js
│   ├── Login.js
│   ├── Navbar.js
│   ├── Register.js
│   └── ReportDumping.js
├── contexts/
│   └── AuthContext.js
├── App.css
├── App.js
├── firebase.js
├── index.css
└── index.js
```

## Technologies Used

- **React 18** - Frontend framework
- **React Router** - Client-side routing
- **Firebase** - Authentication, Firestore, Storage
- **CSS3** - Modern styling with gradients and animations
- **Geolocation API** - GPS coordinate capture

## Features in Detail

### Authentication
- Secure email/password authentication
- Protected routes for authenticated users
- Automatic redirects based on auth state

### Report Dumping
- Image upload with 5MB size limit
- Automatic GPS coordinate capture
- Form validation and error handling
- Firebase Storage integration

### Responsive Design
- Mobile-first approach
- Modern UI with gradients and shadows
- Smooth animations and transitions
- Accessible form controls

## Security Notes

- Update Firebase security rules for production
- Implement proper error handling
- Add input validation and sanitization
- Consider rate limiting for uploads

## Future Enhancements

- Real-time notifications
- Map visualization of reports
- Admin dashboard
- Report status tracking
- Social sharing features
- Advanced analytics

## License

This project is created for SIH (Smart India Hackathon) purposes.
