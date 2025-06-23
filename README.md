# Shortcuts.js

**The easiest way to add keyboard shortcuts and a command palette to your website.**  
Minimal, elegant, and dependency-free.

---

## 🚀 Overview

`Shortcuts.js` is a lightweight JavaScript library (under 10KB) that lets you register keyboard shortcuts with just one line of code — and includes a beautiful built-in **Command Palette** to show all available shortcuts to your users.

Designed with accessibility, responsiveness, and developer happiness in mind.  

---

## ✨ Features

- ⚡ **Fast & lightweight** – <10KB minified, no dependencies.
- 🎹 **Custom keyboard shortcuts** – Support for `Ctrl`, `Cmd`, `Alt`, `Shift` combos.
- 🧭 **Built-in shortcut guide** – Open with `Cmd + ?` or trigger programmatically.
- 🎨 **Dark mode ready** – Adapts automatically or via CSS variables.
- 🛠️ **Easy to use** – Just call `Shortcuts.register()` and you're done.
- ♿ **Accessible** – Fully navigable with keyboard and screen readers.

---

## 🔧 Installation

### CDN

```html
<script src="https://unpkg.com/shortcuts.js"></script>
<link rel="stylesheet" href="https://unpkg.com/shortcuts.js/styles.css" />
````

### NPM

```bash
npm install shortcuts.js
```

Then:

```js
import Shortcuts from 'shortcuts.js';
import 'shortcuts.js/styles.css';
```

---

## 🧠 Usage

```js
// Register a shortcut
Shortcuts.register('Cmd+K', () => {
  alert('Command palette opened!');
}, 'Open Command Palette');

// Show the shortcut guide manually
Shortcuts.showHelp();
```

> 🔍 Tip: Users can press `Cmd + ?` (Mac) or `Ctrl + ?` (Windows) to see the list of shortcuts.

---

## 🧩 API

### `Shortcuts.register(keys, callback, description)`

Registers a new shortcut.

| Param         | Type     | Description                     |
| ------------- | -------- | ------------------------------- |
| `keys`        | `string` | Shortcut combo, e.g. `'Ctrl+S'` |
| `callback`    | `fn`     | Function to run on key press    |
| `description` | `string` | Description for help modal      |

### `Shortcuts.unregister(keys)`

Unregisters an existing shortcut.

### `Shortcuts.showHelp()`

Shows the interactive help modal.

### `Shortcuts.clear()`

Removes all registered shortcuts.

---

## 🎨 Styling

Customize the command palette via CSS variables:

```css
:root {
  --shortcuts-bg: #1a1a1a;
  --shortcuts-text: #fff;
  --shortcuts-accent: #00e0b8;
}
```

---

## 📦 Folder Structure

```
shortcuts.js/
├── shortcuts.js       # Main library file
├── styles.css         # Default styles for modal
├── examples/
│   └── index.html     # Basic usage demo
├── README.md
└── package.json
```

---

## 🌍 Browser Support

✅ Chrome
✅ Firefox
✅ Safari
✅ Edge
✅ Brave
✅ Mobile browsers

---

## 📜 License

MIT — Free to use, modify and distribute.
Made with ❤️ by [@holasoymalva](https://github.com/holasoymalva)

---

## ⭐ Star it if you like it!

If you find this project useful, consider giving it a ⭐ on GitHub and sharing it with your dev friends. Every bit of support helps!
