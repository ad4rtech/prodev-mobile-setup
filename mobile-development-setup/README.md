# Mobile Development Setup with Expo (React Native)

## 📌 Project Overview
This project documents the setup and testing of a mobile development environment using **React Native**, **TypeScript**, and the **Expo Framework**. The goal is to ensure readiness for cross-platform mobile development using a physical device.

---

## 🛠️ Development Environment

- **Operating System:** Windows 10
- **Node.js Version:** v18.x (LTS)
- **npm Version:** Installed with Node.js
- **IDE:** Visual Studio Code
- **Mobile Device:** Android phone
- **Expo Go Version:** Latest (installed from Play Store)

---

## 📲 Expo Go Installation Steps

1. Visited the official Expo Go website: https://expo.dev/go
2. Selected the latest SDK version.
3. Installed **Expo Go** from the Google Play Store.
4. Opened the Expo Go app on my Android device.
5. Created and logged into an Expo account successfully.

---

## 🚀 Testing the Setup

To verify the setup, I created a test Expo project using the following commands:

```bash
npx create-expo-app test-app
cd test-app
npx expo start

---

## ⚠️ Challenges & Solutions

### 📡 Expo Go Phone Connection Issue
**Challenge:**  
The Android phone was unable to connect to the Expo development server when running `npx expo start` on the laptop.

**Cause:**  
This was due to network restrictions/firewall issues on the local Wi-Fi network, which prevented the phone and laptop from communicating properly.

**Solution:**  
The issue was resolved by starting Expo using tunnel mode:

```bash
npx expo start --tunnel
