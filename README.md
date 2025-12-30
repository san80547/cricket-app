CricketFeed 🎥🏏

A Short-Video Social Media Web App for Cricket Content

📌 Project Overview

CricketFeed is a short-video social media web application inspired by platforms like TikTok and Instagram Reels, designed specifically for cricket-related video content.

The application allows users to sign up, log in, upload videos, like videos, comment in real time, and view an infinite scrolling video feed with autoplay functionality.
It is built using HTML, Tailwind CSS, JavaScript, and Firebase, with Cloudinary handling video storage.

🚀 Key Features

🔐 User Authentication (Login & Signup)

🎬 Upload cricket videos with descriptions

▶️ Auto-play / pause videos using Intersection Observer

❤️ Like and unlike videos (real-time)

💬 Comment system with live updates

📊 Real-time comment count updates

🗑 Delete own videos

📱 Mobile-first UI (TikTok-style vertical feed)

☁️ Cloudinary video upload with progress bar

🔄 Real-time updates using Firestore listeners

🧠 Tech Stack
Frontend

HTML5

Tailwind CSS

Vanilla JavaScript (ES6 Modules)

Backend / Cloud

Firebase Authentication – User login & signup

Firebase Firestore – Real-time database

Firebase Analytics

Cloudinary – Video hosting & streaming

🏗 Architecture Overview

Client-side rendering (single HTML file)

Firebase Authentication manages users

Firestore stores:

Videos

Likes

Comments (subcollections)

Cloudinary handles large video uploads efficiently

Real-time listeners update UI instantly

▶️ How to Run the Project
1️⃣ Clone the repository
git clone https://github.com/<your-username>/cricketfeed.git

2️⃣ Open the project

Open index.html in a browser
OR

Use a local server (recommended):

npx serve

3️⃣ Firebase Setup

This project already uses Firebase configuration.
To use your own Firebase project:

Create a Firebase project

Enable:

Authentication (Email/Password)

Firestore Database

Replace the firebaseConfig object in the script

📂 Firebase Firestore Structure
videos (collection)
 ├── videoId (document)
 │    ├── src
 │    ├── description
 │    ├── userId
 │    ├── userEmail
 │    ├── likes [array]
 │    ├── commentCount
 │    └── timestamp
 │
 │    └── comments (subcollection)
 │         ├── commentId
 │         │    ├── text
 │         │    ├── userId
 │         │    ├── userEmail
 │         │    └── timestamp

🔐 Authentication

Email & Password authentication

Only logged-in users can:

Upload videos

Like videos

Comment

Users can delete only their own videos

📈 Learning Outcomes

Real-time web apps with Firebase

Firestore subcollections & listeners

Client-side video upload with progress tracking

Responsive UI using Tailwind CSS

Authentication & authorization logic

Scalable cloud-based architecture

🚧 Future Enhancements

User profiles & avatars

Video categories / hashtags

Follow system

Search functionality

Moderation & reporting system

Backend validation (security rules)

👤 Author

Sandeep
Computer Science & Technology
Ulster University

⭐ Portfolio Note

This project demonstrates:

Full-stack web development

Cloud integration

Real-time database usage

Modern UI/UX design

Practical social media system design
