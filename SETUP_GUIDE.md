# Flutter Student Finance App - Setup Guide

## Project Overview
This is a complete Flutter UI Assignment project implementing **Pages 1, 3, and 4** based on the Figma design.

### Implemented Pages
- **Page 1 (Dashboard)**: Total balance display, quick action buttons, and recent transactions list
- **Page 3 (My Cards)**: Bank card display with linked accounts section
- **Page 4 (User Profile)**: Student profile information with editable fields

### Student Information
Replace the following with your own details:
- **Student Name**: SAYEED JAHIN ABID SAMIN
- **Student ID**: S12345 (YOUR ID HERE)
- **Email**: student.name@iub.edu (YOUR IUB EMAIL HERE)
- **Bio/Story**: Update with your own bio in the profile page

## Running the App

### Prerequisites
- Flutter SDK (3.11.4 or higher) - Already installed at `D:\Sam\FlutterSDK\flutter`
- Android Studio (for Android emulator) - Located at `C:\Program Files\Android\Android Studio`
- Java Development Kit (JDK)

### Option 1: Run on Windows Desktop (Currently Active)
The app is currently running on Windows Desktop. You can interact with it and test the navigation.

```bash
flutter run -d windows
```

### Option 2: Run on Android Emulator (Recommended for Assignment Submission)

#### Step 1: Create an Android Virtual Device (AVD)
1. Open Android Studio
2. Go to: **Tools → Device Manager → Create Virtual Device**
3. Select a device (e.g., Pixel 5)
4. Select API Level (minimum API 21)
5. Click **Finish**

#### Step 2: Start the Emulator
```bash
# List available emulators
flutter emulators

# Start a specific emulator (replace with your AVD name)
flutter emulators --launch Pixel_5_API_30
```

#### Step 3: Run Flutter App on Android
```bash
cd D:\Sam\MobileApp\assignment-two-flutter_UI-SayeedJahinAbidSamin-2222114
flutter run
```

### Option 3: Run on Physical Android Device
1. Enable Developer Mode on your Android device
2. Connect via USB cable
3. Run: `flutter run`

## Navigation Structure
The app uses **PageView with PageController** for navigation:

```
Bottom Navigation Bar
├── Home (Page 1) - Dashboard
├── Cards (Page 3) - My Cards
└── Profile (Page 4) - User Profile
```

**Page Index Mapping:**
- `_currentPage = 0` → Page 1 (Home)
- `_currentPage = 1` → Page 3 (Cards)
- `_currentPage = 2` → Page 4 (Profile)

## Key Features Implemented

### Page 1 - Dashboard
- **Balance Card**: Displays total balance ($8,945.32) with gradient background
- **Quick Actions**: Transfer, Pay Bills, Invest buttons
- **Recent Transactions**: List of 5 sample transactions with icons and amounts

### Page 3 - My Cards
- **Credit Card Display**: Dark card with cardholder info
- **Card Actions**: Block, Details, Limit buttons
- **Linked Accounts**: Shared Savings account display
- **Add Account**: Button to add new accounts

### Page 4 - User Profile
- **Profile Avatar**: Large circular avatar with initials
- **User Details**: Name, Student ID, Email, Bio fields
- **Action Buttons**: Edit Profile and Logout buttons
- **Responsive Layout**: Works on various screen sizes

## Hot Reload & Development
While the app is running, you can:
- Press `r` for Hot Reload (fast reload of code)
- Press `R` for Hot Restart (full restart)
- Press `q` to quit the app

## File Structure
```
lib/
├── main.dart          # Main app file with all pages and navigation
pubspec.yaml          # Project dependencies
android/              # Android-specific configuration
ios/                  # iOS-specific configuration
windows/              # Windows desktop configuration
```

## Customization Instructions

### Replace Student Information
Edit `lib/main.dart` and search for:
- `SAYEED JAHIN ABID SAMIN` → Replace with your full name
- `S12345` → Replace with your student ID
- `student.name@iub.edu` → Replace with your IUB email
- Bio text section → Add your own story/bio

### Modify Colors
The app uses `Colors.blue.shade700` as primary color. To change:
1. Open `lib/main.dart`
2. Replace `Colors.blue.shade700` with your preferred color
3. Save and hot reload with `r`

## Troubleshooting

### "Unable to locate Android SDK"
```bash
# Set Android SDK path
flutter config --android-sdk "C:\Program Files\Android\Sdk"
```

### Emulator Not Starting
1. Check if virtualization is enabled in BIOS
2. Ensure you have sufficient disk space (at least 10GB)
3. Try: `emulator -avd YourAVDName -writable-system`

### Build Errors
```bash
# Clean build and try again
flutter clean
flutter pub get
flutter run
```

### Port Already in Use
If you get "address already in use" error:
```bash
# Find process using the port and kill it, or
flutter run --local-engine-src-path=<path>
```

## Recording App Demo Video
For assignment submission:

1. **On Android Emulator**:
   ```bash
   # Use Android Studio's built-in recorder or
   ffmpeg -f gdigrab -i desktop output.mp4
   ```

2. **Mobile Device Screen Recording**:
   - Android: Use built-in screen recorder or scrcpy
   - iPhone: Use built-in screen recording

3. **Video Requirements**:
   - Show all 3 implemented pages
   - Demonstrate navigation between pages
   - Show any interactive features
   - Duration: 1-2 minutes
   - Do NOT upload to GitHub (only submit in Google Classroom)

## Submission Checklist

- [ ] Replace all "STUDENT NAME" with actual name
- [ ] Replace Student ID with your IUB ID
- [ ] Replace email with your IUB email
- [ ] Add personal bio/story
- [ ] Test all 3 pages work correctly
- [ ] Test navigation between pages works
- [ ] Record demo video
- [ ] Create GitHub repository: `assignment-two-flutter_UI-YourName-YourID`
- [ ] Upload full Flutter project to GitHub (mark as Public)
- [ ] Upload demo video to Google Classroom
- [ ] Do NOT include demo video in GitHub repository

## GitHub Repository Setup
```bash
# In the project directory
git init
git add .
git commit -m "Initial Flutter UI project - Pages 1, 3, 4"
git branch -M main
git remote add origin https://github.com/YourUsername/assignment-two-flutter_UI-Name-ID.git
git push -u origin main
```

## Resources
- [Flutter Documentation](https://flutter.dev)
- [Material Design Guidelines](https://material.io/design)
- [Figma Design](https://www.figma.com/board/yUTvnb1M94dG5hUgM0jCPX/Assignment-2---Flutter-APP-UI)
- [PageView Widget](https://api.flutter.dev/flutter/widgets/PageView-class.html)
- [PageController Widget](https://api.flutter.dev/flutter/widgets/PageController-class.html)

## Support
If you encounter any issues:
1. Check Flutter installation: `flutter doctor`
2. Check internet connection
3. Try clearing cache: `flutter clean`
4. Check for Java installation: `java -version`
5. Ensure Android SDK is properly configured

---
**Last Updated**: April 9, 2026
**Flutter Version**: 3.41.6
**Dart Version**: 3.11.4
