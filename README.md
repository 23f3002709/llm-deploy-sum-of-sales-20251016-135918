# Sum of Sales (Data URI CSV) — Single-Page Web App

A production-ready, static single-page application that decodes an embedded CSV (via data URI), parses it, sums the `sales` column, and displays the total in the `#total-sales` element. Built with Bootstrap 5 and works on GitHub Pages without any backend.

## Features
- Parses embedded CSV from a data URI (no external requests required)
- Sums the `sales` column and displays the result in `#total-sales`
- Clean, responsive UI built with Bootstrap 5
- Dataset preview table rendered on the page
- Robust error handling and graceful fallbacks
- Fully static: suitable for GitHub Pages

## Getting Started
- No build step or server required.
- Simply open `index.html` in any modern browser.

## Usage
1. Open `index.html`.
2. The app will decode the embedded CSV, parse it, and compute the sum of the `sales` column.
3. The computed total appears in the `Total Sales` card (element ID: `#total-sales`).
4. The dataset preview is shown in the table on the right.

## Technical Overview
- Libraries:
  - Bootstrap 5 (CSS/JS) via CDN
- Attachments:
  - `data.csv` is embedded as a data URI inside the JavaScript. The app decodes base64 with `atob`, parses the CSV, and computes totals.
- Code Structure:
  - All code is contained within `index.html`:
    - Inline CSS in `<style>`
    - Inline JavaScript in `<script>`
    - Constants for data URIs
    - Functions: `decodeBase64DataUri`, `parseCsvAndSum`, `renderTable`, `showError`
- Error Handling:
  - If parsing fails, a visible alert is shown and `#total-sales` falls back to `0`.

## Deployment
- This project is fully static and works on GitHub Pages.
- You can host it by uploading the files to any static host or by using GitHub Pages.
- For local use, just open `index.html` directly in your browser.

## License
MIT License

Copyright (c) 2025

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
