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
  - Network gap filling using [Groq](https://console.groq.com/docs/overview).  
  - Audio transcription with [Groq](https://console.groq.com/docs/overview).  
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

| Part 1 | Part 2 | Part 3 |
| --- | --- | --- |
| <img src="./readme/code1.png" width="100%"> | <img src="./readme/code2.png" width="100%"> | <img src="./readme/code3.png" width="100%"> |

| Part 4 |
| --- |
| <img src="./readme/code4.png" width="80%"> |



<br><br>


<!-- Implementation -->
<img src="./readme/title6.svg"/>


### User Screens (Mobile)
| Onboarding screen  | Login screen | Recording screen | Change password |
| ---| ---| ---| ---|
| ![Landing](./readme/screen/splash.gif) | ![fsdaf](./readme/screen/login.gif) | ![fsdaf](./readme/screen/recording.gif) | ![fsdaf](./readme/screen/Password.gif) |
| Transcribe audio | Video segmentation | Gap filling | Gap subtitled |
| ![Landing](./readme/screen/transcribe.gif) | ![fsdaf](./readme/screen/segments.gif) | ![fsdaf](./readme/screen/gapFilling.gif) | ![fsdaf](./readme/screen/gapFilled.gif) |
| Dark mode | Clear videos | Delete user |
| ![Landing](./readme/screen/dark.gif) | ![fsdaf](./readme/screen/videos.gif) |![fsdaf](./readme/screen/delete.gif) |

<br><br>


<!-- Prompt Engineering -->
<img src="./readme/title7.svg"/>

###  Boosting AI for Video Processing: Speech Analysis, Content Structuring, and Filling Gaps

This project leverages advanced prompt engineering techniques to optimize interactions with AI models for transcription analysis, gap filling, and topic segmentation. By carefully designing input prompts, we enhance language understanding and generation, ensuring precise responses tailored to video content. Key implementations include:

- **Transcription Analysis:** Structuring AI queries to improve accuracy in speech-to-text conversion.
- **Gap Filling:** Crafting prompts that guide AI in generating contextually relevant content for silent sections.
- **Topic Segmentation:** Using structured prompts to guide the AI identifying and organizing video sections based on content themes.

These techniques refine AI responses, making Recap Pro a powerful tool for automated video processing.
<br><br>
| Feature | Description | Preview |
| --- | --- | --- |
| Transcribe Audio | Converts speech to text | ![Transcribe](./readme/ai/Transcribe.png) |
| Segment Videos | Splits videos into topic-based segments | ![Topics](./readme/ai/Topics.png) |
| Gap Filling | Fills silent gaps with AI-generated content | ![Gaps](./readme/ai/Gaps.png) |

<!-- AWS Deployment -->
<img src="./readme/title8.svg"/>

### Deployment Strategy: Running on AWS EC2

-Our backend runs on an AWS EC2 instance, providing a stable and flexible environment for our application. EC2 allows us to manage the server, handle incoming requests efficiently, and ensure smooth performance. Since we have full control over the instance, we can update the application whenever needed, restart services, and adjust resources based on demand. This setup keeps our deployment simple while ensuring reliability and responsiveness.

<br><br>
| Register user | Change password | Login user |
| --- | --- | --- |
| ![Request1](./readme/aws/registerUser.png) | ![Request2](./readme/aws/changePassword.png) | ![Request3](./readme/aws/loginUser.png) |
| Get videos | Upload video | Delete video |
| ![Request4](./readme/aws/getVideos.png) | ![Request5](./readme/aws/uploadVideo.png) | ![Request6](./readme/aws/deleteVideos.png) |
| Delete user |  |  |
| ![Request7](./readme/aws/deleteUser.png) |  |  |
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