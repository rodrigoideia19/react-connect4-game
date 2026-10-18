# Connect 4: Special Edition — React.js Web Application

[![Framework: React](https://img.shields.io/badge/Framework-React_18-61DAFB.svg?logo=react&logoColor=black)](https://reactjs.org/)
[![Language: JavaScript](https://img.shields.io/badge/Language-JavaScript_ES6+-F7DF1E.svg?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Course: Linguagens Script](https://img.shields.io/badge/Course-Scripting_Languages-green.svg)](https://www.isec.pt)
[![Institution: ISEC](https://img.shields.io/badge/Institution-ISEC_Coimbra-red.svg)](https://www.isec.pt)

> [!NOTE]  
> **Academic Context:**  
> Developed for the **Scripting Languages (Linguagens Script - LS)** curricular unit in the **BSc in Computer Science (Licenciatura em Engenharia Informática)** at **ISEC - Instituto Superior de Engenharia de Coimbra** (Academic Year 2024/2025).

---

## 📌 Project Overview

An interactive, responsive single-page web implementation of the classic **Connect 4** (*4 em Linha*) game built using **React.js**. This version introduces enhanced competitive gameplay dynamics, including custom special board cells, a real-time turn countdown timer, dynamic win-detection algorithms, and an automated single-player Bot mode.

---

## 🎮 Key Gameplay Features

* **Dual Game Modes:**
  * **2-Player Local PvP:** Custom player profiles and names with alternating turns.
  * **Player vs. Bot (PvE):** Single-player mode against an automated computer opponent.
* **Special Grid Cells (*Casas Especiais*):**
  * Randomly designated bonus slots on the grid that award the player an immediate repeat move upon landing.
* **Turn Countdown Timer:**
  * Real-time timer per play that forces active decision making, penalizing idle players when time expires.
* **Dynamic Win Detection:**
  * Real-time algorithmic evaluation detecting 4-in-a-row connections horizontally, vertically, and diagonally across both axes.
* **Rich UI & Animations:**
  * Smooth CSS/JS falling piece transitions and column hover indicators.
  * Persistent match session scoreboard tracking victories, moves history, and elapsed game time.

---

## 🏗️ Architecture & Component Design

The application is structured into modular functional components utilizing modern React paradigms:

```text
src/
├── assets/                  # SVG game tokens and background artwork
│   ├── black token.svg
│   ├── red token.svg
│   └── bkkk.jpg
├── components/
│   ├── Board.jsx            # Core game engine: state, timer, win logic & AI
│   └── Slot.jsx             # Individual interactive grid slot component
├── App.css                  # Modern UI styles, animations, and board grid layout
├── App.js                   # Application root container
└── index.js                 # React DOM mount point
```

* **State Management:** Pure React Hooks (`useState`, `useEffect`, `useRef`) for turn synchronization, animation sequencing, and interval handling.
* **Clean Code:** Separation of presentation components from board state logic.

---

## 🚀 Getting Started

### Prerequisites
* [Node.js](https://nodejs.org/) (v16 or higher)
* [npm](https://www.npmjs.com/) or [yarn](https://yarnpkg.com/)

### Installation & Execution

1. **Clone the repository:**
   ```bash
   git clone https://github.com/rodrigoideia19/react-connect4-game.git
   cd react-connect4-game
   ```

2. **Install project dependencies:**
   ```bash
   npm install
   ```

3. **Start the local development server:**
   ```bash
   npm start
   ```
   Open [http://localhost:3000](http://localhost:3000) to play in your browser.

4. **Build for production:**
   ```bash
   npm run build
   ```

---

## 👥 Authors

* **Rodrigo Salgueiro Ideia** — [GitHub](https://github.com/rodrigoideia19)
* **André Pessoa Tavares**
* **Gonçalo Bento**

*BSc in Computer Science (LEI / European Course), Instituto Superior de Engenharia de Coimbra (ISEC)*
