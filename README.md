# Study Hub

A responsive, static educational website built with plain HTML, CSS and JavaScript. It is designed to run on GitHub Pages without a backend, database, or external image hosting.

## Project structure

```text
study-hub/
├── index.html
├── css/
│   └── style.css
├── js/
│   └── app.js
└── images/
    └── (add your 28 JPG lesson images here)
```

## Add your lesson images

Copy your own educational JPG images into `images/` using these exact names:

- Arabic: `arabic-01.jpg` through `arabic-07.jpg`
- English: `english-01.jpg` through `english-07.jpg`
- Mathematics: `mathematics-01.jpg` through `mathematics-07.jpg`
- Computer Science: `computer-01.jpg` through `computer-07.jpg`

Images 01–03 are free. Images 04–07 are hidden behind the premium lock until the code is accepted. If an image file is missing, the page displays a helpful filename reminder rather than a broken-image icon.

## Redeem code

The shared code is configured in `js/app.js`:

```js
const REDEEM_CODE = "1057999az";
```

After a successful entry, the unlocked state is saved in the browser's `localStorage` on that device/browser.

**Important security note:** this is a front-end-only demonstration of a redeem code. Anyone who can inspect the JavaScript files can discover the code or modify local storage. It cannot provide secure paid access without a backend.

## Run locally

Open `index.html` in a browser. For the most reliable local preview, use a simple static server, or publish the folder using GitHub Pages.

## Publish on GitHub Pages

1. Create or open your GitHub repository.
2. Upload `index.html`, the `css` folder, the `js` folder, and the `images` folder.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select your main branch and the `/ (root)` folder, then save.
6. Wait for GitHub Pages to publish the site and open the URL shown on the Pages settings screen.

All site asset paths are relative, so the project also works when published from a GitHub project repository.

## Creator chat

The Ask the Creator panel runs entirely in the browser. The exact phrase `من صانع الموقع` triggers the configured reply. Other messages receive a short local fallback response.
