# Biblion

Biblion is a modern, browser-based ebook reader designed for PDF and ePub files. It features a clean, focused reading experience with offline persistence, theme support, and text-to-speech capabilities.

## Features

- **Library Management:** Add PDF/ePub files to a local library stored in your browser.
- **Reading Progress:** Automatically tracks and saves your scroll position.
- **Customizable Themes:** Light, Dark, Sepia, and Night modes.
- **Brightness & Contrast:** Fine-tune the visual experience.
- **Text-to-Speech (TTS):** Listen to your books with integrated voice synthesis.
- **Responsive Design:** Optimized for both desktop and mobile reading.

## Tech Stack

- **Vanilla HTML/CSS/JS**
- **IndexedDB:** For local storage.
- **PDF.js:** For rendering PDF files.
- **Web Speech API:** For Text-to-Speech.

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (for local development)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/jacksonfdam/Biblion.git
   cd Biblion
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

### Running Locally

To run the application locally, use:
```bash
npm start
```
This will start a local server, and you can access the app at `http://localhost:3000`.

## Deployment

### Vercel

This project is ready for deployment on [Vercel](https://vercel.com). You can simply import your repository to Vercel, and it will automatically detect the static files.

## License

This project is private and for personal use.
