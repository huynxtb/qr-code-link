# QR Code Generator

A clean, single-file QR code generator that runs entirely in the browser. Paste a link (or other content), customize the look, and download a print-ready PNG. No build step, no server, no data leaves your machine.

## Features

- **Multiple QR types**
  - Link / URL
  - Contact card (vCard)
  - Wi-Fi network (WPA/WPA2, WEP, or open)
  - Email (with optional subject & body)
  - Phone number
  - SMS (with optional message)
  - Plain text
- **Customization**
  - Module styles: Rounded, Dots, Classic
  - Color palette of presets
  - Center mark: none, built-in glyphs (scan, link, @, code, person, phone, mail), or your own uploaded image / emoji
  - Optional caption rendered below the code
- **Smart error correction** — automatically uses a higher error-correction level when a center mark is present, so the code stays scannable.
- **Download** as a high-resolution PNG.
- **Fully client-side** — content is encoded locally in the browser; nothing is uploaded.

## Usage

1. Open `qr-generator.html` in any modern web browser (double-click it, or serve the folder).
2. Choose a **QR type** and fill in the details.
3. Tweak the style, color, center mark, and caption as desired.
4. Scan-test with your phone, then click **Download PNG**.

> Tip: always scan-test the generated code before printing.

## Tech

- Single self-contained HTML file (`qr-generator.html`) — markup, styles, and logic in one place.
- [qrcodejs (qrcode 1.5.1)](https://cdnjs.com/libraries/qrcode) loaded from a CDN for QR matrix generation.
- HTML5 Canvas for rendering the styled code, center marks, and caption.

The only external dependency is the qrcode library pulled from a CDN, so an internet connection is required on first load.

## Project structure

```
qr-code-link/
└── qr-generator.html   # the entire app
```

## License

No license specified.
