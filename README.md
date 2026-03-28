# Living Histories – Runware API Demo

A lightweight demo showing how to generate historically grounded scenes and maintain character consistency across multiple images using Runware.ai’s image generation API.

---

## What This Demonstrates

This demo explores a simple but powerful use case:

> Can we generate historically accurate scenes *and* place the same person consistently into those scenes?

It includes:

- Prompt-based scene generation  
- Reference-based character consistency (face/identity preservation)  
- Multi-image outputs with seed control  
- A visible API request/response panel for learning and debugging  

---

## 🛠️ How It Works

The app uses Runware’s `imageInference` task to generate images.

Two main workflows:

### 1. Prompt Mode
Generate historically grounded scenes using structured prompts:
- environment (moor, settlement, monastery)
- lighting and atmosphere

### 2. Reference Mode
Upload an image (e.g. a visitor portrait) and:
- pass it via `imageUpload`
- reuse returned UUIDs in `referenceImages`
- generate consistent character outputs across scenes

---

## ⚙️ Run Locally

This is a single-file demo.

1. Clone the repo
2. Open `index.html`
3. Add your Runware API key:

```js
const RUNWARE_API_KEY = "YOUR_RUNWARE_API_KEY_HERE";
