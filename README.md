# Digital Memory Capsule
## Overview
The Digital Memory Capsule is a web application that allows users to create digital time capsules containing messages,
photos, or videos that are "unlocked" after a specified time (e.g., 1 year later). It supports password-protected capsules,
a 3D capsule visualization using Three.js, and group capsules where multiple users can contribute content before the unlock date.
Features

- Create Capsules: Users can create capsules with a name, message, optional password, unlock date, and optional media (images or videos).
Password Protection: Capsules can be secured with a password, required to view contents after unlocking.
Group Capsules: Allow multiple users to contribute messages or media before the unlock date.
3D Visualization: A rotating 3D capsule model is displayed using Three.js for an engaging visual experience.
Local Storage: Capsule data, including media (as base64), is stored in the browser's localStorage for simplicity.

### Technologies Used

- HTML5: Structure of the web app.
JavaScript: Core functionality, including capsule management and Three.js integration.
Three.js: Renders a 3D rotating capsule for visualization.
Tailwind CSS: Styling for a modern, responsive UI.
localStorage: Stores capsule data locally in the browser.

### How to Use

-  a Capsule:
Enter a capsule name, message, optional password, and unlock date.
Optionally upload an image or video.
Check "Group Capsule" to allow contributions from others.
Click "Create Capsule" to save.


### View Capsules:
- Capsules are listed with their unlock dates.
If the current date is past the unlock date, click "View" to see contents (enter password if required).
For group capsules before the unlock date, click "Contribute" to add messages or media.


### 3D Visualization:
- A rotating 3D capsule is displayed at the bottom of the page.


### Contribute to Group Capsules:
- Before the unlock date, add messages or media to group capsules via the contribution form.



### Setup Instructions

Clone or Download:
Download the index.html file containing the entire application.


Run Locally:
Open index.html in a modern web browser (e.g., Chrome, Firefox).
No server is required as the app runs entirely client-side.


Dependencies:
The app uses CDN-hosted libraries:
Three.js: https://cdnjs.cloudflare.com/ajax/libs/three.js/r134/three.min.js
Tailwind CSS: https://cdn.tailwindcss.com


Ensure an internet connection for the initial load to fetch these libraries.



### Limitations

Storage: Media files are stored as base64 strings in localStorage, which has size limits (typically 5-10 MB). Large files may cause issues.
Persistence: Data is stored in the browser's localStorage and will be cleared if the user clears their browser data.
Security: Passwords are stored in plain text in localStorage. For production, use a backend with proper encryption.
Scalability: The app is client-side only. For multi-user group capsules across devices, a backend server is needed.

### Improvements

Backend Integration: Use a server to store capsule data and media, enabling cross-device access and larger file support.
User Authentication: Implement user accounts for secure access to group capsules.
Enhanced Media Support: Support larger files and more media types via cloud storage.
Improved 3D Animation: Add interactive controls to the Three.js capsule (e.g., click to open).

#### License
This project is for educational purposes and is not licensed for commercial use. Feel free to modify and experiment with the code for personal projects.
