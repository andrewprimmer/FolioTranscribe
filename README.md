# FolioTranscribe

**Handwritten Text Recognition for Historical Documents**

FolioTranscribe is a browser-based tool for transcribing historical handwritten documents using AI. It supports archival citation metadata and exports transcriptions as formatted Word documents, ready for academic use.

🌐 **Live site:** [foliotranscribe.com](https://foliotranscribe.com)

---

## Features

- **AI-powered HTR** — powered by Google Gemini, sensitive to historical orthography, abbreviations, and marginal annotations
- **Archival citation fields** — archive, collection, series, box, volume, folio, reference code, date, and document name, auto-assembled into a citation string
- **Text output** — editable transcript window with copy to clipboard
- **Word export** — generates a `.docx` with archival metadata in the page header, citation reference, and page-numbered footer
- **Privacy first** — your API key is stored only in your browser's local storage and never sent to our servers

---

## Setup

### 1. Get a Gemini API Key

Go to [aistudio.google.com](https://aistudio.google.com), sign in with a Google account, and click **Get API key → Create API key**. The free tier allows 1,500 requests per day.

### 2. Deploy to GitHub Pages

1. Fork or clone this repository
2. Go to **Settings → Pages**
3. Set source to **Deploy from a branch → main → / (root)**
4. Your site will be live at `yourusername.github.io/foliotranscribe`

### 3. Use the tool

1. Open the site in your browser
2. Enter your Gemini API key and click **Save Key**
3. Upload a document image (JPG, PNG, TIFF)
4. Optionally fill in archival reference fields
5. Click **Transcribe Document**
6. Copy the text or export to Word

---

## Repository Structure

```
foliotranscribe/
└── index.html        # Complete single-file application
└── README.md         # This file
```

---

## Roadmap

- [ ] Cloudflare Worker proxy for secure API key handling
- [ ] Batch processing of multiple folios
- [ ] Balance sheet extraction to Excel
- [ ] Panel dataset construction for quantitative research
- [ ] Android app with Word export

---

## Privacy & Data

Your Gemini API key is stored in your browser's `localStorage` and is never transmitted to FolioTranscribe servers. Document images are sent directly from your browser to Google's Gemini API for processing. Please review [Google's AI Studio privacy policy](https://policies.google.com/privacy) before processing sensitive archival material.

---

## Built With

- [Google Gemini API](https://ai.google.dev/) — vision and transcription
- [docx.js](https://docx.js.org/) — Word document generation
- [EB Garamond](https://fonts.google.com/specimen/EB+Garamond) / [Libre Baskerville](https://fonts.google.com/specimen/Libre+Baskerville) — typography

---

*FolioTranscribe is developed for academic historical research. If you use it in your work, a mention in your acknowledgements is appreciated.*
