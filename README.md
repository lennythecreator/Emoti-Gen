# EmotiGen

## Overview
EmotiGen is an innovative AI chat application designed to understand and engage in conversations using African American Vernacular English (AAVE). By leveraging advanced natural language processing (NLP) technologies, EmotiGen aims to provide an inclusive and authentic conversational experience for users who communicate using AAVE.

## Features

- **AAVE Understanding**: EmotiGen is trained to understand and respond accurately to AAVE, making it one of the few chat applications tailored to this unique linguistic style.
- **Emotional Intelligence**: The app can detect and appropriately respond to a range of emotions, providing empathetic and contextually relevant replies.
- **Real-time Conversations**: Enjoy smooth, real-time interactions with the AI, simulating a natural conversation flow.
- **Customization**: Users can customize the chatbot's personality to better suit their preferences and needs.
- **Privacy**: EmotiGen is designed with user privacy in mind, ensuring all conversations are secure and confidential.

## Tech Stack

- **Frontend**: React Native
- **Backend**: Firebase (Authentication, Firestore, Functions)
- **AI/NLP**: Custom AI models integrated with the app

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Node.js and npm installed on your machine.
- React Native development environment set up (React Native CLI or Expo CLI).
- Firebase project configured with Firestore and any other necessary services.
- An internet connection for accessing Firebase services and AI models.

## Installation

### Steps

1. **Clone the Repository**

    ```sh
    git clone https://github.com/lennythecreator/Emoti-Gen.git
    cd emoti-gen
    ```

2. **Install Dependencies**

    ```sh
    npm install
    ```

3. **Set Up Firebase**

    - Go to the Firebase Console and create a new project.
    - Add an Android and/or iOS app to your Firebase project.
    - Follow the instructions to download the `google-services.json` (for Android) and `GoogleService-Info.plist` (for iOS).
    - Place these files in the appropriate directories in your React Native project:
        - `android/app/` for `google-services.json`.
        - `ios/` for `GoogleService-Info.plist`.

4. **Configure Firebase**

    Update your Firebase configuration in `src/config/firebaseConfig.js`:

    ```javascript
    import firebase from 'firebase/app';
    import 'firebase/auth';
    import 'firebase/firestore';

    const firebaseConfig = {
      apiKey: "YOUR_API_KEY",
      authDomain: "YOUR_AUTH_DOMAIN",
      projectId: "YOUR_PROJECT_ID",
      storageBucket: "YOUR_STORAGE_BUCKET",
      messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
      appId: "YOUR_APP_ID"
    };

    if (!firebase.apps.length) {
      firebase.initializeApp(firebaseConfig);
    }

    export { firebase };
    ```

5. **Run the Application**

    - For Android:

      ```sh
      npm run android
      ```

    - For iOS:

      ```sh
      npm run ios
      ```

    - For Web:

      ```sh
      npm run web
      ```

## Speech-to-Text Integration

### Free Speech-to-Text APIs

1. **Google Cloud Speech-to-Text API**
   - **Free Tier:** 60 minutes free per month.
   - **Documentation:** [Google Cloud Speech-to-Text](https://cloud.google.com/speech-to-text)

2. **Microsoft Azure Speech Service**
   - **Free Tier:** 5 audio hours per month for standard transcription.
   - **Documentation:** [Azure Speech Service](https://azure.microsoft.com/en-us/services/cognitive-services/speech-to-text/)

3. **IBM Watson Speech to Text**
   - **Free Tier:** 500 minutes free per month.
   - **Documentation:** [IBM Watson Speech to Text](https://www.ibm.com/cloud/watson-speech-to-text)

4. **Amazon Transcribe**
   - **Free Tier:** 60 minutes free per month for the first 12 months.
   - **Documentation:** [Amazon Transcribe](https://aws.amazon.com/transcribe/)

5. **AssemblyAI**
   - **Free Tier:** $5 worth of free credit (roughly 5 hours of audio).
   - **Documentation:** [AssemblyAI](https://www.assemblyai.com/)

6. **Deepgram**
   - **Free Tier:** $150 worth of free credit (approximately 45,000 minutes of audio).
   - **Documentation:** [Deepgram](https://deepgram.com/)

### Other Technologies for Speech-to-Text

#### Open Source Solutions

1. **Mozilla DeepSpeech**
   - **Description:** An open-source speech-to-text engine based on deep learning.
   - **Documentation:** [DeepSpeech GitHub](https://github.com/mozilla/DeepSpeech)
   - **Free:** Yes, but requires significant computational resources for training and usage.

2. **Kaldi**
   - **Description:** An open-source speech recognition toolkit.
   - **Documentation:** [Kaldi](http://kaldi-asr.org/)
   - **Free:** Yes, but requires expertise to set up and customize.

#### Libraries and Tools

1. **Coqui STT (formerly Mozilla TTS)**
   - **Description:** An open-source text-to-speech engine that also supports speech recognition.
   - **Documentation:** [Coqui STT](https://stt.readthedocs.io/en/latest/)
   - **Free:** Yes, open-source.

2. **OpenAI Whisper**
   - **Description:** A versatile speech recognition model by OpenAI.
   - **Documentation:** [OpenAI Whisper GitHub](https://github.com/openai/whisper)
   - **Free:** Yes, open-source.

## Contributing

To contribute to EmotiGen, follow these steps:

1. **Fork the Repository.**
2. **Create a Feature Branch:**

    ```sh
    git checkout -b feature/YourFeature
    ```

3. **Commit Your Changes:**

    ```sh
    git commit -m 'Add some feature'
    ```

4. **Push to the Branch:**

    ```sh
    git push origin feature/YourFeature
    ```

5. **Open a Pull Request.**

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

**EmotiGen** - Making conversations more engaging and emotionally intelligent!
