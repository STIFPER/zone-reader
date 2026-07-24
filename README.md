# Zone Reader — Exposure & Dynamic Range Workbench

A premium, state-of-the-art Web application for the Ansel Adams Zone System exposure calculation. Integrates live camera light-metering and custom photo uploads to automatically compute dynamic ranges, calculate shutter speed values, and align points in real-time.

---

## ⚡ Deployment Instructions

This project is optimized and pre-configured for instant deployment on **Firebase Hosting** and tracking on **GitHub**.

### 1. GitHub Deployment (Push Code)

To push the latest code to your GitHub repository, run the following commands in your terminal:

```bash
# Initialize git repository (if not already done)
git init

# Add all files to staging (ignoring Firebase caches via .gitignore)
git add .

# Commit changes
git commit -m "feat: implement vertical mobile viewfinder, auto 3-zone metering, and satoshi font"

# Link your remote repository and push (Replace with your actual GitHub URL)
git remote add origin https://github.com/stifper/App-Zone-Reader.git
git branch -M main
git push -u origin main
```

---

### 2. Firebase Hosting Deployment

We have configured `firebase.json` and created a production-ready entrypoint at `public/index.html`. To publish the app to the web:

1. **Install Firebase CLI** (if not already installed):
   ```bash
   npm install -g firebase-tools
   ```

2. **Login to Firebase**:
   ```bash
   firebase login
   ```

3. **Initialize & Deploy**:
   ```bash
   # Select your Firebase project when prompted
   firebase init hosting
   
   # Deploy the public/ folder online
   firebase deploy
   ```

Once deployed, Firebase will provide you with a hosting URL (e.g., `https://zone-reader-app.web.app`) to access your app from any mobile phone or device!
