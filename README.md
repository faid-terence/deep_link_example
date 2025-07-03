# Flutter Deep Links Example App with GoRouter

A complete Flutter app demonstrating deep linking implementation using [GoRouter](https://pub.dev/packages/go_router).

This example shows how to create seamless deep links that take users directly to specific content in your Flutter app - no hunting through menus required!

## ✨ Features

- **Cross-platform deep linking** (Android & iOS)
- **HTTPS links** with domain verification
- **Authentication guards** with redirect handling
- **Graceful error handling** for missing content
- **Professional URL structure**
- **Real-world testing examples**

## 🚀 What You'll Learn

- Setting up Android App Links and iOS Universal Links
- Implementing GoRouter for deep link navigation
- Creating authentication guards and redirects
- Handling edge cases (missing content, network errors)
- Testing deep links on real devices

## 📱 App Flow

The example app demonstrates a typical event browsing experience:

### Normal Navigation Flow

![Home Screen](https://res.cloudinary.com/faid-terence/image/upload/v1751542524/Simulator_Screenshot_-_iPhone_16_Pro_-_2025-07-03_at_00.26.19_qafss6.png)

Users start at the home screen and navigate through the events list:

![Events List](https://res.cloudinary.com/faid-terence/image/upload/v1751542527/Simulator_Screenshot_-_iPhone_16_Pro_-_2025-07-03_at_00.26.49_avuzmj.png)

### Deep Link Magic ✨

Watch the power of deep linking in action:

**1. User enters deep link in browser:**
![Browser URL](https://res.cloudinary.com/faid-terence/image/upload/v1751542857/Simulator_Screenshot_-_iPhone_16_Pro_-_2025-07-03_at_13.40.29_mj8z4k.png)

**2. iOS requests permission to open in app:**
![Permission Request](https://res.cloudinary.com/faid-terence/image/upload/v1751542524/Simulator_Screenshot_-_iPhone_16_Pro_-_2025-07-03_at_00.30.22_jumtm4.png)

**3. User lands directly on the target screen:**
![Direct Navigation](https://res.cloudinary.com/faid-terence/image/upload/v1751542526/Simulator_Screenshot_-_iPhone_16_Pro_-_2025-07-03_at_00.29.11_mvvm0n.png)

No navigation required - instant access to the exact content!

## 📖 Complete Tutorial

For detailed implementation steps, setup instructions, and best practices, read the full article:

**[Flutter Deep Linking: Create Links That Actually Work](https://dev.to/faidterence/flutter-deep-linking-create-links-that-actually-work-3l2b)**

## 🛠️ Quick Start

1. **Clone the repository**

   ```bash
   git clone https://github.com/faid-terence/deep_link_example.git
   cd deep_link_example
   ```

2. **Install dependencies**

   ```bash
   flutter pub get
   ```

3. **Run the app**

   ```bash
   flutter run
   ```

4. **Test deep links**

   **Android:**

   ```bash
   adb shell am start -a android.intent.action.VIEW \
     -c android.intent.category.BROWSABLE \
     -d "https://yourapp.com/event/flutter-conference" \
     com.example.yourapp
   ```

   **iOS:**

   ```bash
   xcrun simctl openurl booted "https://yourapp.com/event/flutter-conference"
   ```

## 🔧 Configuration

### Android Setup

- Configure App Links in `android/app/src/main/AndroidManifest.xml`
- Add domain verification with `assetlinks.json`
- Test with ADB commands

### iOS Setup

- Add Associated Domains capability
- Create `apple-app-site-association` file
- Test with iOS Simulator

Full setup instructions are in the [tutorial article](https://dev.to/faidterence/flutter-deep-linking-create-links-that-actually-work-3l2b).

## 🎯 Key Concepts Demonstrated

- **URL Structure Design** - Clean, shareable URLs
- **Authentication Guards** - Protect sensitive content
- **Error Handling** - Graceful fallbacks for missing content
- **Cross-Platform Support** - Works on both Android and iOS
- **Real-World Testing** - Practical testing approaches

## 💻 Implementation

This example demonstrates deep linking implementation in a single `main.dart` file, making it easy to understand and follow along. The code shows:

- GoRouter setup with multiple routes
- Authentication guards and redirects
- Error handling for missing content
- Cross-platform deep link configuration

## 🤝 Contributing

Found a bug or want to improve the example? Contributions are welcome!

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## 💡 More Flutter Resources

- [Flutter Documentation](https://docs.flutter.dev/)
- [GoRouter Package](https://pub.dev/packages/go_router)
- [Android App Links Guide](https://developer.android.com/training/app-links)
- [iOS Universal Links Guide](https://developer.apple.com/ios/universal-links/)

---
