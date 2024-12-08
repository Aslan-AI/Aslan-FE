# Aslan AI Frontend

The frontend component of the Aslan AI Mental Health Support Platform. This web application provides an intuitive interface for users to interact with our AI-powered emotional support system.

## Features

- User Authentication (Login/Register)
- Real-time Chat Interface
- Emotion Detection & Display
- Token Usage Tracking
- Responsive Design
- Dark/Light Theme Support

## Project Structure

```
Aslan-FE-main/
├── index.html        # Main HTML file
├── styles.css        # Global styles
├── script.js         # Main JavaScript file
├── shared/          # Shared utilities
│   └── validation.js # Shared validation rules
└── images/          # Image assets
```

## Setup

1. Clone the repository
2. Open `index.html` in your browser
3. Make sure the backend server is running at `https://aslan-be.onrender.com`

## Integration Notes

The frontend is designed to work with the Aslan AI backend. It expects the following endpoints:

- `/api/auth/login` - User login
- `/api/auth/register` - User registration
- `/api/chat/session` - Start chat session
- `/api/chat/message` - Send/receive messages
- `/api/chat/history` - Get chat history
- `/sentiment/analyze` - Sentiment analysis

## Development

To run the project locally:
1. Use a local server (e.g., `python -m http.server` or Live Server in VS Code)
2. Open `http://localhost:8000` in your browser

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request
