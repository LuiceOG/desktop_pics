 <h1 align="center">Desktop Pics</h1>

<p align="center">
  <strong>Post pictures in YouTube comments and replies from a desktop browser.</strong>
</p>

<p align="center">
  <a href="https://github.com/LuiceOG/desktop_pics/releases/latest">
    <img src="https://img.shields.io/github/manifest-json/v/LuiceOG/desktop_pics?filename=extension%2Fmanifest.json&label=version&color=ff0033" alt="Version">
  </a>
  <img src="https://img.shields.io/badge/Chrome-121%2B-4285F4?logo=googlechrome&logoColor=white" alt="Chrome 121 or newer">
  <img src="https://img.shields.io/badge/Manifest-V3-34A853" alt="Manifest V3">
</p>

<p align="center">
  <a href="#install">Install</a> ·
  <a href="#use">Use</a> ·
  <a href="#troubleshooting">Troubleshooting</a> ·
  <a href="#limits">Limits</a> ·
  <a href="#how-it-works">How it works</a> ·
  <a href="#privacy">Privacy</a>
</p>

## About

**Desktop Pics** is a browser extension project intended to add picture selection to YouTube comments and replies on desktop.

YouTube's desktop comment interface does not natively offer the same picture-attachment experience as its mobile app. Desktop Pics aims to add a **Pics** button next to the emoji button.

- **Picture picker.** Select a picture from the extension's picker.
- **Write around it.** Write a comment alongside your selected picture.
- **Favorites.** Keep frequently used pictures easy to find.
- **Simple setup.** Load the extension in Chrome or a compatible Chromium browser.

> **Important:** Replacing GIF-related text does not automatically make ordinary pictures work. Picture uploading and comment handling must be implemented separately.

## Install

Desktop Pics is loaded from a ZIP file.

<p align="center">
  <a href="https://github.com/LuiceOG/desktop_pics/releases/latest/download/desktop-pics-chrome.zip">
    <img src="https://img.shields.io/badge/Download-Chrome%20%C2%B7%20Edge%20%C2%B7%20Brave-4285F4?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Download for Chrome, Edge and Brave">
  </a>
</p>

### Chrome, Edge, Brave

1. Download [`desktop-pics-chrome.zip`](https://github.com/LuiceOG/desktop_pics/releases/latest/download/desktop-pics-chrome.zip).
2. Extract the ZIP file.
3. Open `chrome://extensions`.
4. Enable **Developer mode**.
5. Click **Load unpacked**.
6. Select the extracted folder containing `manifest.json`.

If YouTube is already open, refresh the tab if the Pics button does not appear.

## Updating

1. Download the latest `desktop-pics-chrome.zip`.
2. Extract the updated files into your extension folder.
3. Open `chrome://extensions`.
4. Click **Reload** on the Desktop Pics extension.

## Use

1. Open a YouTube video or Short.
2. Click **Add a comment…** or **Reply**.
3. Click the **Pics** button next to the emoji button.
4. Select a picture.
5. Write your comment.
6. Click YouTube's **Comment** button.

Picture publishing depends on the extension having a working upload and comment integration mechanism.

## Troubleshooting

| Problem | What to try |
|---|---|
| No Pics button appears | Refresh the YouTube tab. |
| Extension cannot be loaded | Select the folder containing `manifest.json`. |
| Picture picker does not open | Reload the extension and refresh YouTube. |
| Picture does not appear in the posted comment | Check the picture-upload and comment integration implementation. |
| Download link does not work | Check the repository's Releases page. |

## Limits

- **Unofficial.** This project is not affiliated with YouTube or Google.
- **Browser support.** Intended for Chrome and compatible Chromium browsers.
- **Picture support requires implementation.** Changing labels alone does not add image uploading.
- **YouTube compatibility.** YouTube may change its website or reject unsupported comment requests.

## How it works

The extension adds a picture-selection interface to the YouTube comment area. A complete implementation needs a way to upload or host selected pictures and a compatible method of displaying them in comments.

## Project structure

| File | Purpose |
|---|---|
| `extension/manifest.json` | Extension configuration and permissions |
| `extension/src/content.js` | Comment interface and picture picker |
| `extension/src/content.css` | Interface styling |
| `extension/src/main.js` | Page-side integration, if required |
| `extension/src/sw.js` | Background tasks, if required |

## Privacy

- Request only the permissions needed for the extension's functionality.
- Document any external image-hosting services.
- Explain how pictures are stored and transmitted.
- Do not claim pictures are private or stored locally unless the code guarantees it.

## License

Add a license section if you choose a license for your project. If you modify code from another project, preserve and comply with the original project's license requirements.
