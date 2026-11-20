# AI Eco Sorter

A responsive showcase website for an educational waste-segregation project built with Google Teachable Machine.

## Live model

The website includes an embedded area pointing to the project's hosted Teachable Machine model:

https://teachablemachine.withgoogle.com/models/poAO8ZJ1q/

**Important:** A Teachable Machine model URL hosts model assets; it is not guaranteed to be a standalone interactive demo page. If Google does not render an interactive experience inside the iframe, use the **Open AI Eco Sorter model** link below the frame. Camera access in embedded pages also depends on browser permissions and Google's embedding policy.

## Categories
- Organic / Biodegradable
- Recyclable
- Non-recyclable

## Run locally
This is a static website. No Node.js, backend, database, or build step is required.

1. Download or clone this repository.
2. Open the folder.
3. Double-click `index.html` or use VS Code Live Server.
4. For camera testing, use a secure context such as localhost or HTTPS.

## Deploy with GitHub Pages
1. Open the repository **Settings → Pages**.
2. Under **Build and deployment**, select **Deploy from a branch**.
3. Choose branch **main** and folder **/ (root)**, then Save.
4. Wait for GitHub Pages to publish the site.

The expected address is:
https://farixhere.github.io/AI-ECO-SORTER/

## Project limitations
- This is an educational image-classification prototype, not an automated waste-sorting machine.
- Predictions can be wrong, especially with unfamiliar objects, poor lighting, or images unlike the training examples.
- Follow local municipal guidance for actual waste disposal.
