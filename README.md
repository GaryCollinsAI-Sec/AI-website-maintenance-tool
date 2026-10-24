# Abel-AI-website-maintenance-tool

**A browser-based website troubleshooting assistant.**

Abel is a Chrome extension designed to inspect web pages, identify potential website issues, and provide clear explanations and suggested fixes. Its goal is to make website troubleshooting easier by helping developers understand what may be wrong and what they can do about it.

## Features

- **Rule-based website inspection** — Analyze the active web page for supported issues.
- **Page metadata checks** — Identify missing or incomplete metadata, including canonical URL and social-sharing metadata.
- **Accessibility checks** — Identify supported markup issues, such as missing image alternative text.
- **Link diagnostics** — Detect placeholder links that may need a valid destination.
- **Severity classifications** — Categorize findings by severity.
- **Finding classifications** — Distinguish detected conditions, potential issues, and recommendations.
- **Actionable explanations** — Present explanations and suggested fixes for identified findings.
- **Affected-element details** — Inspect relevant page elements and their selectors.
- **Developer-friendly interface** — Review findings in a compact Chrome extension interface.

## Technology Stack

- React
- TypeScript
- Vite
- Tailwind CSS
- Chrome Extensions Manifest V3

## Project Status

**Current version:** 0.1.0 (initial development)

Abel is under active development. The current version focuses on rule-based website inspection, understandable findings, and practical troubleshooting recommendations.

## Installation for Development

### Prerequisites

- Google Chrome or a compatible Chromium-based browser
- Node.js and npm
- Git

### 1. Clone the repository

Replace the placeholder URL with your GitHub repository URL.

```bash
git clone <your-repository-url>
cd abel
```

### 2. Install dependencies

```bash
npm install
```

### 3. Build the extension

```bash
npm run build
```

### 4. Load the extension in Chrome

1. Open `chrome://extensions`.
2. Enable **Developer mode**.
3. Select **Load unpacked**.
4. Choose the generated extension directory, typically `dist`, if that is where your build outputs the extension manifest.
5. Open a supported web page and launch Abel from Chrome's extensions menu.

The build output and manifest configuration must be present and valid for Chrome to load the extension successfully.

## How It Works

Abel uses predefined rules to inspect supported aspects of a web page and report findings. Each finding includes a classification, severity, explanation, and suggested action where applicable.

Abel is intended to assist developers with troubleshooting. Findings should be reviewed in context before applying changes to a website.

## Planned Improvements

Future development may include:

- Expanded website diagnostics
- Improved detection accuracy and reduced false positives
- More detailed troubleshooting guidance
- AI-assisted explanations and fix suggestions
- Optional local AI integration using Ollama and LangChain
- Human-reviewed fixes and verification that changes resolve the identified issue

AI-assisted capabilities are planned and are not represented as implemented features of the current version.

## Limitations

- Detection is limited to the rules implemented in the current version.
- Automated findings may require manual review.
- A recommendation does not necessarily indicate a website defect.
- Abel does not guarantee that every issue on a page will be detected.
- Suggested fixes should be reviewed before being applied.

## Contributing

Abel is an evolving project. Suggestions, bug reports, and contributions that improve diagnostic accuracy, usability, and the quality of troubleshooting recommendations are welcome.

## License

A license has not yet been specified. Licensing terms will be added when the project license is selected.
