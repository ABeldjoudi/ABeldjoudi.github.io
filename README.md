# WalkWithUs 🚶‍♂️

**Version 1.0.9**

A mobile app that connects people who love walking. Find walking buddies, organize group walks, and track your fitness journey.

## Features

### 🗓️ Walk Organization
- Create and organize group walks in your neighborhood
- Set walk conditions (age groups, gender preferences, pace)
- Automatic participant notifications and reminders

### 🔍 Walk Discovery
- Find walks near you based on your location
- Filter by date, distance, and preferences
- Book walks with one tap

### 📊 GPS Walk Tracking (NEW in v1.0.4)
- Track your walks with real-time GPS
- Monitor distance, steps, calories, time and Weight Loss
- View monthly trends and statistics
- All route data stored locally for privacy

### 🏆 Achievements & Badges
- Earn badges for walking milestones
- Track your progress from Walker to Legend
- Celebration animations and sounds

### 👤 User Profiles
- Customizable profiles with photo
- Walking history and statistics
- Badge showcase

## Tech Stack

- **Frontend**: React Native / Expo
- **Backend**: FastAPI (Python)
- **Database**: MongoDB
- **Authentication**: Google Sign-In, Apple Sign-In
- **Maps**: react-native-maps
- **Analytics**: expo-location, expo-sensors

## Project Structure

```
/app
├── backend/          # FastAPI backend server
│   ├── server.py     # Main API endpoints
│   └── requirements.txt
├── frontend/         # Expo React Native app
│   ├── app/          # Screen components (file-based routing)
│   ├── components/   # Reusable UI components
│   ├── contexts/     # React contexts (Auth, etc.)
│   ├── utils/        # Utility functions
│   └── assets/       # Images, sounds, fonts
└── README.md
```

## Environment Variables

### Backend (.env)
```
MONGO_URL=<mongodb-connection-string>
GOOGLE_CLIENT_ID=<google-oauth-client-id>
APPLE_TEAM_ID=<apple-team-id>
```

### Frontend (.env)
```
EXPO_PUBLIC_BACKEND_URL=<backend-api-url>
```

## Running Locally

### Backend
```bash
cd backend
pip install -r requirements.txt
uvicorn server:app --host 0.0.0.0 --port 8001
```

### Frontend
```bash
cd frontend
yarn install
eas build --platform android --profile production
```

## Privacy

See [PRIVACY.md](./PRIVACY.md) for our full privacy policy.

## License

Proprietary - All rights reserved.

## Contact

For support: abdelkaderbeldjoudi8@gmail.com
