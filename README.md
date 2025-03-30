# AI Email Reply Generator

The AI Email Reply Generator is a comprehensive solution that combines Google's Gemini API with:

-A Spring Boot backend with REST API endpoints.
-A React frontend web application.
-A Chrome extension that integrates directly with Gmail.

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
