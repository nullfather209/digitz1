# Button Phone (prototype)

A small keyboard-first web app shell inspired by Cloud Phone's D-pad navigation patterns.

## What it does
- D-pad Up/Down (and Left/Right as previous/next) moves the selection.
- Enter opens the selected menu item.
- Escape / Backspace returns to the home menu.
- Number keys 1–9 select menu entries directly.
- Key tester displays `event.key`, `event.code`, `keyCode`, and repeat state.
- Includes basic Notes and Calculator mini apps, plus a few external web links.
- Can be hosted as a static website and installed as a PWA where supported.

## Important limitations
- This is a browser app, not an Android launcher or a replacement for Android's input system.
- It only works with physical keys that the browser receives as DOM keyboard events.
- It cannot make native Android apps keypad-compatible.
- External websites may still be touch-first or intercept navigation differently.
- Notes text entry depends on whether the phone's keypad/IME sends text input to the browser.

## Try it
1. Open `index.html` in a modern browser, or host this folder on any static HTTPS host (for example, GitHub Pages).
2. Open **Key tester** and press the phone's physical D-pad, center/select, Back, Call/End, and number keys.
3. Note the exact `key` and `code` values shown. Those values determine how to map the phone's keys reliably.

No build step or external JavaScript dependencies are required.
