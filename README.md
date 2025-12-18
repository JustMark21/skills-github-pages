# Catalog Companion (PS 370)

Catalog Companion is a single-page web application that replaces paper order forms with a simple, mobile-friendly catalog. Families can browse available items, select what they want, and submit an order via email or copy-to-clipboard.

## 🚀 Live Demo

[View the live Catalog Companion](https://justmark21.github.io/Catalog_Companion/)

## ✨ Features

- Visual catalog with images and descriptions (54+ items).
- Instant search by item name or ID.
- Tap/click items to add them to a selection tray (shopping-cart style).
- Order form collects:
  - Student & parent name
  - Household size
  - Allergies / dietary notes
- Smart submission options:
  - Opens the user's default email client with a pre-written order.
  - Quick links for Gmail and Outlook webmail.
  - Copy order text to clipboard as a fallback.
- Responsive — works on phones, tablets, and desktops.

## 📂 Project Structure

The app is self-contained and runs entirely in the browser (no backend required).

```text
/ (root)
├── index.html        # The main application (HTML + JS + CSS)
├── images/           # Product images, e.g., 1.jpg, 2.jpg, ..., 54.jpg
└── README.md         # This file
```

## 🛠️ Setup & Deployment

1. Add the files to your repository:
   - Upload `index.html` to the repository root.
   - Create an `images/` folder and upload your product images.

2. Image naming:
   - Rename each image to match the item ID used by the app: `1.jpg`, `2.jpg`, ..., `54.jpg`.

3. Enable GitHub Pages (to publish the site):
   - Go to your repository **Settings** → **Pages**.
   - Under **Source**, choose the `main` branch and `/ (root)` folder.
   - Save. After a minute or two you’ll get a live URL like `https://yourusername.github.io/repo-name/`.

## ⚙️ Customization

- Editing the catalog:
  - Open `index.html` and find the `catalogItems` array (search for `const catalogItems`).
  - Add or remove items there. Example entry:
    ```javascript
    { id: 55, name: "New Item Name", category: "Snacks", description: "Short description" }
    ```
  - Add a matching image `images/55.jpg` if the item has an image.

- Changing the recipient email:
  - Search `index.html` for the existing recipient email (e.g., `CatalogCompanionPS370@outlook.com`) and replace it with the desired address in both the visible tip text and the JavaScript handling the submission.

## 📝 Usage Guide

1. Select items by tapping/clicking them.
2. The selection tray shows the count and selected items.
3. Click "Review & Submit" to open the order form.
4. Fill in student/parent details, household size, and allergy info.
5. Choose a send method:
   - Default email client (desktop or mobile)
   - Gmail (web)
   - Outlook (web)
   - Or copy the order text to the clipboard and paste it into any app

## 📄 License

This project is licensed under the MIT License. See the LICENSE file for details (or add one if you need an explicit license file).
