# NewsCloud 📰

A simple news app built with **Flutter**. The app fetches live headlines from [NewsAPI](https://newsapi.org/) and lets users browse news by category.

## Features

- Browse top headlines by category (General, Sports, Technology, Business, etc.)
- Category selector on the home screen
- Article detail view opened in an in-app WebView
- Loading and error states while fetching data

## Screenshots

| Home | Category | Article |
|------|----------|---------|
| <img width="300" src="https://github.com/user-attachments/assets/ce155ad3-dec5-4290-9609-3b665c7e5843" /> | <img width="300" src="https://github.com/user-attachments/assets/27e8b8c5-ce87-47d2-aa11-86eb2d24545b" /> |<img width="300" src="https://github.com/user-attachments/assets/0442881d-eea5-4643-bf8d-95f2c36d8074" /> |

## Tech Stack

- **Flutter** / Dart
- **Dio** — HTTP client for API requests
- **webview_flutter** — in-app browser for reading full articles
- **NewsAPI** — data source for headlines

## Project Structure

```
lib/
├── models/          # Data models (Article, Category)
├── services/        # API calls (NewsService)
├── Views/           # Screens (Home, Category, Detail)
├── widgets/         # Reusable UI pieces (list builder, cards, tiles)
└── main.dart
```

## Note on the API Key

The NewsAPI key in `news_service.dart` is a free-tier test key with no sensitive data behind it, left in the code for simplicity. In production projects, API keys should be kept out of source control (e.g. using `flutter_dotenv` + `.gitignore`).

