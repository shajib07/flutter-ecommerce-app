# 🛍️ Flutter E-Commerce Application

A modern, feature-rich e-commerce mobile application built with Flutter and BLoC architecture. This app provides a complete shopping experience with authentication, product browsing, cart management, and user profiles.

![Flutter](https://img.shields.io/badge/Flutter-3.5.0-blue?style=for-the-badge&logo=flutter)
![Dart](https://img.shields.io/badge/Dart-3.0.0-blue?style=for-the-badge&logo=dart)
![BLoC](https://img.shields.io/badge/BLoC-8.1.4-purple?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

## ✨ Features

- 🔐 **User Authentication** - Secure login and registration system
- 📱 **Product Catalog** - Browse products with categories and search
- 🛒 **Shopping Cart** - Add, remove, and manage cart items
- 👤 **User Profile** - Personal information and order history
- 🌙 **Dark/Light Theme** - Material 3 design with theme switching
- 📊 **State Management** - BLoC pattern for predictable state
- 🌐 **API Integration** - RESTful API with DummyJSON
- 📱 **Cross-Platform** - iOS, Android, Web, Desktop support
- 🧪 **Comprehensive Testing** - Unit and widget tests
- 🔄 **Real-time Updates** - Live cart and product updates

## 🏗️ Architecture

This application follows **Clean Architecture** principles with **Feature-Driven Development**:

```
lib/
├── config/          # App configuration
├── core/            # Core utilities and services
├── features/        # Feature modules
│   ├── auth/        # Authentication feature
│   ├── products/    # Products feature
│   ├── cart/        # Shopping cart feature
│   ├── profile/     # User profile feature
│   └── splash/      # Splash screen feature
└── main.dart        # App entry point
```

### Architecture Layers:
- **Presentation Layer**: UI components, BLoCs, and pages
- **Domain Layer**: Business logic and repositories
- **Data Layer**: Models, repositories, and API services

## 🚀 Getting Started

### Prerequisites

- **Flutter SDK**: 3.5.0 or higher
- **Dart**: 3.0.0 or higher
- **Android Studio** / **VS Code**
- **Git**

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/shajib07/flutter-ecommerce-app.git
   cd flutter-ecommerce-app
   ```

2. **Install dependencies**
   ```bash
   flutter pub get
   ```

3. **Run the application**
   ```bash
   flutter run
   ```

### Platform Support

- ✅ **Android** (API 21+)
- ✅ **iOS** (12.0+)
- ✅ **Web**
- ✅ **macOS**
- ✅ **Linux**
- ✅ **Windows**

## 📦 Dependencies

### Core Dependencies
```yaml
# State Management
flutter_bloc: ^8.1.4
equatable: ^2.0.5

# Network
dio: ^5.4.1
pretty_dio_logger: ^1.3.1

# Local Storage
shared_preferences: ^2.2.2

# UI Components
cached_network_image: ^3.3.1
flutter_svg: ^2.0.10+1
shimmer: ^3.0.0

# Utils
intl: ^0.19.0
logger: ^2.0.2+1
```

### Development Dependencies
```yaml
flutter_lints: ^4.0.0
mockito: ^5.4.4
build_runner: ^2.4.8
bloc_test: ^9.1.6
```

## 🧪 Testing

### Run Tests
```bash
# Run all tests
flutter test

# Run tests with coverage
flutter test --coverage

# Generate mock files
flutter packages pub run build_runner build
```

### Test Structure
```
test/
├── features/
│   ├── cart/
│   │   └── presentation/bloc/cart_bloc_test.dart
│   └── products/
│       ├── data/repositories/product_repository_test.dart
│       └── presentation/bloc/products_bloc_test.dart
└── widget_test.dart
```

## 🏗️ Project Structure

```
ecommerce_app/
├── android/                 # Android platform code
├── ios/                    # iOS platform code
├── lib/                    # Main Dart code
│   ├── config/            # App configuration
│   │   ├── app_routes.dart
│   │   └── app_theme.dart
│   ├── core/              # Core utilities
│   │   └── network/
│   │       └── api_service.dart
│   ├── features/          # Feature modules
│   │   ├── auth/          # Authentication
│   │   ├── products/      # Products
│   │   ├── cart/          # Shopping cart
│   │   ├── profile/       # User profile
│   │   └── splash/        # Splash screen
│   └── main.dart
├── test/                   # Test files
├── web/                    # Web platform
├── windows/                # Windows platform
├── linux/                  # Linux platform
├── macos/                  # macOS platform
└── pubspec.yaml           # Dependencies
```

## 🔧 Configuration

### Environment Setup
- **API Base URL**: `https://dummyjson.com`
- **Flutter SDK**: `^3.5.0`
- **Target Platforms**: Android, iOS, Web, macOS, Linux, Windows

### Build Configuration
- **Android**: Minimum SDK 21, Target SDK 34
- **iOS**: Deployment Target 12.0
- **Web**: Modern browsers with ES6 support

## 🚀 Deployment

### Android
```bash
# Build APK
flutter build apk --release

# Build App Bundle
flutter build appbundle --release
```

### iOS
```bash
# Build iOS App
flutter build ios --release
```

### Web
```bash
# Build Web App
flutter build web --release
```

## 📱 Screenshots

*[Add screenshots of your app here]*

## 🔌 API Endpoints

The application integrates with the DummyJSON API:

- **Base URL**: `https://dummyjson.com`
- **Authentication**: `POST /auth/login`
- **Products**: `GET /products`
- **Product Details**: `GET /products/{id}`
- **Categories**: `GET /products/categories`
- **Products by Category**: `GET /products/category/{category}`

## 🤝 Contributing

1. **Fork the repository**
2. **Create a feature branch**
   ```bash
   git checkout -b feature/amazing-feature
   ```
3. **Commit your changes**
   ```bash
   git commit -m 'Add some amazing feature'
   ```
4. **Push to the branch**
   ```bash
   git push origin feature/amazing-feature
   ```
5. **Open a Pull Request**

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Md Atahar Hossain (shajib07)**

- GitHub: [@shajib07](https://github.com/shajib07)
- LinkedIn: [Your LinkedIn]
- Email: [Your Email]

## 🙏 Acknowledgments

- [Flutter Team](https://flutter.dev/) for the amazing framework
- [BLoC Library](https://bloclibrary.dev/) for state management
- [DummyJSON](https://dummyjson.com/) for the API
- [Material Design](https://material.io/) for design guidelines

## 📞 Support

If you have any questions or need help, please:

1. Check the [Issues](https://github.com/shajib07/flutter-ecommerce-app/issues) page
2. Create a new issue if your problem isn't already listed
3. Contact the author directly

---

⭐ **Star this repository if you found it helpful!**