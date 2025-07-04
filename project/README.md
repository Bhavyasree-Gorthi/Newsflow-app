# NES News - Flutter News Aggregator App

A modern, clean news aggregator app built with Flutter that fetches and displays news articles from NewsAPI.org.

## Features

- 📰 **Trending News**: View the latest news articles on the home screen
- 🏷️ **Category Filtering**: Filter news by categories (Business, Sports, Tech, etc.)
- 🔍 **Search**: Search for news articles by keyword
- 📱 **News Details**: View full details of news articles
- 🌙 **Dark/Light Mode**: Toggle between light and dark themes
- 📱 **Cross-Platform**: Works on both Android and iOS
- 🔄 **Pull-to-Refresh**: Refresh news with pull gesture
- 🖼️ **Image Caching**: Efficient image loading with caching

## Tech Stack

- **Frontend**: Flutter with Dart
- **State Management**: Provider pattern
- **API**: NewsAPI.org
- **Image Caching**: cached_network_image
- **HTTP Client**: http package
- **URL Launcher**: url_launcher for opening articles

## Getting Started

### Prerequisites

- Flutter SDK (latest stable version)
- Dart SDK
- Android Studio / VS Code
- NewsAPI.org API key

### Installation

1. **Clone or download the project**
   ```bash
   cd flutter_nes_news
   ```

2. **Install dependencies**
   ```bash
   flutter pub get
   ```

3. **Configure API Key**
   - Open `lib/utils/env.dart`
   - Replace `YOUR_API_KEY_HERE` with your actual NewsAPI.org API key
   - Get your free API key from [NewsAPI.org](https://newsapi.org/)

4. **Run the app**
   ```bash
   flutter run
   ```

## Project Structure

```
lib/
├── main.dart                 # App entry point
├── core/
│   ├── constants/
│   │   └── api_constants.dart # API configuration
│   └── theme/
│       └── app_theme.dart    # App themes
├── models/
│   └── article_model.dart    # Article data model
├── services/
│   └── news_service.dart     # API service
├── view/
│   ├── screens/
│   │   ├── home_screen.dart  # Main news list
│   │   ├── detail_screen.dart # Article detail
│   │   └── settings_screen.dart # Settings
│   └── widgets/
│       └── news_tile.dart    # News card widget
├── viewmodel/
│   └── news_provider.dart    # State management
└── utils/
    └── env.dart             # Environment variables
```

## API Configuration

The app uses NewsAPI.org for fetching news articles. You need to:

1. Sign up at [NewsAPI.org](https://newsapi.org/)
2. Get your free API key
3. Replace the placeholder in `lib/utils/env.dart`

```dart
class Env {
  static const String apiKey = 'YOUR_ACTUAL_API_KEY';
}
```

## Features in Detail

### Home Screen
- Displays trending news articles
- Category tabs for filtering
- Search bar for keyword search
- Pull-to-refresh functionality
- Error handling with retry option

### Article Detail Screen
- Full article content
- Article metadata (author, date, source)
- Share functionality
- "Read Full Article" button to open in browser

### Settings Screen
- Dark/Light mode toggle
- App information
- API information

### News Categories
- Business
- Entertainment
- General
- Health
- Science
- Sports
- Technology

## Dependencies

```yaml
dependencies:
  flutter:
    sdk: flutter
  http: ^1.1.0
  provider: ^6.1.1
  cached_network_image: ^3.3.0
  url_launcher: ^6.2.1
  shared_preferences: ^2.2.2
  flutter_dotenv: ^5.1.0
```

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## License

This project is open source and available under the [MIT License](LICENSE).

## Support

If you encounter any issues or have questions:

1. Check the [Flutter documentation](https://flutter.dev/docs)
2. Verify your API key is correct
3. Ensure you have a stable internet connection
4. Check the NewsAPI.org status

## Screenshots

[Add screenshots of your app here]

---

**Built with ❤️ using Flutter** 