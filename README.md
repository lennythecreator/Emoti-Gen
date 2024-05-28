# Emoti-Gen

## Overview
Emoti-Gen is an innovative AI chat application designed to understand and engage in conversations using African American Vernacular English (AAVE). By leveraging advanced natural language processing (NLP) technologies, Emoti-Gen aims to provide an inclusive and authentic conversational experience for users who communicate using AAVE.

## Features

- **AAVE Understanding**: Emoti-Gen is trained to understand and respond accurately to AAVE, making it one of the few chat applications tailored to this unique linguistic style.
- **Emotional Intelligence**: The app can detect and appropriately respond to a range of emotions, providing empathetic and contextually relevant replies.
- **Real-time Conversations**: Enjoy smooth, real-time interactions with the AI, simulating a natural conversation flow.
- **Customization**: Users can customize the chatbot's personality to better suit their preferences and needs.
- **Privacy**: Emoti-Gen is designed with user privacy in mind, ensuring all conversations are secure and confidential.

## Tech Stack

- **Frontend**: React Native
- **Backend**: Firebase (Authentication, Firestore, Functions)
- **AI/NLP**: Custom AI models integrated with the app

## Installation

### Prerequisites

- Ensure you have the latest version of [Node.js](https://nodejs.org/) installed.
- Install [Expo CLI](https://docs.expo.dev/get-started/installation/) for React Native development.
- An internet connection for accessing Firebase services and AI models.

### Steps

1. **Clone the Repository**

   ```bash
   git clone https://github.com/yourusername/emoti-gen.git


2. **Navigate to the Project Directory**

   ```bash
   cd emoti-gen

3. **Install Dependencies**

   ```bash
   npm install
4. **Set Up Firebase**
   ```bash
   // firebaseConfig.js
   import firebase from 'firebase/app';
   import 'firebase/auth';
   import 'firebase/firestore';
   
   const firebaseConfig = {
     apiKey: "YOUR_API_KEY",
     authDomain: "YOUR_AUTH_DOMAIN",
     projectId: "YOUR_PROJECT_ID",
     storageBucket: "YOUR_STORAGE_BUCKET",
     messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
     appId: "YOUR_APP_ID",
   };
   
   if (!firebase.apps.length) {
     firebase.initializeApp(firebaseConfig);
   }
   
   export { firebase };
5. **Run the Application**
   ```bash
   npm run web


