# Hanzi Trainer

A simple, effective, and offline-first flashcard application for memorizing Chinese characters (Hanzi). This tool uses a Spaced Repetition System (SRS) to help you focus on the characters you know least, and it runs entirely in your web browser.


![Hanzi Trainer Screenshot](https://raw.githubusercontent.com/gmitch/hanzi-trainer/refs/heads/main/hanzi1.png)
![Hanzi Trainer Screenshot](https://raw.githubusercontent.com/gmitch/hanzi-trainer/refs/heads/main/hanzi2.png)
![Hanzi Trainer Screenshot](https://raw.githubusercontent.com/gmitch/hanzi-trainer/refs/heads/main/hanzi3.png)

## Features

-   **Spaced Repetition System (SRS):** Characters you struggle with appear more frequently. Each word has a score from 1 (new) to 10 (mastered).
-   **Load from CSV:** Easily import your vocabulary lists from a simple `.csv` file.
-   **Save/Load Progress:** Save your entire session, including scores for each word, into a `.json` file. Load it again later to pick up exactly where you left off.
-   **Dual Audio Pronunciation:** Listen to both **Mandarin** (for the simplified character) and **Cantonese** (for the traditional character) pronunciations using the browser's built-in text-to-speech.
-   **Traditional & Simplified:** Displays both character sets to aid comprehensive learning. The front of the card shows the simplified character, with the traditional form in the corner for reference.
-   **Offline First:** The entire application is a single HTML file. Once loaded, it works completely offline. Your data is never uploaded.
-   **Zero Dependencies:** No need to install anything. Just open the HTML file in a browser.

## How to Use

1.  **Prepare Your Vocabulary List**
    Create a `.csv` file with four columns in the following order: `Simplified`, `Traditional`, `Pinyin`, `English`.
    
    *Example `vocab.csv` file:*
    ```csv
    你,你,nǐ,you
    好,好,hǎo,good
    学,學,xué,to study
    生,生,shēng,life / to be born
    ```

2.  **Download the App**
    Download the `hanzi-trainer.html` file from this repository.

3.  **Start a Session**
    -   Open the `hanzi-trainer.html` file in your web browser (Chrome, Firefox, Safari, etc.).
    -   To start with a new vocabulary list, click **"Start New Session"** and select your `.csv` file.
    -   To enable audio feature, provide your Gemini API key following the steps [here](https://ai.google.dev/gemini-api/docs/api-key)
    -   To continue a previous session, click **"Load Existing Session"** and select your saved `.json` file.

4.  **Study**
    -   Look at the simplified character on the front. The traditional character is in the top right.
    -   Click the card to flip it over and see the details.
    -   Use the audio buttons to hear the Mandarin and Cantonese pronunciations.
    -   Click **"Knew It"** or **"Didn't Know"** to rate your knowledge and move to the next card.

5.  **Save Your Progress**
    When you are done studying, click the **"Save Session"** button. This will download a `chinese_session.json` file containing all your words and their current scores.

## Technologies Used

-   **HTML5**
-   **CSS3**
-   **Vanilla JavaScript (ES6)**
-   **Web Speech API** for text-to-speech functionality.

## Future Ideas

-   Implement the "Commonly Paired With" side panel to show character context.
-   Add support for customizable SRS settings.
-   Integrate a dictionary API to fetch character data automatically.

## License

This project is licensed under the MIT License.
