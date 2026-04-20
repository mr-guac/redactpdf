# RedactPDF

A free, private PDF redaction tool that runs entirely in your browser. No upload, no account, no server.

🔗 **Live at [redactpdf.net](https://redactpdf.net)**

## How it works

Most free PDF redaction tools upload your file to their servers and draw black rectangles over text — the underlying data is still there and can be recovered by anyone who removes the rectangle layer.

RedactPDF works differently:

1. Your PDF is loaded entirely in your browser using [PDF.js](https://mozilla.github.io/pdf.js/)
2. You draw redaction boxes over sensitive content
3. On download, each page is rasterized to a PNG image with your redactions burned in
4. A new PDF is rebuilt from those images using [pdf-lib](https://pdf-lib.js.org/)
5. The text layer is permanently destroyed — not just covered

Your file never leaves your device. There is no server.

## Usage

### Online
Visit [redactpdf.net](https://redactpdf.net) — no installation required.

### Offline
Download `redactpdf.html` and open it in any modern browser. Works offline after the libraries have been cached on first load.

> **Note:** This tool loads PDF.js and pdf-lib from CDN. A one-time internet connection is required on first load for the libraries to cache. Fully offline air gapped environments with no internet access are not currently supported.

## Features

- ✅ True redaction — text layer permanently destroyed, not just covered
- ✅ Multi-page PDF support
- ✅ No file size or page count limits
- ✅ No upload — 100% client-side processing
- ✅ No account or signup required
- ✅ Works offline after initial load
- ✅ Free forever

## Tech stack

- [PDF.js](https://mozilla.github.io/pdf.js/) by Mozilla — PDF rendering
- [pdf-lib](https://pdf-lib.js.org/) — PDF generation
- Vanilla HTML, CSS, JavaScript — no frameworks

## Disclaimer

This tool is provided as-is for general use. You are solely responsible for verifying that all sensitive information has been fully and correctly redacted before sharing any document. Always review your output before distributing. This tool makes no guarantees that redactions meet any specific legal, regulatory, or compliance standard. For legally sensitive documents consult a qualified professional.

## License

MIT — free to use, modify, and distribute.

## Contributing

Pull requests welcome. Keep it simple — this is intentionally a single file tool.
