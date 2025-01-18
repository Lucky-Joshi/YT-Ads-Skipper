# YouTube Ad Skipper

A **Chrome Extension** that automatically skips YouTube ads, ensuring a seamless video-watching experience. It also tracks the number of ads skipped, displaying them as a badge on the extension icon.

---

## Features

- **Automatic Ad Skipping**: Detects ads and skips them automatically.
- **Ad Counter**: Keeps track of the number of ads skipped.
- **Playback Speed Adjustment**: Speeds up ads to minimize interruptions.
- **User-Friendly Interface**: Simple and intuitive design.

---

## How It Works

1. The **background script** initializes the extension and tracks tab updates.
2. The **content script** detects and skips ads on YouTube by interacting with the DOM.
3. A **popup interface** displays the total number of ads skipped.
4. The **badge** on the extension icon dynamically updates with the ad count.

---

## Files Overview

### 1. **manifest.json**
Defines the extension's metadata and permissions.
- Specifies the content script and background service worker.
- Includes permissions for interacting with YouTube and storing data.

### 2. **background.js**
Handles:
- Initialization of storage for ad counts.
- Badge updates to display the number of ads skipped.
- Injecting content scripts into YouTube tabs.

### 3. **content.js**
Core logic for:
- Detecting ads on YouTube.
- Skipping ads and speeding up playback during ads.
- Sending messages to update the ad counter.

### 4. **popup.html**
The user interface for the extension.
- Displays the current status and total ads skipped.
- Styled with a sleek and modern design.

### 5. **popup.js**
Dynamically updates the popup with the latest ad count from local storage.

---

## Installation

1. Clone or download this repository.
2. Go to `chrome://extensions/` in your Chrome browser.
3. Enable **Developer Mode** (toggle in the top-right corner).
4. Click on **Load Unpacked** and select the folder containing the project files.
5. The extension is now installed and active.

---

## Usage

1. Navigate to YouTube and start watching videos.
2. The extension will automatically detect and skip ads.
3. Open the extension popup to view the total ads skipped.

---

## Contributing

Contributions are welcome! Feel free to fork this repository and submit pull requests.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Acknowledgments

- Inspired by the need for uninterrupted YouTube experiences.
- Built using Chrome Extension APIs.

