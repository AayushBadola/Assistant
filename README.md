
# 🚀 Advanced Browser-Based Voice Assistant 🎙️

[![Language: HTML5](https://img.shields.io/badge/Language-HTML5-E34F26?style=for-the-badge&logo=html5)](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/HTML5)
[![Language: CSS3](https://img.shields.io/badge/Language-CSS3-1572B6?style=for-the-badge&logo=css3)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![Language: JavaScript](https://img.shields.io/badge/Language-JavaScript-F7DF1E?style=for-the-badge&logo=javascript)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg?style=for-the-badge)](https://github.com/AayushBadola)
[![Platform: Browser](https://img.shields.io/badge/Platform-Browser-lightgrey.svg?style=for-the-badge)](https://developer.mozilla.org/en-US/docs/Web/API)

---

## ✨ Overview

Welcome to the **Advanced Browser-Based Voice Assistant**! This project demonstrates a sophisticated voice assistant that runs entirely within your web browser using standard Web APIs. It leverages the power of the **Web Speech API** (`SpeechRecognition` and `SpeechSynthesis`) along with various external APIs to provide a wide range of functionalities without requiring any backend server setup for its core operation. Just open the HTML file and start interacting!

This assistant can understand your voice commands, perform actions like fetching information, managing simple tasks, controlling the page, and responding back with synthesized speech.

---

## 🌟 Features

This assistant boasts a wide array of capabilities:

*   🗣️ **Voice Command Recognition:** Listens and interprets spoken commands.
*   🔊 **Speech Synthesis:** Provides spoken feedback and responses.
*   🕰️ **Time & Date:** Get the current time and date.
*   🤣 **Jokes & Facts:** Tells jokes and random interesting facts.
*   🌐 **Web Search & Navigation:**
    *   Open Google, YouTube, News.
    *   Perform Google searches for specific queries.
    *   Basic page navigation (back, forward, reload).
    *   Scroll page up/down.
    *   Enter/Exit fullscreen mode.
*   ☀️ **Weather Information:** Fetches current weather for any city using the [OpenWeatherMap API](https://openweathermap.org/api).
*   🧮 **Basic Calculations:** Evaluates simple mathematical expressions.
*   ⏲️ **Timers:** Set countdown timers with optional desktop notifications (requires permission).
*   📝 **Notes Management:** Add, read, and clear simple notes stored in `localStorage`.
*   ✅ **To-Do List:** Manage a persistent to-do list (add, read, mark done, clear) stored in `localStorage`.
*   📖 **Dictionary Definitions:** Look up word definitions using the [DictionaryAPI.dev](https://dictionaryapi.dev/).
*   🌍 **Wikipedia Summaries:** Fetch introductory summaries for topics from Wikipedia.
*   📋 **Clipboard Control:** Copy the assistant's last response to the clipboard (requires secure context).
*   🎲 **Random Generators:** Flip a coin, roll dice (custom sides), generate random numbers.
*   🎨 **Theme Control:** Toggle between light and dark themes for the assistant page.
*   📄 **Page Text Search:** Find text within the current HTML page (`window.find`).
*   🔗 **Conversion Links:** Open Google search for currency/unit conversions.
*   🎤 **Voice Listing:** List available speech synthesis voices in the browser console.
*   👤 **Personalization:** Remembers and recalls the user's name (using `localStorage`).

---



## 🚀 Getting Started

There are two main ways to get the code:

**Option 1: Cloning the Repository (Recommended for developers)**

1.  Ensure you have [Git](https://git-scm.com/downloads) installed on your system.
2.  Open your terminal or command prompt.
3.  Navigate to the directory where you want to store the project.
4.  Clone the repository using the following command:
    ```bash
    git clone https://github.com/AayushBadola/Assistant.git
    ```

5.  Navigate into the newly created directory:
    ```bash
    cd Assistant
    ```

**Option 2: Downloading the ZIP File**

1.  Go to the GitHub repository page: [https://github.com/AayushBadola/Assistant](https://github.com/AayushBadola/Assistant) 
2.  Click the green `<> Code` button.
3.  Select `Download ZIP`.
4.  Extract the contents of the downloaded ZIP file to a location on your computer.

---

## ▶️ How to Run

Once you have the code locally:

1.  **Locate the HTML File:** Find the main `.html` file (e.g., `index.html`, `new.html`, or `voice_assistant.html`) within the project directory.
2.  **Open in Browser:**
    *   **Double-click** the HTML file. It should open in your default web browser.
    *   *Alternatively*, **right-click** the file, select "Open With", and choose a compatible browser (Chrome, Edge, Firefox recommended).
    *   *Alternatively*, open your browser and use the `File -> Open File...` menu option to navigate to and select the `.html` file.
3.  **Grant Permissions:**
    *   🎤 **Microphone:** The *first time* you click the "Start Listening" button, your browser will request **permission to use your microphone**. You **MUST ALLOW** this for voice recognition to function.
    *   🔔 **Notifications (Optional):** The page might also request permission to **show notifications** (for timer alerts). Allowing this enhances the timer feature, but it's optional.
4.  **Interact:**
    *   Click the `🎙️ Start Listening` button.
    *   Wait for the status to indicate `👂 Listening...`.
    *   Speak a command clearly (e.g., "What's the weather in Paris?", "Add note pick up groceries", "Set timer for 5 minutes").
    *   The assistant will process the command and respond.

---

## 🛠️ Technical Details

*   **Core APIs:**
    *   `Web Speech API (SpeechRecognition & SpeechSynthesis)`
    *   `Fetch API`
    *   `LocalStorage API`
    *   `Notification API`
    *   `Clipboard API`
*   **External APIs Used:**
    *   [OpenWeatherMap](https://openweathermap.org/api)
    *   [DictionaryAPI.dev](https://dictionaryapi.dev/)
    *   [Wikipedia API](https://www.mediawiki.org/wiki/API:Main_page)
*   **Browser Compatibility:** Primarily designed for modern desktop browsers.
    *   ✅ Google Chrome (Recommended)
    *   ✅ Microsoft Edge (Chromium-based)
    *   ⚠️ Mozilla Firefox (May require flags/partial support)
    *   ⚠️ Safari (Support may vary)

---

## ⚙️ Configuration

The assistant requires one external API key for full functionality:

*   **OpenWeatherMap API Key:** This key is necessary for the weather commands.
    *   You need to obtain a free API key from [OpenWeatherMap](https://openweathermap.org/appid).
    *   Once you have the key, locate the following line within the `<script>` section of the main HTML file:
        ```javascript
        const OPENWEATHERMAP_API_KEY = 'YOUR_API_KEY_HERE'; // Replace this placeholder
        ```
    *   Replace `'YOUR_API_KEY_HERE'` with the actual API key you obtained.

> **⚠️ Security Note:** Even though the key isn't listed *here*, remember that embedding API keys directly in client-side JavaScript makes them visible to anyone viewing the page source. Be mindful of usage limits associated with your key. For projects requiring higher security or shared deployment, manage API keys server-side.

---

## 📜 Command List

Here is a list of commands the assistant currently understands. Commands are generally case-insensitive.

<details>
<summary><strong>Click to Expand/Collapse Command List</strong></summary>

| Category        | Command Examples                                       | Description                                                              |
| :-------------- | :----------------------------------------------------- | :----------------------------------------------------------------------- |
| **🗣️ Basic**    | `Hello`, `Hi`, `Hey`                                   | Greets the user (personalizes if name is known).                         |
|                 | `How are you?`                                         | Reports its status.                                                      |
|                 | `What's your name?`, `Who are you?`                    | States its name.                                                         |
|                 | `Thank you`, `Thanks`                                  | Responds politely.                                                       |
|                 | `Goodbye`, `Bye`                                       | Says goodbye.                                                            |
| **🕒 Info**      | `Time`, `What's the time?`                             | Tells the current time.                                                  |
|                 | `Date`, `What's today's date?`                         | Tells the current date.                                                  |
|                 | `Weather in [City]`, `What's the weather in [City]?` | Fetches and speaks the current weather for the specified city.         |
|                 | `Define [Word]`, `What does [Word] mean?`              | Looks up and speaks the definition of a word.                            |
|                 | `Wikipedia [Topic]`, `Tell me about [Topic]`           | Looks up and reads a summary of the topic from Wikipedia.              |
| **🧮 Calculate** | `Calculate [Expression]`, `What is 5 plus 5?`          | Evaluates a mathematical expression (e.g., `5*8`, `100/4`, `2 power 8`). |
| **🌐 Browser**   | `Open Google/YouTube/News`                             | Opens the respective website in a new tab.                               |
|                 | `Search for [Query]`, `Google [Query]`                 | Performs a Google search for the query in a new tab.                     |
|                 | `Scroll down`, `Page down`                             | Scrolls the current page down.                                           |
|                 | `Scroll up`, `Page up`                                 | Scrolls the current page up.                                             |
|                 | `Go back`, `Previous page`                             | Navigates to the previous page in history.                               |
|                 | `Go forward`, `Next page`                              | Navigates to the next page in history.                                   |
|                 | `Reload page`, `Refresh page`                          | Reloads the current page.                                                |
|                 | `Full screen`, `Enter fullscreen`                      | Attempts to enter fullscreen mode.                                       |
|                 | `Exit fullscreen`, `Minimize`                          | Exits fullscreen mode if active.                                         |
|                 | `Find on page [Text]`, `Search this page for [Text]` | Highlights occurrences of the text on the current page.                  |
|                 | `Convert [Amount] [Unit1] to [Unit2]`                  | Opens Google search for the specified conversion (e.g., `Convert 10 USD to EUR`). |
| **⏲️ Timer**     | `Set timer for [Number] [Unit]` (seconds/minutes/hours) | Sets a countdown timer (e.g., `Set timer for 10 minutes`).             |
|                 | `Cancel timer`, `Clear timers`                         | Cancels all active timers.                                               |
|                 | `Enable notifications`                                 | Prompts the user for notification permission if not already granted/denied. |
| **📝 Notes**     | `Add note [Content]`, `Note down [Content]`            | Saves a note.                                                            |
|                 | `Read my notes`, `Show notes`                          | Reads out all saved notes.                                               |
|                 | `Clear my notes`, `Delete all notes`                   | Deletes all saved notes.                                                 |
| **✅ To-Do**     | `Add to do [Task]`, `Add task [Task]`                  | Adds an item to the to-do list.                                          |
|                 | `Read my to do list`, `Show my tasks`                  | Reads out incomplete to-do items.                                        |
|                 | `Mark [Item] done`, `Check off [Item]`                 | Marks a specific to-do item as completed (match by number or text).      |
|                 | `Clear to do list`, `Clear all tasks`                  | Deletes the entire to-do list.                                           |
|                 | `Clear completed tasks`, `Remove done items`           | Removes only the completed items from the list.                          |
| **👤 Personal**  | `My name is [Name]`                                    | Saves the user's name.                                                   |
|                 | `What's my name?`, `Say my name`                       | Recalls the saved user name.                                             |
|                 | `Forget my name`                                       | Deletes the saved user name.                                             |
| **🎲 Fun**       | `Joke`, `Tell me a joke`                               | Tells a programmed joke.                                                 |
|                 | `Fact`, `Tell me something interesting`                | Tells a random fact.                                                     |
|                 | `Flip a coin`                                          | Simulates a coin flip.                                                   |
|                 | `Roll a die`, `Roll the dice`                          | Rolls a standard 6-sided die.                                            |
|                 | `Roll a D[Number]` (e.g., `Roll a D20`)                | Rolls a die with the specified number of sides.                          |
|                 | `Random number`                                        | Gets a random number between 1 and 100.                                  |
|                 | `Random number between [Min] and [Max]`                | Gets a random number within the specified range.                         |
| **📋 Control**   | `Copy that`, `Copy last response`                      | Copies the assistant's last spoken text to the clipboard.                |
|                 | `Change theme`, `Toggle theme`                         | Switches between the light and dark UI themes.                           |
|                 | `List voices`, `Available voices`                      | Lists some available TTS voices in the console and speaks the count.     |

</details>

---

## 🤔 Troubleshooting

*   **Assistant doesn't hear me / "No speech detected":**
    *   Ensure you allowed microphone permission.
    *   Check microphone connection, OS settings, and mute status.
    *   Speak clearly, closer to the mic, or in a quieter room.
    *   Reload the page.
*   **Weather/Dictionary/Wikipedia commands fail:**
    *   Check internet connection.
    *   **Verify you have correctly inserted your OpenWeatherMap API key into the HTML file as described in the Configuration section.**
    *   External APIs might be down or rate-limiting. Check the browser's developer console (`F12` -> Console) for errors.
*   **Notifications don't appear:**
    *   Ensure notification permission was granted. Check browser/OS settings if previously denied.
    *   Check OS notification/focus assist settings.
*   **Some commands don't work:**
    *   Use a compatible browser (Chrome/Edge recommended).
    *   Check the developer console (`F12` -> Console) for JavaScript errors.
    *   Ensure your command matches the expected patterns.

---

## 🤝 Contributing

Contributions are welcome!

1.  **Fork** the repository.
2.  Create a **Branch** (`git checkout -b feature/AmazingFeature`).
3.  **Commit** your Changes (`git commit -m 'Add some AmazingFeature'`).
4.  **Push** to the Branch (`git push origin feature/AmazingFeature`).
5.  Open a **Pull Request**.

Alternatively, open an **Issue** with the tag "enhancement" or "bug".

---

## 📜 License

Distributed under the MIT License. See `LICENSE` file for more information (or refer to standard MIT license text).

---

## 👨‍💻 Author & Contact

*   **Author:** Aayush Badola
*   **GitHub:** [![GitHub Badge](https://img.shields.io/badge/-AayushBadola-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/AayushBadola)
*   **LinkedIn:** [![LinkedIn Badge](https://img.shields.io/badge/-Aayush%20Badola-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/aayush-badola-0a7b2b343/)
*   **Email:** [![Email Badge](https://img.shields.io/badge/-aayush.badola2@gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:aayush.badola2@gmail.com)

---

<p align="center">
  <img src="https://img.shields.io/badge/Made%20with-❤️-red?style=flat-square" alt="Made with Love"/>
  &nbsp;&nbsp;&nbsp;&nbsp;
  <img src="https://img.shields.io/badge/Powered%20by-☕-brown?style=flat-square" alt="Powered by Coffee"/>
</p>

