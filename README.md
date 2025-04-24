# RIDA - Road Safety AI Dashboard

## Project Overview

RIDA (Road Safety AI Dashboard) is a comprehensive web application designed to monitor and analyze road safety data in real-time. The dashboard provides insights on traffic conditions, weather impacts, accident hotspots, and trends to help maintain safer road conditions.

## Features

- **Role-based Authentication**: Different access levels for Admin, Analyst, and General User roles
- **Live Traffic Reports**: Real-time updates on road conditions and incidents
- **Weather Integration**: Current weather conditions and forecasts
- **Accident Heatmap**: Visual representation of accident-prone areas
- **Trend Analysis**: Weekly, monthly, and yearly trend graphs
- **City Search**: Quick access to city-specific data
- **Responsive Design**: Optimized for both desktop and mobile devices

## Login Credentials (Demo)

For testing the application, use the following credentials:

- **Admin**: admin@rida.com / password
- **Analyst**: analyst@rida.com / password
- **General User**: user@rida.com / password

## Technologies Used

- React with TypeScript
- Firebase (Authentication, Firestore, Realtime Database, Cloud Functions)
- Tailwind CSS with shadcn/ui components
- Recharts for data visualization
- React Router for navigation
- Vite for development and build tooling

## Project Setup Instructions

1. Clone the repository
2. Install dependencies: `npm install`
3. Set up Firebase:
   - Create a Firebase project at [firebase.google.com](https://firebase.google.com)
   - Enable Authentication, Firestore, Realtime Database, and Cloud Functions
   - Update the Firebase configuration in `src/lib/firebase.ts`
4. Start the development server: `npm run dev`

## Firebase Configuration

To connect the application to your Firebase project, update the configuration in `src/lib/firebase.ts`:

```javascript
const firebaseConfig = {
  apiKey: "your-api-key",
  authDomain: "your-project.firebaseapp.com",
  projectId: "your-project-id",
  storageBucket: "your-project.appspot.com",
  messagingSenderId: "your-messaging-sender-id",
  appId: "your-app-id"
};
```

## Project Structure

- `src/components/` - Reusable UI components
- `src/components/dashboard/` - Dashboard-specific widgets
- `src/components/layout/` - Layout components (Sidebar, Header)
- `src/components/auth/` - Authentication-related components
- `src/context/` - React context providers (Auth)
- `src/pages/` - Main application pages
- `src/lib/` - Utility functions and services

