# Awesome No-Upload Tools [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> Free tools that work on your files **inside your browser**, so your PDFs, spreadsheets, photos and data never get uploaded to someone else's server.

Most "free online" file tools upload your file, process it on a server and send the result back. That's fine for a meme, but not for a contract, a payslip, a medical letter or a customer list. Every tool on this list does the work **on your own device**, in the browser, using JavaScript and WebAssembly.

Each entry was checked against the tool's own documentation or privacy terms. Where a tool has exceptions, such as an export or AI feature that does use a server, the note says so.

## Contents

- [How tools are checked](#how-tools-are-checked)
- [PDF](#pdf)
- [Images and photos](#images-and-photos)
- [Documents, spreadsheets and slides](#documents-spreadsheets-and-slides)
- [CSV and data](#csv-and-data)
- [File conversion](#file-conversion)
- [Audio](#audio)
- [Encryption](#encryption)
- [Developer tools](#developer-tools)
- [Diagrams and whiteboards](#diagrams-and-whiteboards)
- [Study, citations and maths](#study-citations-and-maths)
- [Business](#business)
- [SEO and web](#seo-and-web)
- [How to check a tool yourself](#how-to-check-a-tool-yourself)
- [Contributing](#contributing)

## How tools are checked

A tool is listed only if all of these are true:

1. **It's free to use** for the listed job, with no watermark or required sign-up.
2. **Your files are processed on your device.** The tool's own docs, README or privacy terms say so, and we've looked at its network activity where possible.
3. **It runs in a normal web browser,** with no install needed. (Self-hosted server apps are not listed: that's a different kind of privacy.)
4. **Exceptions are disclosed.** If any feature sends data to a server, it's noted.

Open source is marked 🟢. Works offline after the first load is marked ✈️.

## PDF

- [BentoPDF](https://github.com/alam00000/bentopdf) 🟢: a large client-side PDF toolkit for merging, splitting, compressing, converting and editing. Its README says all processing happens in the browser. AGPL-3.0, with a paid licence for closed-source use.
- [Cromagnon PDF Studio](https://cromagnon.app/studios/pdf-studio) ✈️: annotate, sign, true redaction, merge, split, compress, OCR, password-protect and fill forms, all in the browser. Optional AI summaries use your own key and run only when you ask.
- [PDF.js viewer](https://mozilla.github.io/pdf.js/web/viewer.html) 🟢: Mozilla's PDF reader, the one built into Firefox. It opens PDFs entirely in the browser.

## Images and photos

- [miniPaint](https://viliusle.github.io/miniPaint/) 🟢: a layered image editor with filters, crop and drawing tools that opens PNG, JPG, WEBP, GIF and TIFF. Its README says nothing is sent to a server. MIT (per the README).
- [Squoosh](https://squoosh.app) 🟢 ✈️: Google Chrome Labs' image compressor. It compares codecs side by side and processes images locally with WebAssembly.
- [Photopea](https://www.photopea.com) ✈️: a full layered photo editor that opens PSD, XCF, Sketch and more. Its terms say opened files are processed on your own hardware. Its privacy terms don't cover the newer AI features, so treat those separately.
- [Cromagnon Image Studio](https://cromagnon.app/studios/image-studio) ✈️: light, colour, curves and HSL, crop, resize, compress and convert to WEBP or AVIF, with batch export. Masks and background removal run on the device.
- [Cromagnon image compressor](https://cromagnon.app/tools/image-compressor), [converter](https://cromagnon.app/tools/image-converter) and [favicon generator](https://cromagnon.app/tools/favicon-generator): single-job image tools.

## Documents, spreadsheets and slides

- [Cromagnon Document Studio](https://cromagnon.app/studios/document-studio) ✈️: write and edit real DOCX files, with templates, mail merge and compare.
- [Cromagnon Excel Studio](https://cromagnon.app/studios/excel-studio) ✈️: open and edit XLSX files with working formulas, formats, filters and several sheets.
- [Cromagnon Presentation Studio](https://cromagnon.app/studios/presentation-studio) ✈️: open, edit, present and export PowerPoint (PPTX) decks, including to PDF and video.
- [StackEdit](https://stackedit.io/app) 🟢 ✈️: a Markdown editor that keeps documents in the browser's own storage, with export to Markdown, HTML and PDF. Google Drive and Dropbox sync are optional. Apache-2.0.
- [Cromagnon universal file viewer](https://cromagnon.app/tools/universal-file-viewer): open PDF, Word, Excel, slides, images, email and ZIP files without installing anything.

## CSV and data

- [Datasette Lite](https://lite.datasette.io) 🟢: Simon Willison's Datasette running in the browser through Python compiled to WebAssembly (Pyodide). Explore CSV and SQLite files and run SQL on them.
- [DuckDB Wasm shell](https://shell.duckdb.org) 🟢: the DuckDB analytics database in the browser. Query CSV and Parquet files with SQL.
- [Cromagnon CSV Studio](https://cromagnon.app/studios/csv-studio) ✈️: profile columns, clean, deduplicate, split, merge, pivot and chart large CSV files.
- [Cromagnon CSV splitter](https://cromagnon.app/tools/csv-splitter), [CSV to JSON](https://cromagnon.app/tools/csv-to-json) and [JSON to CSV](https://cromagnon.app/tools/json-to-csv): quick single-job converters.

## File conversion

- [VERT](https://vert.sh) 🟢: converts images, audio and documents between hundreds of formats with WebAssembly, on your device. **Video is the exception:** the official site converts video on its server, unless you host VERT yourself. AGPL-3.0.

## Audio

- [AudioMass](https://audiomass.co) ✈️: a waveform audio editor for cut, trim, fade, EQ, compression, reverb and pitch, with MP3 export. It runs in the browser with no backend. The source is on GitHub, but without a standard licence.

## Encryption

- [hat.sh](https://hat.sh) 🟢: encrypts and decrypts files in the browser with libsodium (XChaCha20-Poly1305, Argon2id). Its README says no data is collected or sent. Safari and mobile browsers are limited to 1 GB files. MIT.

## Developer tools

- [CyberChef](https://gchq.github.io/CyberChef/) 🟢 ✈️: GCHQ's "Cyber Swiss Army Knife" for encoding, decoding, hashing, compression and data analysis. Its README says input is never sent to the server. The HTTP request and DNS-over-HTTPS operations contact hosts you choose, by design.
- [JSON Crack](https://jsoncrack.com/editor) 🟢: turns JSON, YAML, CSV and XML into an interactive graph you can explore. The project says all data processing is local. Apache-2.0.
- [IT-Tools](https://it-tools.tech) 🟢 ✈️: a large set of developer utilities, including UUIDs, JWT, converters and network calculators, built as a fully client-side app. GPL-3.0.
- [Cromagnon developer tools](https://cromagnon.app/tools?category=Developer): JSON formatter, regex tester, JWT decoder, SQL formatter, cron parser, hash generator and more.

## Diagrams and whiteboards

- [Excalidraw](https://excalidraw.com) 🟢 ✈️: a hand-drawn style whiteboard. Drawings autosave in the browser, and live collaboration is end-to-end encrypted.
- [tldraw](https://www.tldraw.com): an infinite canvas whiteboard. When you're signed out, drawings are stored on your own computer (browser storage). Signed-in files are saved to tldraw's cloud. The SDK is source-available under its own licence.
- [draw.io](https://app.diagrams.net) 🟢: flowcharts and diagrams, saved to your device or the storage you choose. Exporting to PDF (and to images in old browsers) sends the diagram to draw.io's server, where it's deleted after delivery. A "lockdown" setting turns that off.

## Study, citations and maths

- [Cromagnon Study Studio](https://cromagnon.app/studios/study-studio) ✈️: flashcards with the FSRS memory model, eight study modes and Anki and Quizlet import. Decks stay in your browser unless you sign in to sync.
- [Cromagnon Citation Studio](https://cromagnon.app/studios/citation-studio): references in 18 styles, including APA, MLA, Chicago, Harvard and IEEE. Looking up a DOI or ISBN contacts public catalogues; your reference list stays in your browser.
- [Cromagnon Math Studio](https://cromagnon.app/studios/math-studio) ✈️: equations, calculus, statistics and graphs, with every step shown.

## Business

- [Cromagnon Invoice Studio](https://cromagnon.app/studios/invoice-studio) ✈️: invoices, quotes and receipts in any currency, exported to PDF and kept in your browser.

## SEO and web

These work on text you paste. Checks of a live web page must fetch it, so they're not listed here.

- [Cromagnon SERP preview](https://cromagnon.app/tools/serp-preview): see how a title and description look in Google, measured in pixels.
- [Cromagnon schema markup generator](https://cromagnon.app/tools/schema-generator): JSON-LD structured data, with Google's required properties checked.
- [Cromagnon llms.txt generator](https://cromagnon.app/tools/llms-txt-generator): build and check an `llms.txt` file for AI assistants.

## How to check a tool yourself

You don't have to take anyone's word for it, including ours:

1. Open the tool, then open your browser's developer tools (F12) and go to the **Network** tab.
2. Load or drop a test file and run the tool.
3. Watch for a request that carries your file: a large `POST` or `PUT` upload, or a request the size of your file.
4. Better still, load the tool once, **turn off your internet**, and try again. If it still works, the work is happening on your device.

## Contributing

Suggestions are welcome. Please open an issue or a pull request with:

- the tool's name and link, and the section it belongs in;
- a link to where the tool says files stay in the browser (README, docs or privacy terms);
- any feature that does send data to a server.

Tools that upload files, require an account for the basic job, or add watermarks won't be added. See [CONTRIBUTING.md](CONTRIBUTING.md).

---

Maintained by the team behind [Cromagnon](https://cromagnon.app), a free suite of in-browser file tools, which is why several of its tools appear here. Other tools are listed on the same terms, and corrections from their makers are welcome.

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](LICENSE) To the extent possible under law, the contributors have waived all copyright to this list.
