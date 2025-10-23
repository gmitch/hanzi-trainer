# Hanzi Trainer

A powerful, multi-deck flashcard application for memorizing Chinese characters (Hanzi). This tool uses a Spaced Repetition System (SRS) and saves your progress automatically, right in your browser.

## How to Use

### 1. Live App (Recommended)

You don't need to download or install anything. Just use the live version:

➡️ **[Open the Hanzi Trainer App](https://gmitch.github.io/hanzi-trainer/hanzi-trainer.html)**

---

### 2. Download or Clone

You can also run the project from your local computer.

* **Clone the Repo:**
    `git@github.com:gmitch/hanzi-trainer.git`
    Then, open the `hanzi-trainer.html` file in your browser.

* **Download Directly:**
    You can [download the `hanzi-trainer.html` file directly](https://raw.githubusercontent.com/gmitch/hanzi-trainer/main/hanzi-trainer.html) (right-click and "Save As...").

---

## Getting Started: Deck Management

This app is built around a "Deck Manager" that holds all your vocabulary lists.

### 1. Create a Deck

1.  From the main screen, click **"Create New Deck"**.
2.  Give your deck a unique name (e.g., "HSK 1" or "Chapter 3 Verbs").
3.  Upload your vocabulary `.csv` file.

    **CSV Format:** Your file must have four columns in this specific order:
    `Simplified`, `Traditional`, `Pinyin`, `English`
    
    *Example `vocab.csv` file:*
    ```csv
    你,你,nǐ,you
    好,好,hǎo,good
    学,學,xué,to study
    生,生,shēng,life / to be born
    ```
4.  Click **"Create Deck"**. You will be returned to the manager, where you'll see your new deck.

### 2. Open & Study a Deck

* On the main screen, find the deck you want to study and click **"Open"**.
* This will take you to the main flashcard view.
* Click the card to flip it over.
* Use the audio buttons for **Mandarin** and **Cantonese** pronunciations.
* Select **"Knew It"** or **"Didn't Know"** to rate your knowledge.

### 3. Automatic Saving

Your progress (the 1-10 score for each word) is **saved automatically** to your browser's local storage every time you answer a card. There is no "Save" button.

You can close the app at any time. When you re-open that deck, you will pick up right where you left off.

### 4. Manage Your Decks

From the main "Manage Decks" screen, you can:
* **Rename:** Click **"Edit"** to give a deck a new name.
* **Delete:** Click **"Delete"** to permanently remove a deck and all its progress (you will be asked to confirm).

## Features

-   **Multi-Deck Library:** Create, rename, and delete multiple, separate vocabulary decks.
-   **Automatic Progress Saving:** Uses browser `localStorage` to save your scores automatically. No manual saving or loading!
-   **Spaced Repetition System (SRS):** Characters you struggle with appear more frequently. Each word has a score from 1 (new) to 10 (mastered).
-   **Load from CSV:** Easily import your vocabulary lists from a 4-column `.csv` file.
-   **Dual Audio Pronunciation:** Listen to both **Mandarin** (Simplified) and **Cantonese** (Traditional) pronunciations.
-   **Traditional & Simplified:** Displays both character sets to aid comprehensive learning.
-   **Zero Dependencies:** A single HTML file that runs entirely in your browser.

## Technologies Used

-   **HTML5**
-   **CSS3**
-   **Vanilla JavaScript (ES6)**
-   **Web Speech API** (for text-to-speech)
-   **Browser `localStorage`** (for progress saving)

## License

This project is licensed under the MIT License.
