# 📚 Notes Manager

> A OneNote-style local notes manager built with HTML, CSS, and JavaScript.  
> Organize your `.docx`, `.pdf`, and `.one` files into **Notebooks → Sections → Pages** — all stored locally, no account needed.
# link :- https://shadowknight711.github.io/notes-manager/


---

## ✨ Features (v1.0.0)

| Feature | Details |
|---|---|
| 📓 Notebooks | Create multiple notebooks with custom emoji icons |
| 🗂 Sections | Color-coded sections inside each notebook |
| 📄 Pages | Upload `.docx`, `.pdf`, or `.one` files as pages |
| 🌙 Dark Mode | Full dark theme, saved across sessions |
| ◀▶ Collapsible panels | Hide/show rail, sections, and pages panels independently |
| 💾 Save & Load | Export to `.notesbook` file; re-import with Merge or Replace |
| 🗑 Reset | Clear all data safely with confirmation |
| 📦 No size limits | Uses IndexedDB instead of localStorage — handles large files |

---

## 🌐 Use in Browser

No installation needed. Just open `index.html` directly in your browser:

1. Download or clone this repo
2. Open `index.html` in Chrome, Edge, or Firefox
3. Start adding notebooks and uploading files

> **Note:** All data is saved in your browser's IndexedDB. Clearing browser data will erase your notes — use **💾 Save** regularly to back up your `.notesbook` file.

---

## 📁 Project Structure

```
notes-manager/
├── index.html           # App — all HTML, CSS, and JS in one file
├── LICENSE              # MIT License
├── CHANGELOG.md         # Version history
└── .gitignore
```

---

## 📖 How to Use

### 1. Create a Notebook
Click **＋** in the left rail → pick an emoji and give it a name (e.g. "Biology").

### 2. Add Sections
Click **＋ Add section** in the sections panel → pick a color and name (e.g. "Chapter 1").

### 3. Upload Pages
Click **⬆ Add Page** → select one or more `.docx`, `.pdf`, or `.one` files → assign to a notebook and section.

### 4. Save Your Notes
Click **💾 Save** to download a `.notesbook` backup file. To restore on a different browser or device, click **📂 Load**.

### 5. Collapse Panels
Click the **◀** arrow tabs on the right edge of any panel to collapse it. Click **☰** in the topbar to restore all panels at once.

---

## ⚠️ OneNote (.one) Files

Notes Manager does a best-effort text extraction from `.one` binary files. This works for most simple notes but:
- Embedded images, drawings, and complex layouts are not supported
- Files over 20 MB are skipped (shows a message instead)
- For best results, **export from OneNote as PDF or DOCX** before importing

---

## 🔒 Privacy

All your notes stay **entirely on your device**. Nothing is uploaded to any server. The app has no analytics, no telemetry, and no network requests beyond loading two open-source libraries (mammoth.js for DOCX, pdf.js for PDF) on first load.

---

## 🛠 Tech Stack

- **HTML + CSS + JavaScript** — no framework, single file
- **[mammoth.js](https://github.com/mwilliamson/mammoth.js)** — DOCX → HTML conversion
- **[pdf.js](https://mozilla.github.io/pdf.js/)** — PDF rendering
- **IndexedDB** — local storage with no size limits

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first.

1. Fork the repo
2. Create a branch: `git checkout -b feature/my-feature`
3. Commit: `git commit -m 'Add my feature'`
4. Push: `git push origin feature/my-feature`
5. Open a Pull Request

---

## 📄 License

[MIT](LICENSE) © 2025 Kevin Jose
