# 📱 First Mobile App with Expo Router

## 🎯 Objective

Set up the first mobile application using the Expo Router template.  
Understand the scaffolding process, modify the home screen, and observe the effects of resetting the project.

---

## 📂 Project Setup

### 1. Navigate to Project Directory

```bash
cd prodev-mobile-setup
mkdir prodev-mobile-app-0x00
cd prodev-mobile-app-0x00
2. Initialize Project with Expo Router Template
npx create-expo-app@latest .


Selected the Expo Router template.

Waited for dependencies to install successfully.

3. Modify the Home Screen

Opened:

app/(tabs)/index.tsx


Found the default text:

Welcome!


Replaced it with:

First App Created

▶️ Running the App

Started the development server with:

npx expo start


Android → Scanned the QR code in the Expo Go app.

iOS → Can scan QR code using the Camera app.

Verified that the app loaded successfully and displayed:
“First App Created” 🎉

🔄 Resetting the Project

Ran the reset command:

npm run reset-project

Observations

Prompted:

Do you want to move existing files to /app-example instead of deleting them? (Y/n):


→ Selected Y to preserve old files.

Script output:

/app-example directory created.

/components moved to /app-example/components.

/hooks moved to /app-example/hooks.

/scripts moved to /app-example/scripts.

New /app directory created with fresh files:

app/index.tsx

app/_layout.tsx

Final confirmation message:

✅ Project reset complete.


Effect: The project was cleaned, caches reset, and a new Expo Router structure was generated while the original files were safely stored in /app-example.

📂 Final Directory Structure
prodev-mobile-setup/
└── prodev-mobile-app-0x00/
    ├── README.md
    ├── app/
    │   ├── index.tsx
    │   ├── _layout.tsx
    ├── app-example/
    │   ├── app/(tabs)/index.tsx
    │   ├── constants/Colors.tsx
    │   ├── components/
    │   ├── hooks/
    │   └── scripts/
    ├── package.json
    └── scripts/reset-project.js

🚧 Challenges Faced

Encountered a Windows EPERM (operation not permitted) error when the app folder was open in VS Code or Metro bundler was running.

✅ Fixed by closing VS Code/File Explorer, stopping Metro bundler, then rerunning the reset.

After resolving, the reset script worked as expected.

✅ Conclusion

Successfully scaffolded a React Native project using Expo Router.

Modified and tested the home screen on a physical device with Expo Go.

Understood how the reset-project script preserves old files into /app-example and regenerates a fresh /app for clean development.
```
