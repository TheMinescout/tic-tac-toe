# 🎮 Terra Cotta Game Suite & The AI One-Shot Challenge

Welcome to the **Terra Cotta Game Suite**, a collection of classic arcade and logic games bundled into a single, lightweight HTML file. 

This repository serves two purposes:
1.  To host the **Official Game Suite**, a polished, fully functional web app.
2.  To host an **AI Experiment**, comparing how different Large Language Models (LLMs) respond to the exact same complex coding prompt in a single attempt.

---

## 🌟 The Official Version
**File:** [`index.html`](./index.html)  
**Status:** ✅ Maintained, Updated, Recommended.

This is the polished version of the game. It includes bug fixes, UI improvements, and stable multiplayer connectivity. If you just want to play, **launch this version.**

### Features
* **5 Games in One:**
    * **Tic-Tac-Toe Suite:** Normal (3x3), 3D (3x3x3), and Ultimate (9x9).
    * **Snake:** Classic arcade gameplay.
    * **Minesweeper:** Logic puzzle with flagging.
    * **Dino Run:** Infinite runner.
    * **Pac-Man Lite:** Grid-based arcade chase.
* **Multiplayer:** Peer-to-peer hosting and joining for Tic-Tac-Toe using PeerJS.
* **Tech Stack:** Single-file HTML5 (HTML/CSS/JS). No build tools required.
* **Design:** Minimalist Material Design 3 aesthetic (Terra Cotta & Dark Grey).

---

## 🤖 The AI "One-Shot" Experiment

We challenged leading AI models to build this exact application. 

**The Rules:**
1.  They were given **one specific prompt** (see below).
2.  They had to generate the entire code in a **single output**.
3.  **No human intervention** or bug fixing was allowed for these specific files (unless the code was literally unrunnable due to truncation).

### The Contestants
You can test the raw, unedited outputs of each AI below to see how they interpreted the prompt and handled the logic:

| AI Model | File Link | Notes |
| :--- | :--- | :--- |
| **Google Gemini** | [`gemini.html`](./gemini.html) | See how Gemini handled the 3D logic and CSS. |
| **ChatGPT** | [`gpt.html`](./gpt.html) | Check OpenAI's approach to the single-file constraint. |
| **Claude** | [`claude.html`](./claude.html) | Observe Anthropic's take on the Terra Cotta aesthetic. |

---

## 📝 The Prompt
The following prompt was given to every AI model. It describes the design system, the tech stack, and the game logic required:

> "Code a complete, single-file HTML5 game application called 'Terra Cotta Game Suite' that requires no external assets (use CSS/Canvas for graphics). The app should function as a central hub where the user selects a game from a grid of cards to play. The technical stack must be HTML, CSS, and vanilla JavaScript all in one file, using PeerJS (via CDN) for multiplayer networking and Canvas Confetti (via CDN) for win effects. The application must be fully responsive for mobile devices, handling touch events (swipes for Snake/Pac-Man, taps for others) and scaling the UI to fit small screens without breaking."
>
> "Style the application with a clean, minimalist 'Material Design 3' aesthetic. Use this specific color palette: a clean White (#FFFFFF) background, Terra Cotta (#DD8566) as the primary accent color for buttons and highlights, Dark Grey (#474D4D) for text and game elements, and Silver (#F5F5F5) for surfaces. UI elements should feature rounded corners (pill-shaped buttons, rounded cards), subtle drop shadows, and the Roboto font. Include a generated SVG favicon in the head that matches the theme. Ensure there is a global 'Back to Hub' button accessible from every game screen."
>
> "Implement the following five games within the suite:
> **Tic-Tac-Toe Suite:** Must include Normal (3x3), 3D (3x3x3 stacked grids using CSS 3D transforms), and Ultimate (9x9) variants. It needs three modes: Local Pass & Play, vs. Random Bot, and P2P Multiplayer (Host/Join via a 9-digit code or shareable link).
> **Snake:** A classic canvas-based version.
> **Minesweeper:** Grid-based with flagging and flood-fill revealing.
> **Dino Run:** A simple canvas infinite runner with jumping.
> **Pac-Man Lite:** A simplified grid-based version with random ghost AI.
> Ensure all game logic is modular and that the 3D Tic-Tac-Toe board includes a visual stack animation when a player wins."

---

## 🚀 How to Run
Since this is a single-file application, you don't need to install Node.js, Python, or any dependencies.

1.  **Download** the repository (or just the `.html` file you want to play).
2.  **Open** the file in any modern web browser (Chrome, Edge, Firefox, Safari).
3.  **For Multiplayer:** PeerJS requires a secure context or localhost. To play multiplayer with friends over the internet, we recommend hosting this on **GitHub Pages**.

### Enabling GitHub Pages
1.  Go to `Settings` in your repository.
2.  Click `Pages` on the left sidebar.
3.  Under `Source`, select `Deploy from a branch` and choose `main` (or `master`).
4.  Your game will be live at `https://<your-username>.github.io/<repo-name>/`.

---

*This project is open source. Feel free to fork and improve the main `index.html`!*
