# Hanzi Trainer

A simple, effective, and offline-first flashcard application for memorizing Chinese characters (Hanzi). This tool uses a Spaced Repetition System (SRS) to help you focus on the characters you know least, and it runs entirely in your web browser.

![Hanzi Trainer Welcome Screen](https://raw.githubusercontent.com/gmitch/hanzi-trainer/refs/heads/main/hanzi1.png)
![Hanzi Trainer Flashcard Front](https://raw.githubusercontent.com/gmitch/hanzi-trainer/refs/heads/main/hanzi2.png)
![Hanzi Trainer Flashcard Back](https://raw.githubusercontent.com/gmitch/hanzi-trainer/refs/heads/main/hanzi3.png)

## How to Use

There are two easy ways to use this app.

### 1. Live App (Recommended)

You don't need to download or install anything. Just use the live version:

➡️ **[Open the Hanzi Trainer App](https://gmitch.github.io/hanzi-trainer/hanzi-trainer.html)**

---

### 2. Download Directly (or clone this repo! git@github.com:gmitch/hanzi-trainer.git )

You can just download the single file needed to run the app.

1.  Go to the `hanzi-trainer.html` file in the repo: **[Click Here](https://github.com/gmitch/hanzi-trainer/blob/main/hanzi-trainer.html)**
2.  Find the "Raw" button (it's near the top right of the file view).
3.  Right-click the **"Raw"** button.
4.  Select "Save Link As..." (or "Save As...") to download the file to your computer.
5.  Open the downloaded `hanzi-trainer.html` file in your browser.

---

## App Instructions

1.  **Prepare Your Vocabulary List**
    Create a `.csv` file with four columns in the following order: `Simplified`, `Traditional`, `Pinyin`, `English`.
    
    *Example `vocab.csv` file:*
    ```csv
    你,你,nǐ,you
    好,好,hǎo,good
    学,學,xué,to study
    生,生,shēng,life / to be born
    ```

2.  **Start a Session**
    -   To start with a new vocabulary list, click **"Start New Session"** and select your `.csv` file.
    -   To continue a previous session, click **"Load Existing Session"** and select your saved `.json` file.

3.  **Study**
    -   Look at the simplified character on the front. The traditional character is in the top right.
    -   Click the card to flip it over and see the details.
    -   Use the audio buttons to hear the Mandarin and Cantonese pronunciations.
    -   Click **"Knew It"** or **"Didn't Know"** to rate your knowledge and move to the next card.

4.  **Save Your Progress**
    When you are done studying, click the **"Save Session"** button. This will download a `hanzi_trainer_session.json` file containing all your words and their current scores.

## Features

-   **Spaced Repetition System (SRS):** Characters you struggle with appear more frequently. Each word has a score from 1 (new) to 10 (mastered).
-   **Load from CSV:** Easily import your vocabulary lists from a simple `.csv` file.
-   **Save/Load Progress:** Save your entire session, including scores for each word, into a `.json` file. Load it again later to pick up exactly where you left off.
-   **Dual Audio Pronunciation:** Listen to both **Mandarin** (for the simplified character) and **Cantonese** (for the traditional character) pronunciations using the browser's built-in text-to-speech.
-   **Traditional & Simplified:** Displays both character sets to aid comprehensive learning.
-   **Offline First:** The entire application is a single HTML file. Your data is never uploaded.
-   **Zero Dependencies:** No need to install anything.

## Technologies Used

-   **HTML5**
-   **CSS3**
-   **Vanilla JavaScript (ES6)**
-   **Web Speech API** for text-to-speech functionality.

## License

This project is licensed under the MIT License.
