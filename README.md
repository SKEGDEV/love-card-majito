# Romantic Envelope Card

A beautiful, interactive love card built with Astro. The project features a customizable envelope, falling petals, background glow effects, and a configurable digital letter with a photo attachment.

## Prerequisites

Make sure you have Node.js installed on your machine. You can use `npm`, `yarn`, or `pnpm` as your package manager.

## Installation

First, install the dependencies using your preferred package manager:

```bash
# Using pnpm (recommended)
pnpm install

# Using npm
npm install

# Using yarn
yarn install
```

## Running Locally for Debugging / Development

To start the development server and test the card locally:

```bash
# Using pnpm
pnpm run dev

# Using npm
npm run dev

# Using yarn
yarn dev
```

The application will be available at `http://localhost:4321`.

## Deployment (Building for Production)

To build the project for production, generating a static site in the `dist/` directory:

```bash
# Using pnpm
pnpm run build

# Using npm
npm run build

# Using yarn
yarn build
```

You can then serve the `dist/` folder using any static file server or deploy it to platforms like Vercel, Netlify, or GitHub Pages.

## Customizing the Card

You can easily adapt this card for whoever you want without needing to touch the main code.

### 1. Text Configuration

Edit the `public/config.json` file. This file controls the text displayed on the envelope and inside the letter:

```json
{
  "relationshipStart": "YYYY-MM-DD", 
  "envelopeTo": "To: [Name]",
  "envelopeFrom": "From: [Your Name]",
  "title": "Title of your letter",
  "paragraphs": [
    "Paragraph 1...",
    "Paragraph 2...",
    "Paragraph 3..."
  ],
  "signature": "Your signature"
}
```

*   **`relationshipStart`**: Used to calculate the time together counter automatically.
*   **`paragraphs`**: Each string in the array creates a new paragraph in the letter.

### 2. Custom Images

To change the photo or the pushpin:

1.  Navigate to the `src/assets/` directory.
2.  Replace `photo.jpg` with your own image (keep the same name, or update the import reference in `src/pages/index.astro`).
3.  Replace `pushpin.svg` if you want a different pin graphic.
