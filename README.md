# richtext.js

A lightweight, custom rich text editor built in **vanilla JavaScript** using `contenteditable`, designed for fine-grained control over cursor tracking, Markdown formatting, and undo/redo history.

This is a personal side project, currently a work in progress, being developed independently in native JavaScript. It is intended to be integrated into Rocket.Chat as part of a planned Composer overhaul during Google Summer of Code (GSoC) 2025.

---

## ✨ Features (in progress)

- ✅ Real-time Markdown-style formatting (`*bold*`, `_italic_`, `~strikethrough~`, etc.)
- 🎯 Precise cursor tracking and position monitoring
- ⏪ Undo/Redo via custom input history stack
- 🔁 Input state detection and change tracking
- ⌨️ Keyboard-driven editing (`Enter`, `Backspace`, `Delete`)
- 🪄 Handles complex formatting input edge cases

---

## 🛠️ Project Status

This is an **experimental build** focused on exploring low-level editor internals using the DOM Selection API and manually managed formatting rules.

Eventually, this system will form the basis of a **rich-text editing experience inside Rocket.Chat's message composer**, enabling Markdown previews, smart formatting, and potentially collaborative input features.

---

## 🔧 Usage

1. Clone the repo or copy the HTML + script section.
2. Open `index.html` in your browser.
3. Start typing with Markdown-style syntax:
   - `*bold*`
   - `_italic_`
   - `~strikethrough~`
   - Combined: `*_~boldItalicStrikethrough~_*`.

---

## 📌 Notes

- Cursor and selection logic is manually handled via `getSelection()` and `Range`.
- Markdown symbols are visually preserved using `<span>` wrappers.
- No external libraries or frameworks used — pure HTML + JS.

## 📸 Screenshots

![image](https://github.com/user-attachments/assets/c499b893-21a7-447c-bb78-6155ac8a41c8)
