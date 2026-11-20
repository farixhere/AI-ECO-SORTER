# AI Eco Sorter 🌱

**AI Eco Sorter** is an educational web project that explores how artificial intelligence can support better waste segregation. It combines a sustainability-focused website with an image-classification model trained using **Google Teachable Machine**.

> The goal is to make waste categories easier to understand and demonstrate how a machine-learning model can classify an image. This is a learning prototype, not a certified waste-management system.

## ♻️ Why this project is useful

Waste is easier to manage when it is separated correctly. People may not always know whether an item belongs with organic waste, recyclable materials, or non-recyclable waste.

AI Eco Sorter demonstrates how an image classifier could help by:

- **Supporting awareness:** gives people an interactive way to learn about common waste categories.
- **Encouraging segregation:** helps explain why separating waste at the source matters.
- **Making AI approachable:** shows a practical, everyday example of image classification.
- **Supporting education:** can be used for classroom demonstrations, science exhibitions, and introductory AI activities.
- **Starting conversations:** encourages users to think about recycling, composting, and responsible disposal.

### Intended categories

The model is intended to recognise these three broad classes:

| Category | Examples (illustrative) | General idea |
|---|---|---|
| Organic / Biodegradable | Fruit and vegetable scraps, leaves | Materials that can usually decompose or be composted |
| Recyclable | Clean paper, cardboard, some plastic or metal containers | Materials that may be processed and made into new products |
| Non-recyclable | Certain contaminated or mixed-material items | Items that generally cannot go into common recycling streams |

**Important:** These examples are general guidance only. Actual disposal rules differ by location, material composition, and local waste collection facilities. Always follow your local municipality's instructions.

## 🧠 How the AI works

AI Eco Sorter uses an image-classification model created with Google Teachable Machine.

1. **Collect examples:** images are gathered and organised into the waste categories the model should learn.
2. **Train:** Teachable Machine uses those examples to train an image classifier.
3. **Test:** new images are shown to the model to see how well it recognises examples it has not seen before.
4. **Export:** the trained model can be hosted by Teachable Machine or downloaded for use in another application.
5. **Predict:** when an image is supplied, the model returns a score for each learned class. The highest-scoring class is typically shown as the prediction.

The scores are model confidence values, not guarantees that the prediction is correct. Results depend on the quality, quantity, balance, and variety of the training images.

## 🛠️ How we built it

The project has two main parts:

### 1. The website

The showcase website is built with:

- **HTML** for the page structure and content.
- **CSS** for the layout, responsive design, colours, typography, and visual styling.
- **Google Fonts** for the typography.

It is a lightweight static website. It does not require a database, server, or backend to display the project information.

### 2. The machine-learning model

- **Google Teachable Machine** was used to create and train the image-classification model.
- The model was exported as a hosted Teachable Machine model.
- The hosted model URL used for this project is:

  https://teachablemachine.withgoogle.com/models/poAO8ZJ1q/

A hosted Teachable Machine model provides model files such as `model.json` and `metadata.json`. A website can load those files with the Teachable Machine image library and TensorFlow.js to run predictions. See the official [Teachable Machine image library documentation](https://github.com/googlecreativelab/teachablemachine-community/tree/master/libraries/image).

### Note about the live demo / embedding

Google's Teachable Machine website may block being displayed inside another website using an iframe. This is a browser/security restriction set by the remote website; adding camera permissions to the iframe cannot override it.

The model URL above is a hosted model endpoint, not necessarily a standalone interactive Teachable Machine page. For a reliable integrated demo, the website should load the hosted model files directly with the Teachable Machine JavaScript library and provide its own camera and image-upload controls. The current showcase page and hosted model are separate parts of the project.

## 🚀 Run the website locally

This repository contains a static website, so you do not need to install Node.js or run a backend.

1. Open the repository: [farixhere/AI-ECO-SORTER](https://github.com/farixhere/AI-ECO-SORTER).
2. Select **Code → Download ZIP**, then extract the ZIP file.
3. Open the extracted project folder.
4. Open `index.html` in a browser to view the showcase website.

For camera-based browser features, use a secure context such as **localhost** or an **HTTPS** website. Opening a local HTML file directly may not grant camera access.

## 🌐 Publish with GitHub Pages

1. Open this repository on GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select the `main` branch and the `/ (root)` folder.
5. Click **Save** and wait for GitHub Pages to publish.

When enabled, the site should be available at:

**https://farixhere.github.io/AI-ECO-SORTER/**

## 🎤 Exhibition demonstration

A simple way to present the project:

1. Open the published AI Eco Sorter website.
2. Introduce the waste-segregation problem and the three categories.
3. Explain that the image model was trained with examples using Google Teachable Machine.
4. Open the live model/demo when available and test it with a few sample items or images.
5. Explain that the model predicts from visual patterns learned during training and can make mistakes.
6. Finish by discussing how better waste separation can support recycling and composting.

**Exhibition tip:** Prepare a few test images in advance, use good lighting, and test the demo on the actual exhibition computer and browser before presenting. Do not rely on an internet connection or camera permission working without testing first.

## ⚠️ Limitations and responsible use

- This is an educational prototype, not an industrial sorting system.
- The model can misclassify unfamiliar objects, mixed materials, dirty items, unusual angles, or images with poor lighting.
- A high confidence score does not prove that a prediction is correct.
- The three categories are simplified; real waste rules can be more detailed and vary by location.
- Do not use the prediction as the only basis for handling hazardous, medical, electronic, or chemical waste.

## 🔭 Possible future improvements

- Integrate the hosted model directly into the website with camera and image-upload controls.
- Add clearer disposal suggestions based on local waste rules.
- Expand and balance the training dataset with more object types, backgrounds, and lighting conditions.
- Test the model using new images that were not included in training.
- Add multilingual explanations for exhibition visitors.

## 📚 References

- [Google Teachable Machine](https://teachablemachine.withgoogle.com/)
- [Teachable Machine Image Library — official documentation](https://github.com/googlecreativelab/teachablemachine-community/tree/master/libraries/image)
- [TensorFlow.js](https://www.tensorflow.org/js)

---

**AI Eco Sorter** — Small choices. Smarter planet. 🌍
