# Developer Portfolio Technical Specification

Version 1.0

## Core Technical Requirements

### Video Examples of Podcast Generators

- [Basic Example](https://www.paulgasbarra.com) - Tier 1 - Basic example of a portfolio website

- [Advanced Example]() - Tier 2 - No Example Yet - AI Chat Bot - an ai chat bot that can answer questions about the candidate

## User Flow

If you want to see the user flow for this project to envision your building process or understand the user experience, please refer to the [user-flow.md](user-flow.md) file.

### Frontend (HTML/CSS/JS)

- Simple HTML website built off a template
- BootstrapMade template
- [BootstrapMade](https://bootstrapmade.com/)
- [BootstrapMade Templates](https://bootstrapmade.com/templates/)

### Backend (Express)

- Express server
- Google Gemini API
- Google Gemini API Key

### Required Libraries

#### Frontend

- HTML
- CSS
- JavaScript

#### Backend Packages

- express
- google-generative-ai
- multer (optional)
- cors
- dotenv

## API Endpoints

### 1. Generate Responses to User Queries about the Candidate

```javascript
POST /api/generate-response
type: application/json

{
  "userQuery": "What are this candidate's strengths?"
}

```

## AI Integration

### Gemini AI Configuration

```javascript
const genAI = new GoogleGenerativeAI(API_KEY);
const model = genAI.getGenerativeModel({
  model: "gemini-1.5-flash",
  generationConfig: {
    temperature: 0.5,
    topP: 0.95,
    topK: 40,
    maxOutputTokens: 5500,
  },
});
```

### Prompt Engineering

- Helpful assistant
- Answer questions about the candidate
- Use info from linked resume to answer questions about the candidate
-

### Directory Management

## UI Requirements

### Input Methods

- Pop-up chat bot that allows users to ask questions about the candidate

### Styling Requirements

- Responsive design (mobile-first)
- Clear visual hierarchy
- Interactive elements feedback
- Loading states
- Error state handling

## Error Handling

- Client-side validation
- Server-side error handling
- Graceful fallbacks

## Resources

- [BootstrapMade Templates](https://bootstrapmade.com/templates/)
- [Prompt Engineering Guide](https://www.promptingguide.ai/)

[Back to Home](README.md)
[User Flow](user-flow.md)
