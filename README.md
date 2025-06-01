# Welcome to E-Checker app 👋

This is an [Expo](https://expo.dev) project created with [`create-expo-app`](https://www.npmjs.com/package/create-expo-app).

## Get started

1. Install dependencies

   ```bash
   npm install
   ```

2. Start the app

   ```bash
   npx expo start
   ```

In the output, you'll find options to open the app in a

- [development build](https://docs.expo.dev/develop/development-builds/introduction/)
- [Android emulator](https://docs.expo.dev/workflow/android-studio-emulator/)
- [iOS simulator](https://docs.expo.dev/workflow/ios-simulator/)
- [Expo Go](https://expo.dev/go), a limited sandbox for trying out app development with Expo

You can start developing by editing the files inside the **app** directory. This project uses [file-based routing](https://docs.expo.dev/router/introduction).

### FrontEnd Architecture
SmartCheckApp/
│
├── app/
│   ├── assets/                # Images, fonts, icons
│   ├── components/           # Reusable UI components (e.g., Button, Card, InputField)
│   ├── navigation/           # Navigation stack, tabs, route config
│   │   └── AppNavigator.js
│   ├── screens/              # Feature-based screens
│   │   ├── Auth/
│   │   │   ├── LoginScreen.js
│   │   │   └── RegisterScreen.js
│   │   ├── Outage/
│   │   │   ├── ReportOutage.js
│   │   │   └── OutageStatus.js
│   │   ├── Meter/
│   │   │   └── MeterReading.js
│   │   ├── Billing/
│   │   │   └── BillingDetails.js
│   │   └── Notifications/
│   │       └── Notification.js
│   ├── services/             # API calls and integrations (Axios instance, API calls)
│   │   └── api.js
│   ├── store/                # Redux or Context API (state management)
│   │   ├── actions/
│   │   ├── reducers/
│   │   └── store.js
│   ├── utils/                # Helper functions (validators, formatters, etc.)
│   └── config/               # App config (environment variables, base URLs)
│
├── .env                      # Environment variables (API keys, URLs)
├── App.js                    # App entry point
├── package.json              # Project dependencies and scripts
└── README.md                 # Project overview and setup guide

