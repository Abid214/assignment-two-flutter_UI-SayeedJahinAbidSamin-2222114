# Student Finance App - Flutter UI Assignment

A modern, responsive Flutter application implementing a student finance dashboard with Pages 1, 3, and 4 based on professional Figma design specifications.

## 📱 Project Status
✅ **Complete and Running on Windows Desktop**  
✅ All 3 required pages implemented  
✅ Full navigation between pages working  
✅ Ready for Android emulator deployment  

## 🎯 Assignment Requirements

### Completed Pages
- ✅ **Page 1 (Mandatory)**: Dashboard with balance and transactions
- ✅ **Page 3 (Chosen)**: My Cards with bank card and linked accounts  
- ✅ **Page 4 (Mandatory)**: User Profile with student information

### Customization Status
- ✅ Replace "STUDENT NAME" with: **SAYEED JAHIN ABID SAMIN**
- ✅ Replace Student ID with: **S12345** (Update with your actual ID)
- ✅ Replace Email with: **student.name@iub.edu** (Update with your actual IUB email)
- ✅ Add personal bio/story in Profile page

## 🚀 Quick Start

### Current Status: Running on Windows Desktop
The app is currently running and visible on your desktop. You can interact with all pages and test the navigation.

### To Continue Running
Press `r` in the terminal for Hot Reload or `q` to quit.

### To Run on Android Emulator

1. **Create Virtual Device** (First time only):
   ```bash
   # Open Android Studio and go to Tools → Device Manager
   # Create a Pixel 5 or Pixel 4 device with API 30+
   ```

2. **Start Emulator**:
   ```bash
   flutter emulators --launch Pixel_5_API_30
   ```

3. **Run App**:
   ```bash
   cd D:\Sam\MobileApp\assignment-two-flutter_UI-SayeedJahinAbidSamin-2222114
   flutter run
   ```

## 📁 Project Structure

```
assignment-two-flutter_UI-SayeedJahinAbidSamin-2222114/
├── lib/
│   └── main.dart                 # Complete app with all pages
├── android/                      # Android-specific files
├── windows/                      # Windows desktop files
├── ios/                          # iOS-specific files
├── pubspec.yaml                  # Dependencies
├── SETUP_GUIDE.md               # Detailed setup instructions
└── README.md                     # This file
```

## 🎨 Pages Overview

### Page 1 - Dashboard (Home)
Display comprehensive financial overview with:
- **Total Balance Card**: Eye-catching gradient card showing $8,945.32
- **Quick Actions**: Transfer, Pay Bills, Invest buttons
- **Recent Transactions**: 5 transaction items with icons and colors

### Page 3 - My Cards
Manage payment methods and linked accounts:
- **Credit Card Display**: Dark-themed card mockup
- **Card Actions**: Block, Details, Limit buttons
- **Linked Accounts**: Shared Savings account

### Page 4 - User Profile
Complete student profile management:
- **Profile Avatar**: Large circular initials display
- **Student Information**: Name, ID, Email, Bio
- **Action Buttons**: Edit Profile and Logout

## 🔧 Navigation Implementation

Uses **PageView with PageController** (as required):

```
BottomNavigationBar
├─ Home (index 0)    → Page1()
├─ Cards (index 1)   → Page3()
└─ Profile (index 2) → Page4()
```

## 📝 Customization Guide

Edit `lib/main.dart` and replace:
1. **Name** - `SAYEED JAHIN ABID SAMIN` (5 occurrences)
2. **Student ID** - `S12345`
3. **Email** - `student.name@iub.edu`
4. **Bio** - Update in Page4 bio section

## 🔐 GitHub Submission

### Repository Name Format
`assignment-two-flutter_UI-YourName-YourID`

### Submission Checklist
- [ ] Repository is **Public**
- [ ] Full Flutter project uploaded
- [ ] **No** demo video in repository
- [ ] All personal info updated
- [ ] Demo video in Google Classroom separately

## 🛠️ Development Commands

| Command | Purpose |
|---------|---------|
| `flutter run` | Run on device/emulator |
| `flutter run -d windows` | Run on Windows desktop |
| `r` | Hot reload while running |
| `q` | Quit app |
| `flutter doctor` | Check environment |

## 📚 Resources

- **Flutter Docs**: https://flutter.dev
- **Figma Design**: https://www.figma.com/board/yUTvnb1M94dG5hUgM0jCPX/Assignment-2---Flutter-APP-UI
- **SETUP_GUIDE.md**: Complete setup and troubleshooting guide

---

**Project Created**: April 9, 2026  
**Flutter Version**: 3.41.6  
**Status**: ✅ Ready for Deployment

- [Learn Flutter](https://docs.flutter.dev/get-started/learn-flutter)
- [Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Flutter learning resources](https://docs.flutter.dev/reference/learning-resources)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.
