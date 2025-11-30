# LinguaFlow - AI Conversation Partner

A multi-agent language learning application built for the Google AI Agents Course Capstone.

## Features

- **Multi-Agent Architecture**:
  - **Conversation Partner**: Engages in natural dialogue.
  - **Grammar Coach**: Provides real-time corrections in your native language.
  - **Cultural Advisor**: Offers cultural insights relevant to the conversation.
  - **Scenario Generator**: Creates immersive roleplay situations.
- **Multi-Language Support**:
  - **Native Languages**: English, Cantonese (yue), Traditional Chinese (zh-TW), etc.
  - **Target Languages**: English, Japanese, French, German, Traditional Chinese.
- **Memory**: Remembers user profile and conversation history.

## Prerequisites

- Node.js (v18+)
- Google Gemini API Key

## Setup

1.  Clone the repository (or navigate to the directory).
2.  Install dependencies:
    ```bash
    npm install
    ```
3.  Create a `.env` file in the root directory and add your API Key:
    ```env
    GEMINI_API_KEY=your_api_key_here
    PORT=3000
    ```

## Running the Application

1.  **Development Mode**:
    ```bash
    npm run dev
    ```
2.  **Production Build**:
    ```bash
    npm run build
    npm start
    ```
3.  Open your browser to `http://localhost:3000`.

## Usage

1.  Select your **Native Language** (e.g., Cantonese) and **Target Language** (e.g., English).
2.  Click **Update** to save settings.
3.  Click **Start New Scenario** to generate a roleplay situation.
4.  Type or speak your response.
5.  Receive a reply from the partner, plus grammar corrections and cultural tips in the sidebar!

## Architecture

- **Backend**: Node.js + Express + TypeScript
- **AI**: Google Gemini Pro via `@google/generative-ai`
- **Frontend**: Vanilla HTML/CSS/JS
