# Weather App 🌤️

![Weather App](https://img.shields.io/badge/version-1.0-blue.svg)  
![Weather App](https://img.shields.io/badge/platform-Flutter-lightblue.svg)  
![Weather App](https://img.shields.io/badge/api-openweathermap.org-brightgreen.svg)

The **Weather App** is a cross-platform application built using Flutter for both Android and iOS. It utilizes the OpenWeatherMap API to fetch and display real-time weather information. The app adheres to the **Bloc State Management Pattern** for clean and structured architecture.

---

## Features

- **Cross-Platform**: Available on both Android and iOS.
- **State Management**: Implements the Bloc architecture for structured and scalable code.
- **Dynamic Weather Updates**: Fetches real-time weather data.
- **Customizable Units**: Switch between Celsius and Fahrenheit.
- **Search Functionality**: Look up weather by city name.
- **Error Handling**: Graceful handling of API errors and exceptions.
- **Theming**: Dynamic theme switching.

---

## Project Structure

### **Bloc Structure**

The application uses the **Bloc** pattern with the following structure:

```
blocs/
├── weather/
│   ├── weather_bloc.dart
│   ├── weather_event.dart
│   ├── weather_state.dart
├── theme/
│   ├── theme_bloc.dart
│   ├── theme_event.dart
│   ├── theme_state.dart
├── temp_settings/
│   ├── temp_settings_bloc.dart
│   ├── temp_settings_event.dart
│   ├── temp_settings_state.dart
└── blocs.dart
```

### **Other Key Components**

- **Constants**: Global constants for API keys, URLs, etc.
    - `constants/constants.dart`

- **Models**: Data models for weather and error handling.
    - `models/custom_error.dart`
    - `models/direct_geocoding.dart`
    - `models/weather.dart`

- **Pages**: Application screens.
    - `pages/home_page.dart`
    - `pages/search_page.dart`
    - `pages/settings_page.dart`

- **Exceptions**: Handles API-specific exceptions.
    - `exceptions/weather_exception.dart`

- **Services**: Contains API and HTTP utility classes.
    - `services/http_error_handler.dart`
    - `services/weather_api_services.dart`

- **Repositories**: Manages data interactions and APIs.
    - `repositories/weather_repository.dart`

- **Widgets**: Custom reusable widgets.
    - `widgets/error_dialog.dart`

---

## Getting Started

### Prerequisites

Make sure you have the following installed:

- Flutter SDK: [Install Flutter](https://flutter.dev/docs/get-started/install)
- OpenWeatherMap API Key: Sign up at [OpenWeatherMap](https://openweathermap.org/).

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/ahmedsiddique01/simple_bloc_weather_app.git
   ```
2. Navigate to the project directory:
   ```bash
   cd weather_app
   ```
3. Get the dependencies:
   ```bash
   flutter pub get
   ```
4. Run the app:
   ```bash
   flutter run
   ```

---

## Configuration

1. Add your OpenWeatherMap API key in the `constants/constants.dart` file:
   ```dart
   const String openWeatherMapAPIKey = "your_api_key_here";
   ```

---

## Dependencies

The app uses the following packages:

- **Bloc**: For state management (`flutter_bloc`)
- **HTTP**: For API communication (`http`)
- **Equatable**: Simplifies equality checks (`equatable`)

---

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature/your-feature
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add your message here"
   ```
4. Push to your branch:
   ```bash
   git push origin feature/your-feature
   ```
5. Create a pull request.

---

## Acknowledgements

- [Flutter](https://flutter.dev/)
- [OpenWeatherMap API](https://openweathermap.org/)
- [Bloc Pattern](https://bloclibrary.dev/)

---

