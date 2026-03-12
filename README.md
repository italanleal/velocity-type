# ⚡ Velocity Type | 100 Word Challenge

Velocity Type is a minimalist, high-performance typing game designed to test both speed (WPM) and accuracy. Unlike standard typing tests, Velocity Type uses a **Markov Chain** to generate rhythmic, semi-natural text from a local corpus, creating a unique typing flow every time you play.

!

## ✨ Key Features

* **🧠 Markov Chain Generation**: Text is generated dynamically from a local `corpus.txt`. This ensures a natural linguistic flow rather than just a random string of words.
* **💎 Precision Scoring**: 
    * **Perfect Words**: Earn a golden "PERFECT" bonus and increase your multiplier by typing words with zero mistakes and zero backspaces.
    * **Strict Multiplier**: Any mistype immediately resets your streak multiplier to 1.0x.
* **❤️ Life System**: You have 3 lives. Committing a word with uncorrected errors costs a life. 
* **🎯 Pixel-Perfect Cursor**: An absolute-positioned cursor that tracks character offsets in real-time.
* **🔒 Anti-Cheat/Zoom**: Custom JavaScript handlers to disable browser zooming (Ctrl + Scroll/Keys) to maintain layout integrity.

## 🕹️ How to Play

1.  **Start Typing**: The 50ms precision WPM timer starts the moment you press your first key.
2.  **Aim for Perfection**: Type a word perfectly (no backspaces, no errors) to glow gold and boost your score multiplier.
3.  **Correct Mistakes**: You can use `Backspace` or `Ctrl + Backspace` to fix errors, but the word will no longer be "Perfect."
4.  **Finish the Challenge**: Complete 30 words (configurable) without losing your 3 lives.

## 🚀 Installation & Setup

1.  **Clone the Repository**:
    ```bash
    git clone [https://github.com/yourusername/velocity-type.git](https://github.com/yourusername/velocity-type.git)
    ```
2.  **Add your Corpus**:
    Place a text file named `corpus.txt` inside the `/static` folder. The Markov Chain will use this text to generate the game content.
3.  **Run**:
    Since the game uses `fetch` to read the static file, you must run it via a local server (like Live Server in VS Code) to avoid CORS issues.

## 🛠️ Built With

* **HTML5/CSS3**: Custom cyberpunk aesthetic with neon glow effects.
* **Vanilla JavaScript**: No heavy frameworks—just raw DOM manipulation and a Bigram Markov Chain implementation.
