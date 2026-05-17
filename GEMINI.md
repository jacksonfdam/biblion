# Biblion

Biblion is a modern, browser-based ebook reader designed for PDF and ePub files. It features a clean, focused reading experience with offline persistence, theme support, and text-to-speech capabilities.

## Project Overview

*   **Type:** Browser-based SPA (Single Page Application)
*   **Technologies:** 
    *   **HTML/CSS/JS:** Vanilla stack for the core interface and logic.
    *   **IndexedDB:** For local storage of books and reading progress.
    *   **PDF.js:** Used for rendering PDF documents.
    *   **Web Speech API:** Powering the Text-to-Speech (TTS) feature.
    *   **Google Fonts:** Lora, Source Serif 4, and JetBrains Mono for a refined typographic experience.
*   **Architecture:**
    *   The project is primarily contained within `index.html`, which houses the structure, styling, and the majority of the application logic in a large script block.
    *   `index.js` currently serves as a minimal entry point with a placeholder console log.
    *   `package.json` manages basic project metadata but lacks specific build or test scripts beyond defaults.

## Key Features

*   **Library Management:** Add PDF/ePub files to a local library stored in the browser.
*   **Reading Progress:** Automatic tracking and saving of scroll positions.
*   **Theming:** Multiple reading modes (Light, Dark, Sepia, Night) and adjustable brightness/contrast.
*   **Typography:** Custom font sizing and carefully selected serif/monospace fonts.
*   **Text-to-Speech:** Integrated TTS with voice selection and rate control.
*   **Offline Support:** Once loaded, the application can function without an active internet connection thanks to local storage.

## Building and Running

The project now includes a simple Node.js server for local development and hosting:

1.  **Installation:** Run `npm install` to install dependencies (Express).
2.  **Run:** Run `npm start` to start the local server. The application will be available at `http://localhost:3000`.
3.  **Vercel Deployment:** The project is configured with `vercel.json` to be deployed as a Node.js application. It uses the `@vercel/node` builder and routes all traffic to `index.js`, which exports the Express app for compatibility with Vercel's serverless environment.
4.  **Tests:** Currently, no automated tests are specified. (TODO: Implement basic unit/integration tests).

## Development Conventions

*   **Code Style:** The project uses a compact, single-file approach for its core features.
*   **Logic Location:** Most UI interactions and data management are handled within `index.html`'s `<script>` tag.
*   **Persistence:** All persistent data (books, progress) must be handled through the IndexedDB wrapper functions (`dbGet`, `dbPut`, `dbDel`).
