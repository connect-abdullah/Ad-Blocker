# Chrome Ad Blocker Extension

## Overview
This is a simple Chrome ad blocker extension that helps block ads from various websites. The extension works by using two JSON files:
1. **`manifest.json`**: Configures the Chrome extension and sets up permissions.
2. **`rules.json`**: Contains the rules specifying which websites and resources to block.

I created the rules by identifying websites that frequently show ads, with guidance from ChatGPT. The blocked websites include those serving push ads, popup ads, banner ads, and more.

## Features
- Blocks ads from popular ad-serving websites.
- Prevents intrusive ads like popups, banners, and interstitials.
- Simple and lightweight design.

## Installation Instructions
Follow the steps below to use the ad blocker extension in Chrome:

### ### Step 1: Download the Files
1. Download the extension files, which include `manifest.json` and `rules.json`.
2. Save them in a folder on your computer, for example: `~/Documents/Ad-Blocker`.

### Step 2: Remove the `metadata` Folder
If you notice a `metadata` folder in the extension folder, please delete it. This folder is automatically generated when the extension is loaded into Chrome, and having it there initially can prevent the extension from being loaded properly.

### Step 3: Enable Developer Mode in Chrome
1. Open Chrome and navigate to `chrome://extensions`.
2. In the top-right corner, toggle **Developer mode** to `ON`.

### Step 4: Load the Extension
1. Click the **Load unpacked** button.
2. Select the folder where you saved the extension files (`~/Documents/Ad-Blocker`).

### Step 5: Use the Extension
Once loaded, the ad blocker will automatically start blocking ads based on the rules defined in `rules.json`.

## How It Works
- **`manifest.json`**: Defines the extension's metadata and permissions required for blocking network requests.
- **`rules.json`**: Contains a list of ad-serving domains and resource types to block.

The extension uses the Chrome `declarativeNetRequest` API to block ad-related network requests before they load.

## Example Blocked Websites
Here are some examples of the ad-serving websites included in `rules.json`:
- `doubleclick.net`
- `googleadservices.com`
- `popads.net`
- `taboola.com`
- `outbrain.com`

## Disclaimer
This extension is for personal use and learning purposes. Use it responsibly and respect websites that rely on ads for revenue.


------------------------------------------

#### Let’s code, learn, and grow together! 🚀  

------------------------------------------
