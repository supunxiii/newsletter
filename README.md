## Overview

This is a news newsletter application developed as an Android mobile application. Newsletter is a simple yet effective platform for displaying breaking news articles with rich content including headlines, images, and detailed descriptions. The application demonstrates modern Android development practices and provides users with an intuitive interface for consuming news content.

![Android](https://img.shields.io/badge/Android-3DDC84?style=flat-square&logo=android&logoColor=white)
![Java 8](https://img.shields.io/badge/Java-8-007396?style=flat-square&logo=java&logoColor=white)
![Android SDK 33](https://img.shields.io/badge/Android%20SDK-33-3DDC84?style=flat-square&logo=android&logoColor=white)
![Gradle 7.4.2](https://img.shields.io/badge/Gradle-7.4.2-02303A?style=flat-square&logo=gradle&logoColor=white)
![Material Design](https://img.shields.io/badge/Material%20Design-1.8.0-757575?style=flat-square&logo=material-design&logoColor=white)

## Features

The Newsletter Android application offers the following features:

1. **Breaking News Display**

   - Prominent "Breaking News" label for immediate attention
   - Eye-catching red badge to highlight important updates
   - Monospace font styling for distinctive presentation

2. **Article Headlines**

   - Large, readable headline text (34sp font size)
   - Clear visual hierarchy for easy scanning
   - Responsive layout adapting to different screen sizes

3. **Rich Media Support**

   - High-quality image integration within articles
   - Optimised image display with proper sizing and constraints
   - Visual content to enhance article engagement

4. **Detailed Article Content**

   - Comprehensive article descriptions and full text
   - Clean, readable typography for extended reading
   - Proper text formatting and spacing

5. **Modern Android UI**
   - Material Design principles implementation
   - ConstraintLayout for flexible, responsive layouts
   - Consistent theming and colour schemes
   - Support for both light and dark themes

## Technologies Used

- **Java 8**: Primary programming language for Android development
  - Source and target compatibility with Java 8 features
  - Object-oriented programming principles
- **Android SDK 33**: Latest Android development framework
  - Compile SDK: API Level 33 (Android 13)
  - Minimum SDK: API Level 30 (Android 11)
  - Target SDK: API Level 33 (Android 13)
- **Gradle 7.4.2**: Build automation and dependency management
  - Android Gradle Plugin version 7.4.2
  - Automated build processes and configurations
- **AndroidX Libraries**:
  - AppCompat 1.6.1: Backward compatibility support
  - Material Components 1.8.0: Material Design UI components
  - ConstraintLayout 2.1.4: Advanced layout management
- **Testing Frameworks**:
  - JUnit 4.13.2: Unit testing framework
  - AndroidX Test Ext JUnit 1.1.5: Android instrumentation testing
  - Espresso Core 3.5.1: UI testing automation

## Project Specifications

- **Platform**: Android Mobile Application
- **Programming Language**: Java
- **Minimum Android Version**: Android 11 (API 30)
- **Target Android Version**: Android 13 (API 33)
- **Application ID**: com.example.newsletter_new
- **Version**: 1.0 (Version Code: 1)
- **Build System**: Gradle with Android plugins

## User Interfaces

### UI

![Homepage Screenshot](https://github.com/supunxiii/supunxiii/blob/7653f59dcf38771e7791a1cc0795c9d6b4cdcd3c/user-interfaces/news-letter/newsletter-ui-1.png)

## Getting Started

To run the Newsletter Android application locally, follow these steps:

1. **Prerequisites**:

   - Install [Android Studio](https://developer.android.com/studio) (Arctic Fox or later recommended)
   - Ensure Java Development Kit (JDK) 8 or higher is installed
   - Set up an Android Virtual Device (AVD) or connect a physical Android device

2. Clone the repository:

   ```shell
   git clone https://github.com/your-username/newsletter.git
   ```

3. Navigate to the project directory:

   ```shell
   cd newsletter
   ```

4. Open the project in Android Studio:

   - Launch Android Studio
   - Select "Open an Existing Project"
   - Navigate to the cloned repository directory
   - Click "OK" to open the project

5. Sync the project with Gradle:

   - Android Studio should automatically prompt to sync
   - If not, click "File" → "Sync Project with Gradle Files"
   - Wait for the sync to complete

6. Run the application:

   - Select your target device (emulator or physical device)
   - Click the "Run" button (green play icon) or press `Shift + F10`
   - The application will build and install on your selected device

7. Alternative: Build from command line:

   ```shell
   # On macOS/Linux
   ./gradlew assembleDebug

   # On Windows
   gradlew.bat assembleDebug
   ```

   The APK will be generated in `app/build/outputs/apk/debug/`

## Project Structure

```
newsletter/
├── .gradle/                          # Gradle cache and build files
├── .idea/                            # Android Studio IDE configurations
├── app/                              # Main application module
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/example/newsletter_new/
│   │   │   │   └── MainActivity.java            # Main activity class
│   │   │   ├── res/
│   │   │   │   ├── drawable/                    # Drawable resources
│   │   │   │   ├── layout/
│   │   │   │   │   └── activity_main.xml        # Main layout file
│   │   │   │   ├── mipmap-*/                    # App icons
│   │   │   │   ├── values/
│   │   │   │   │   ├── colors.xml               # Colour definitions
│   │   │   │   │   ├── strings.xml              # String resources
│   │   │   │   │   └── themes.xml               # App themes
│   │   │   │   ├── values-night/
│   │   │   │   │   └── themes.xml               # Dark theme
│   │   │   │   └── xml/                         # XML configurations
│   │   │   └── AndroidManifest.xml              # App manifest
│   │   ├── androidTest/                         # Instrumented tests
│   │   └── test/                                # Unit tests
│   ├── build.gradle                             # App-level build config
│   └── proguard-rules.pro                       # ProGuard rules
├── gradle/                                      # Gradle wrapper files
│   └── wrapper/
├── build.gradle                                 # Project-level build config
├── gradle.properties                            # Gradle properties
├── gradlew                                      # Gradle wrapper script (Unix)
├── gradlew.bat                                  # Gradle wrapper script (Windows)
├── settings.gradle                              # Project settings
└── README.md                                    # This file
```

## Development Guidelines

### Building the Application

To build the project in different configurations:

```shell
# Debug build
./gradlew assembleDebug

# Release build (requires signing configuration)
./gradlew assembleRelease

# Clean and rebuild
./gradlew clean assembleDebug
```

### Running Tests

```shell
# Run unit tests
./gradlew test

# Run instrumented tests (requires connected device/emulator)
./gradlew connectedAndroidTest

# Run all tests
./gradlew testDebug connectedAndroidTest
```

## Contributors

This project was developed by:

- **Supun Wijesooriya** - Developer

## Contributing

Contributions to the Newsletter application are welcome! If you would like to contribute, please follow these steps:

1. Fork the repository.

2. Create a new branch:

   ```shell
   git checkout -b feature/your-feature-name
   ```

3. Make your changes and commit them:

   ```shell
   git commit -m "Add your commit message"
   ```

4. Push your changes to your forked repository:

   ```shell
   git push origin feature/your-feature-name
   ```

5. Open a pull request to the main repository, describing your changes and the purpose of the pull request.

## Important Notes

- This application requires **Android 11 (API 30) or higher** to run
- The application is optimised for mobile devices running Android 11–13
- Currently displays sample content; can be extended with real-time news API integration
- Material Design components ensure consistent UI across different Android devices
- ProGuard rules are included for code optimisation in release builds

## Future Enhancements

Potential improvements for future versions:

- Integration with news APIs (e.g., NewsAPI, Google News API)
- Multiple article support with scrollable list
- Category-based news filtering
- Bookmark and save functionality
- Share articles via social media
- Push notifications for breaking news
- User preferences and personalisation
- Offline reading mode with local caching

## Contact

For any enquiries or feedback, please contact the development team:

- **Supun Wijesooriya**: [GitHub Profile](https://github.com/supunxiii)
- **Project Repository**: [newsletter](https://github.com/supunxiii/newsletter)

---
**Note:** This is a beginner-friendly programme designed to understand Android native application development. The project covers fundamental concepts including Activity lifecycle management, ConstraintLayout implementation, XML-based UI design, resource management (drawables, strings, themes), Material Design principles, and AndroidX library integration.
