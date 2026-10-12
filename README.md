# QR Code Generator

A browser-based QR code generator. Enter any text or URL, customize the appearance, and download the result as a PNG — no server, no sign-up, no API key required.

## Features

- Generate QR codes from any text or URL
- Adjustable output size (128, 256, 512, 1024 px)
- Four error-correction levels (L, M, Q, H)
- Custom foreground and background colors
- Live color preview
- One-click PNG download
- Keyboard shortcut: `Ctrl + Enter` (or `Cmd + Enter`) to generate
- Fully client-side — nothing is uploaded anywhere

## Tech Stack

- HTML5
- CSS3 (custom properties, grid, flexbox)
- Vanilla JavaScript
- [qrcodejs](https://github.com/davidshimjs/qrcodejs) via CDN
- Canvas API for PNG export

## How to Run

1. Clone or download this folder.
2. Open `index.html` in any modern browser.
3. Type your text or URL, adjust the settings, and click **Generate QR Code**.
4. Click **Download PNG** to save the image.

No build step, no dependencies to install.

### Optional: run with Live Server in VS Code

1. Install the **Live Server** extension.
2. Right-click `index.html` → **Open with Live Server**.

## How It Works

The app uses the `qrcodejs` library to render the QR code onto a canvas element. The **Download PNG** button reads that canvas with `toDataURL()` and triggers a client-side download. All logic runs in the browser — the page can work fully offline once the library is cached or saved locally.

## File Structure
qr-code-generator/
├── index.html
└── README.md

text

## License

Free to use for personal and educational purposes.