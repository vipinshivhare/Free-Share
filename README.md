
# Free Share

A simple file sharing application that allows users to upload and share files using a unique ID. Users can upload files up to 100MB in size and retrieve them using the unique ID within a certain time frame.

---

## Overview

Free Share enables quick and secure file sharing without the need for complex setups or accounts. Simply upload a file, receive a unique ID, and share it with others to download the file.

---

## Features

- **File Upload:** Upload files up to 100MB to Firebase Storage.
- **Unique ID Generation:** Each file gets a unique 5-digit ID for retrieval.
- **File Retrieval:** Download files using the unique ID.
- **Automatic Deletion:** Files are automatically deleted from Firebase Storage 15 seconds after retrieval.
- **Drag-and-Drop Support:** Upload files by dragging them into the browser.
- **Progress Indicator:** Shows the upload progress in real-time.
- **Offline Support:** Implements a Progressive Web App (PWA) for offline functionality.

---

## How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/free-share.git
   cd free-share
   ```

2. Open the `index.html` file in your browser.

3. Alternatively, visit the deployed application [here](DEPLOYMENT_LINK).

---

## File Structure

```plaintext
free-share/
├── index.html         # Main HTML file
├── style.css          # CSS for styling
├── script.js          # JavaScript for client-side functionality
├── serviceworker.js   # Service Worker for PWA functionality
├── manifest.json      # Manifest file for PWA
├── logo/              # Folder containing logo and related assets
├── upload.png         # Upload icon
├── download.png       # Download icon
└── README.md          # Project documentation
```

---

## Firebase Configuration

Update the `firebaseConfig` object in `script.js` with your Firebase project credentials:

```javascript
const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_AUTH_DOMAIN",
  databaseURL: "YOUR_DATABASE_URL",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_STORAGE_BUCKET",
  messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
  appId: "YOUR_APP_ID",
  measurementId: "YOUR_MEASUREMENT_ID"
};
```

---

## Usage Instructions

1. **Upload a File:**

   - Click on the "Upload" button or drag a file into the browser.
   - Wait for the upload to complete and note the unique ID displayed.

2. **Download a File:**

   - Enter the unique ID in the "Receive File" section and click "Download."
   - The file will open in a new tab and be available for download.

3. **Drag-and-Drop:**

   - Drag a file into the "Drop Here" area to upload directly.

---

## Limitations

- **File Size:** Maximum file size is 100MB.
- **Retention Period:** Files are deleted 15 seconds after download.
- **Unique ID Conflicts:** Rare conflicts may occur if multiple IDs are generated simultaneously.

---

## Contribution

Feel free to fork this repository and submit pull requests with improvements or new features. Ensure your changes are well-documented and tested.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

---

## Deployment Link

Add your deployment link here: https\://sharefile-804.firebaseapp.com

