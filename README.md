# React Native Movie App 🎬

A modern, cross-platform mobile application built with React Native and Expo that allows users to discover, search, and save their favorite movies. The app features a beautiful UI with smooth animations and integrates with popular movie APIs and cloud services.

## 🚀 Features

- **Movie Discovery**: Browse trending and popular movies
- **Advanced Search**: Search movies by title with real-time results
- **Movie Details**: View comprehensive movie information including ratings, cast, and synopsis
- **Save Favorites**: Save movies to your personal collection
- **Trending Analytics**: View most searched movies based on user activity
- **Cross-Platform**: Works on iOS, Android, and Web
- **Modern UI**: Beautiful design with smooth animations and gradients
- **Offline Support**: Cached data for better user experience

## 🛠 Tech Stack

### Core Framework
- **React Native** (0.76.7) - Cross-platform mobile development
- **Expo** (52.0.31) - Development platform and build tools
- **TypeScript** (5.3.3) - Type-safe JavaScript development

### Navigation & Routing
- **Expo Router** (4.0.17) - File-based routing system
- **React Navigation** (7.0.14) - Navigation library
- **React Navigation Bottom Tabs** (7.2.0) - Tab navigation

### UI & Styling
- **NativeWind** (4.1.23) - Tailwind CSS for React Native
- **Tailwind CSS** (3.4.17) - Utility-first CSS framework
- **Expo Linear Gradient** (14.0.2) - Gradient components
- **Expo Blur** (14.0.3) - Blur effects
- **React Native Heroicons** (4.0.0) - Icon library

### Animation & Interactions
- **React Native Reanimated** (3.16.1) - Smooth animations
- **React Native Gesture Handler** (2.20.2) - Touch gestures
- **Expo Haptics** (14.0.1) - Haptic feedback

### Backend & APIs
- **TMDB API** - The Movie Database API for movie data
- **Appwrite** (react-native-appwrite 0.7.0) - Backend-as-a-Service for user data and analytics

### Development Tools
- **Jest** (29.2.1) - Testing framework
- **Babel** (7.25.2) - JavaScript compiler
- **Metro** - React Native bundler

## 📱 Project Structure

```
react-native-movie-app-main/
├── app/                    # Expo Router pages
│   ├── (tabs)/            # Tab navigation screens
│   │   ├── index.tsx      # Home screen
│   │   ├── search.tsx     # Search screen
│   │   ├── save.tsx       # Saved movies
│   │   └── profile.tsx    # User profile
│   ├── movie/
│   │   └── [id].tsx       # Movie details page
│   └── _layout.tsx        # Root layout
├── components/            # Reusable UI components
│   ├── MovieCard.tsx      # Movie card component
│   ├── SearchBar.tsx      # Search input component
│   └── TrendingCard.tsx   # Trending movie card
├── services/              # API and external services
│   ├── api.ts            # TMDB API integration
│   ├── appwrite.ts       # Appwrite backend service
│   └── usefetch.ts       # Custom fetch hook
├── interfaces/            # TypeScript type definitions
├── constants/             # App constants and configurations
├── assets/               # Images, icons, and fonts
└── types/                # Additional type definitions
```

## 🚀 Getting Started

### Prerequisites

- Node.js (v18 or higher)
- npm or yarn
- Expo CLI (`npm install -g @expo/cli`)
- iOS Simulator (for iOS development)
- Android Studio (for Android development)

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd react-native-movie-app-main
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Environment Setup**
   Create a `.env` file in the root directory with the following variables:
   ```env
   EXPO_PUBLIC_MOVIE_API_KEY=your_tmdb_api_key
   EXPO_PUBLIC_APPWRITE_PROJECT_ID=your_appwrite_project_id
   EXPO_PUBLIC_APPWRITE_DATABASE_ID=your_appwrite_database_id
   EXPO_PUBLIC_APPWRITE_COLLECTION_ID=your_appwrite_collection_id
   ```

4. **Start the development server**
   ```bash
   npm start
   ```

5. **Run on your preferred platform**
   ```bash
   # iOS
   npm run ios
   
   # Android
   npm run android
   
   # Web
   npm run web
   ```

## 🔧 Available Scripts

- `npm start` - Start the Expo development server
- `npm run ios` - Run on iOS simulator
- `npm run android` - Run on Android emulator
- `npm run web` - Run on web browser
- `npm test` - Run tests in watch mode
- `npm run lint` - Run ESLint

## 📊 API Integration

### TMDB API
The app integrates with The Movie Database (TMDB) API to fetch:
- Movie search results
- Movie details and metadata
- Popular and trending movies
- Movie posters and images

### Appwrite Backend
Appwrite is used for:
- Storing user search analytics
- Tracking trending searches
- User preferences and saved movies

## 🎨 UI/UX Features

- **Responsive Design**: Adapts to different screen sizes
- **Dark/Light Mode**: Automatic theme switching
- **Smooth Animations**: Reanimated for fluid interactions
- **Gradient Backgrounds**: Modern visual appeal
- **Haptic Feedback**: Enhanced user experience
- **Loading States**: Proper loading indicators

## 🧪 Testing

The project includes Jest testing setup with:
- Component testing
- API integration testing
- Custom hooks testing

Run tests with:
```bash
npm test
```

## 📦 Building for Production

### iOS
```bash
expo build:ios
```

### Android
```bash
expo build:android
```

### Web
```bash
expo build:web
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [TMDB](https://www.themoviedb.org/) for providing the movie data API
- [Appwrite](https://appwrite.io/) for the backend services
- [Expo](https://expo.dev/) for the development platform
- [React Native](https://reactnative.dev/) community

## 📞 Support

If you encounter any issues or have questions, please:
1. Check the [Issues](../../issues) page
2. Create a new issue with detailed information
3. Contact the development team

---

Made with ❤️ using React Native and Expo 