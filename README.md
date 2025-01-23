<img src="./readme/title1.svg"/>

<br><br>

<!-- project philosophy -->
<img src="./readme/title2.svg"/>

A screen recording app powered by AI that extracts and summarizes video content for quick reviews. It intelligently fills  in network lag gaps with context-based suggestions to ensure smooth playback. Additionally, it segments the video into organized sections based on the topics covered, improving navigation and sharing.

### User Stories
#### Admin
- As an admin, I want to manage user accounts to ensure the platform is secure and user-friendly.
- As an admin, I want to monitor and adjust AI features like gap filling, summarization, and segmentation to optimize performance.
- As an admin, I want to analyze user feedback on AI features to continually improve the system.
#### User
- As a user, I want the app to summarize my recordings, so I can quickly review and share key content.
- As a user, I want AI to automatically fill in network lag gaps, ensuring smooth playback and no disruptions.
- As a user, I want my video to be divided into sections based on content, so I can easily navigate and share specific topics.

<br><br>
<!-- Tech stack -->
<img src="./readme/title3.svg"/>

###  RecapPro is built using the following technologies:

- This project uses the [Flutter app development framework](https://flutter.dev/).
Flutter is a cross-platform hybrid app development platform that allows us to use a single codebase for apps on iOS, Android, desktop, and the web.  
- For screen recording, the app integrates native SDKs like [ReplayKit](https://developer.apple.com/documentation/replaykit) for iOS and [MediaProjection](https://developer.android.com/reference/android/media/projection/MediaProjection) for Android using Flutter’s [Platform Channels](https://docs.flutter.dev/development/platform-integration/platform-channels).  
- Backend operations are managed with [Node.js](https://nodejs.org/) and [Express.js](https://expressjs.com/).  
- Persistent storage and metadata management use [MongoDB](https://www.mongodb.com/).  
- For video processing, the app employs [FFmpeg](https://ffmpeg.org/).  
- AI features include:  
  - Network gap filling using [Deep Video Interpolation (DVI)](https://arxiv.org/abs/1711.09078).  
  - Audio transcription with [Mozilla DeepSpeech](https://github.com/mozilla/DeepSpeech).  
  - Summarizing transcriptions with [OpenAI GPT](https://platform.openai.com/).  


<br><br>
<!-- UI UX -->
<img src="./readme/title4.svg"/>


>RecapPro's interface was designed with user experience in mind. We used wireframing and multiple iterations of mockups to create an intuitive and engaging platform.

- Project Figma design [figma](https://www.figma.com/design/qPOK5c0TeBfIz2ulzV6xUb/Recap-Pro?node-id=0-1&t=k5YeQ8ZgT5QJ5g4F-1)


### Mockups
| Register  | Home Screen | Video Screen |
| ---| ---| ---|
| ![Landing](./readme/uix/Register.png) | ![fsdaf](./readme/uix/Home.png) | ![fsdaf](./readme/uix/Edit.png) |

<br><br>

<!-- Database Design -->
<img src="./readme/title5.svg"/>

###  Architecting Data Excellence: Innovative Database Design Strategies:


<p align="center">
  <img src="./readme/code1.png" width="45%" />
  <img src="./readme/code2.png" width="45%" />
</p>
<p align="center">
  <img src="./readme/code3.png" width="45%" />
  <img src="./readme/code4.png" width="45%" />
</p>



<br><br>


<!-- Implementation -->
<img src="./readme/title6.svg"/>


### User Screens (Mobile)
| Login screen  | Register screen | Landing screen | Loading screen |
| ---| ---| ---| ---|
| ![Landing](https://placehold.co/900x1600) | ![fsdaf](https://placehold.co/900x1600) | ![fsdaf](https://placehold.co/900x1600) | ![fsdaf](https://placehold.co/900x1600) |
| Home screen  | Menu Screen | Order Screen | Checkout Screen |
| ![Landing](https://placehold.co/900x1600) | ![fsdaf](https://placehold.co/900x1600) | ![fsdaf](https://placehold.co/900x1600) | ![fsdaf](https://placehold.co/900x1600) |

### Admin Screens (Web)
| Login screen  | Register screen |  Landing screen |
| ---| ---| ---|
| ![Landing](./readme/demo/1440x1024.png) | ![fsdaf](./readme/demo/1440x1024.png) | ![fsdaf](./readme/demo/1440x1024.png) |
| Home screen  | Menu Screen | Order Screen |
| ![Landing](./readme/demo/1440x1024.png) | ![fsdaf](./readme/demo/1440x1024.png) | ![fsdaf](./readme/demo/1440x1024.png) |

<br><br>


<!-- Prompt Engineering -->
<img src="./readme/title7.svg"/>

###  Mastering AI Interaction: Unveiling the Power of Prompt Engineering:

This project leverages advanced prompt engineering techniques to optimize interactions with AI models for transcription analysis, gap filling, and topic segmentation. By carefully designing input prompts, we enhance language understanding and generation, ensuring precise responses tailored to video content. Key implementations include:

- **Transcription Analysis:** Structuring AI queries to improve accuracy in speech-to-text conversion.
- **Gap Filling:** Crafting prompts that guide AI in generating contextually relevant content for silent sections.
- **Topic Segmentation:** Using structured prompts to guide the AI identifying and organizing video sections based on content themes.

These techniques refine AI responses, making Recap Pro a powerful tool for automated video processing.
<br><br>

<!-- AWS Deployment -->
<img src="./readme/title8.svg"/>

###  Efficient AI Deployment: Unleashing the Potential with AWS Integration:

- This project leverages AWS deployment strategies to seamlessly integrate and deploy natural language processing models. With a focus on scalability, reliability, and performance, we ensure that AI applications powered by these models deliver robust and responsive solutions for diverse use cases.

<br><br>

<!-- How to run -->
<img src="./readme/title10.svg"/>

> Recap Pro is a powerful tool for processing and segmenting videos with AI-driven insights. Follow the steps below to set it up locally.


### Prerequisites

Ensure you have the following installed on your system:

- **Node.js** (Recommended: Latest LTS version) - [Download](https://nodejs.org/)
- **npm** (Comes with Node.js, but update if necessary)
  ```sh
  npm install npm@latest -g
  ```
- **FFmpeg** (Required for video processing)
  - macOS (Homebrew):
    ```sh
    brew install ffmpeg
    ```
  - Ubuntu:
    ```sh
    sudo apt update && sudo apt install ffmpeg
    ```
  - Windows:
    - Download from [FFmpeg official site](https://ffmpeg.org/download.html) and add it to your system PATH.

- **Flutter** (Latest stable version)
  - Follow installation guide: [Flutter Docs](https://flutter.dev/docs/get-started/install)

### Installation

1. **Get a free API Key** at [Groq](https://console.groq.com/keys)
2. **Clone the repository**
   ```sh
   git clone https://github.com/Moe-Karim/RecapPro.git
   ```
3. **Navigate into the project directory**
   ```sh
   cd RecapPro
   ```
4. **Install Node.js dependencies**
   ```sh
   npm i
   ```
5. **Set up the API key** in `.env`
   ```js
   const API_KEY = 'ENTER_YOUR_API_KEY_HERE';
   ```
6. **Install Flutter dependencies**
   ```sh
   flutter pub get
   ```
7. **Run the app**
   - **Backend:**

      - **Backend dev mode:**
      ```sh
      npm run start:dev
      ```
      or

      - **Backend:**
      ```sh
      npm run start
      ```
   - **Frontend (Flutter app):**
     ```sh
     flutter run
     ```

Now, you should be able to run **Recap Pro** locally and explore its features. 🚀