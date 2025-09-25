# Simple XLIFF Editor

A dead-simple, **client-side-only** web application for viewing, editing, and saving XLIFF files of all versions (1.x and 2.x) in a familiar, easy-to-use tabular format.

This tool is built entirely with **HTML, CSS, and vanilla JavaScript**, meaning **no data ever leaves your browser**. It's fast, private, and requires zero server-side setup.

---

## 🚀 Live Demo

See it in action right now!

🔗 **[Launch the Simple XLIFF Editor](https://mrmadhav.github.io/xliff-editor/)**

---

## ✨ Features

* **100% Client-Side:** All file parsing and editing happens directly in your browser. No backend, no databases, and maximum privacy.
* **XLIFF Version Agnostic:** Supports both older **XLIFF 1.x** and modern **XLIFF 2.x** formats by correctly identifying and extracting translatable units (`<trans-unit>` and `<unit>`).
* **Intuitive Table View:** Displays **Source**, **Target**, and **Note** fields in a clean, tabular format, mimicking the experience of professional CAT tools.
* **In-Place Editing:** Simply click on any **Target** cell and start typing to modify the translation directly.
* **Quick Download:** A single button click downloads the original file with your edits saved, maintaining all original XLIFF metadata.

---

## 🖥️ How It Works

1.  **Upload:** Click "Choose File" and select an `.xlf` or `.xliff` file.
2.  **Parse:** The JavaScript uses the `DOMParser` to read the XML content and identifies all translatable units.
3.  **Edit:** The table is populated, and the **Target** column is made **`contenteditable`** for direct editing.
4.  **Save:** When you click "Download Edited XLIFF," the tool uses the **`XMLSerializer`** to update the original XML structure with your new translations and triggers a direct browser download.

---

## 🛠️ Technology Stack

| Technology | Purpose |
| :--- | :--- |
| **HTML5** | Structure and File Input |
| **CSS3** | Styling (Simple, Clean UI) |
| **Vanilla JavaScript** | File Reading (`FileReader`), XML Parsing (`DOMParser`), DOM Manipulation, and File Download (`Blob` API). |

---

## 💡 Contribution

This project is intended to be a simple, lightweight utility. If you find a bug, particularly with specific XLIFF structures, or have an idea for a non-server-side enhancement, please feel free to:

1.  **Open an Issue:** Describe the bug or feature request clearly.
2.  **Fork the Repository:** Submit a Pull Request with your suggested changes.
