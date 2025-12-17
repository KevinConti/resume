# Kevin Conti's Resume

This repository contains my resume in JSON Resume format.

## Setup

Install dependencies:
```bash
npm install
```

## Exporting with Different Themes

The project uses `resumed` (a modern fork of resume-cli) for exporting resumes with different themes.

### One-time Global Setup

Install the required tools and themes globally:

```bash
# Install resumed CLI
npm install -g resumed

# Install puppeteer (required for PDF export)
npm install -g puppeteer

# Install available themes
npm install -g jsonresume-theme-even jsonresume-theme-elegant jsonresume-theme-kendall jsonresume-theme-paper
```

### Export to PDF

Export your resume with a specific theme:

```bash
resumed export resume.json --theme jsonresume-theme-even --format pdf --output kevinconti-even.pdf
resumed export resume.json --theme jsonresume-theme-elegant --format pdf --output kevinconti-elegant.pdf
resumed export resume.json --theme jsonresume-theme-kendall --format pdf --output kevinconti-kendall.pdf
resumed export resume.json --theme jsonresume-theme-paper --format pdf --output kevinconti-paper.pdf
```

## Development

Start a local server to preview your resume:

```bash
npm start
```

This will serve the resume using the customized Stack Overflow theme at http://localhost:4000

## Available Themes

- **even** - Clean, two-column layout with professional sidebar
- **elegant** - Minimalist single-column design
- **kendall** - Modern with clear section headers
- **paper** - Simple, traditional ATS-friendly format
- **stackoverflow** (custom) - Customized Stack Overflow theme (current default)
