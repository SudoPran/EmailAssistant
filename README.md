# AI Email Reply Generator

A Spring Boot with a React and Chrome extension that generates AI-powered email replies using Google's Gemini API.

## Features

- **Web Application**:
  - Paste any email content and select a tone (professional, casual, friendly)
  - Get AI-generated replies instantly
  - Copy replies to clipboard with one click

- **Chrome Extension**:
  - Integrates directly with Gmail
  - Adds "AI Reply" button to compose windows
  - Generates context-aware replies based on email content
  - Maintains Gmail's native UI look and feel

## Technologies Used

- **Backend**:
  - Spring Boot
  - WebFlux for reactive API calls
  - Google Gemini API integration
  - CORS configuration for cross-origin requests

- **Frontend**:
  - React.js with Vite
  - Material UI for styling
  - Axios for API calls

- **Chrome Extension**:
  - Manifest v3
  - Mutation Observers for DOM monitoring
  - Content scripts for UI injection
  - Gmail API integration

## Installation

### Prerequisites
- Java 17+
- Node.js 16+
- Google Chrome
- Google Gemini API key

### Backend Setup
1. Clone the repository
2. Configure environment variables in `application.properties`:
   ```properties
   gemini.api.url=https://generativelanguage.googleapis.com/v1beta/models/gemini-pro:generateContent
   gemini.api.key=your_api_key_here
