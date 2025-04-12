# Teams Chat Viewer

A lightweight, fully client-side HTML application to view exported Microsoft Teams chat history with media support.

## 📦 Features

- Load and parse `messages.json` exported from Microsoft Teams
- Display conversations and messages in a clean chat-like interface
- Supports:
  - Group and 1-on-1 conversations
  - Rich-text messages
  - Embedded images via `amsreferences`
- Distinguish sender and receiver messages with styled bubbles
- Display user initials or avatars (if available)
- Group messages by date
- No server or upload — everything runs locally in your browser

## 🛠 How to Use

1. Export your Teams chat data from Microsoft [here](https://go.microsoft.com/fwlink/?linkid=2128346).
2. Extract the `.tar` archive and locate:
   - `messages.json`
   - The `media/` folder containing `.json` and image files
3. Open `index.html` in a browser (Chrome/Edge recommended).
4. Use the file input to select:
   - `messages.json`
   - All `.json` metadata files from the `media/` folder
5. Conversations will appear on the left. Click one to view its messages.

> Note: Due to browser security restrictions, double-clicking to open `index.html` may not allow local file reading. **Use a simple HTTP server (e.g., Python, Node.js)** or drag-and-drop into a secure localhost environment.

## 🧱 Project Structure

