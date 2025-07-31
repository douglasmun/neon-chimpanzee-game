# **Neon Chimpanzee Game**
Test Your Memory, Master the Sequence! Inspired by cognitive research on chimpanzee memory.

## **Executive Summary:**

"Neon Chimpanzee" is an electrifying and educational browser-based game inspired by groundbreaking cognitive research on chimpanzee memory. It challenges players to replicate rapidly flashing number sequences, pushing the boundaries of their short-term memory and pattern recognition skills. With a progressively challenging difficulty curve—from "Human" to the lightning-fast "Chimp" mode—a vibrant neon aesthetic, and competitive high-score tracking, this game offers a unique blend of scientific insight and thrilling gameplay. Designed for accessibility and seamless play on both desktop and mobile devices, "Neon Chimpanzee" provides a captivating experience that's both fun and intellectually stimulating.

## **Technical Summary:**

"Neon Chimpanzee" is a robust, client-side web application built primarily with HTML, CSS, and JavaScript, designed for broad browser compatibility and responsiveness.

### **Core Features:**

* **Dynamic Tile Generation**: Creates interactive, numbered circular tiles in random, non-overlapping positions within the game area for each level.  
* **Progressive Difficulty System**: Adapts game parameters—sequence display time, number of tiles, and score multiplier—across four distinct difficulty levels ("Human," "Smart," "Genius," and "Chimp") based on the player's progression.  
* **Memory Sequence Playback**: Visually displays number sequences by rapidly highlighting tiles, demanding acute observation from the player.  
* **Interactive Input Validation**: Processes player clicks/touches, verifying the correctness of the input sequence against the displayed pattern.  
* **Real-time Countdown Timer**: Implements a pressure-inducing timer that resets per level, challenging players to recall sequences within a time limit.  
* **Scoring and High Score Management**: Calculates scores based on sequence length and difficulty, and persistently stores top scores using localStorage for competitive leaderboards.  
* **Responsive UI/UX**: Features a "neon" themed visual design that dynamically adjusts to various screen sizes, ensuring an optimal experience on both desktop and mobile devices.

### **Technical Highlights:**

* **Pure Client-Side Implementation**: The entire game logic, including state management, UI rendering, and high-score persistence, is handled client-side using vanilla JavaScript, eliminating the need for server-side infrastructure.  
* **Robust Event Handling**: Utilizes addEventListener for click, touchstart, and keydown events, ensuring broad input compatibility and accessibility for interactive elements.  
* **Accessibility Enhancements**: Incorporates tabindex for keyboard navigation on game tiles, aria-live regions for screen reader announcements, and improved color contrast ratios for better readability.  
* **Efficient Animation and Timing**: Leverages setTimeout and setInterval for precise control over sequence display and timer updates, with a mechanism to clear pending operations efficiently on game state changes.  
* **Secure User Input Handling**: Employs an escapeHtml function to sanitize user-provided high score names, preventing Cross-Site Scripting (XSS) vulnerabilities.  
* **Modular Game State Management**: Organizes game variables within a gameState object, facilitating clear separation of concerns and easier maintenance of game logic.
