
# Vintage PDF Typing Speed Analyzer ⌨️🕰️

A purely client-side, browser-based typing speed tester that allows users to upload their own PDF documents and use the extracted text for their typing tests. It features a retro, mechanical typewriter aesthetic and provides real-time performance analytics.

## ✨ Features

* **Local PDF Parsing:** Utilizes Mozilla's `pdf.js` to extract text from uploaded PDFs entirely within the browser. No files are ever sent to a server, ensuring complete user privacy.
* **Vintage Typewriter UI:** Carefully styled to mimic a classic mechanical typewriter, complete with ruled paper textures, classic fonts, ink-bleed effects, and strike-throughs for typing errors.
* **Real-Time Analytics:** Tracks and displays Words Per Minute (WPM), Accuracy percentage, and total errors dynamically as you type.
* **Customizable Sessions:** Users can select 1, 2, 3, or 5-minute timed sessions.
* **Interactive Results Modal:** A clean pop-up displays final statistics when the timer expires, offering options to retry the current text or perform a hard reset for a new document.

## 🛠️ Tech Stack

* **HTML5:** Semantic structure and hidden input mapping for mobile/desktop-agnostic keystroke capturing.
* **CSS3:** Custom properties (variables), keyframe animations, CSS gradients for paper texturing, and responsive flexbox layouts.
* **Vanilla JavaScript (ES6+):** Event handling, real-time math calculations for WPM/Accuracy, state management, and DOM manipulation.
* **PDF.js:** (Imported via CDN) Used for asynchronous document rendering and text extraction.

## 🚀 How to Run Locally

Because this project has no backend dependencies, running it is incredibly simple:

1. Clone this repository or download the ZIP file.
2. Open the `index.html` file directly in any modern web browser (Chrome, Firefox, Safari, Edge).
3. Upload a text-based PDF and start typing!

## 💡 How the Typing Capture Works
Instead of relying on fragile global `keydown` events (which often fail on mobile devices or alternative keyboard layouts), this project overlays a transparent, hidden `<input>` field over the text display. Clicking the paper focuses the input, ensuring 100% accurate keystroke capturing across all devices.
