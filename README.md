# Scripture Splitter Tool (BKIM Ministry)
### By Joel Deroche
This tool splits a scripture reference into manageable episodes based on user-defined reading speed and maximum reading time per episode. The tool uses the Bible API to fetch scripture text and dynamically generates episodes, allowing customization of episode numbering, reading speed, and more. 

---

## Features

- Fetch scripture text automatically using a Bible API.
- Split scripture into episodes based on reading speed and time limits.
- Option to include or hide scripture text in episodes dynamically.
- Customize episode numbering starting point.
- Displays metadata for each episode, such as word count, estimated reading time, and verse range.

---

## Installation and Usage

### 1. Requirements

- A modern web browser (e.g., Chrome, Firefox, Edge).
- Internet connection (for fetching scripture from the Bible API).

### 2. How to Use

1. **Clone or Download the Tool:**
   - Save the provided HTML file to your local machine.

2. **Open the Tool:**
   - Open the HTML file in your web browser.

3. **Set Parameters:**
   - **Scripture Reference:** Enter the scripture reference you want to split (e.g., `1 Samuel 15`).
   - **Reading Speed (Words per Second):** Set your reading speed (default: 4 words per second).
   - **Maximum Time Per Episode (Seconds):** Specify the maximum time you want to spend reading each episode (default: 90 seconds).
   - **Starting Episode Number:** Define the number for the first episode (default: 1).

4. **Fetch and Split Scripture:**
   - Click **"Fetch and Split Scripture"** to retrieve and process the scripture.

5. **Toggle Scripture Visibility:**
   - Use the **"Toggle Scripture Visibility"** button to show or hide the scripture text in all episodes.

---

## Example

### Input:
- **Scripture Reference:** `1 Samuel 15`
- **Reading Speed:** `4 words per second`
- **Max Time:** `60 seconds`
- **Starting Episode Number:** `5`

### Output:
- The tool splits the scripture into episodes such as:
  - **Episode 5:** 350 words, ~87.5 seconds, Verses: 15:1–15:10.
  - **Episode 6:** 360 words, ~90 seconds, Verses: 15:11–15:20.

Each episode will contain:
- A title with the episode number.
- Metadata including the word count, reading time, and verse range.
- The scripture text (optionally hidden).

---

## API Integration

The tool uses the [Bible API](https://bible-api.com/) to fetch scripture data. The scripture reference entered (e.g., `1 Samuel 15`) is sent as a query to the API, and the resulting JSON response is parsed to extract verses and chapter information.

---

## Known Limitations

1. The Bible API may have limited support for certain translations or scripture references.
2. Requires an internet connection to fetch scripture.

---

## Future Improvements

- Add support for multiple Bible translations.
- Allow saving episodes as a downloadable file.
- Provide advanced formatting options for episodes.

---

## Troubleshooting

1. **Error: "Failed to fetch scripture":**
   - Ensure the scripture reference is correctly formatted (e.g., "1 Samuel 15").
   - Verify your internet connection.

2. **Episodes are not splitting as expected:**
   - Check if the reading speed and max time values are appropriate.
   - Ensure the scripture reference has enough content to split.

For further assistance, feel free to ask for clarifications!
