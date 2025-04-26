# PieApp OTA Install Package

This folder contains everything needed for an over-the-air installation of PieApp on iPhone via GitHub Pages.

## Files

- `PieApp.ipa`  
  Placeholder for your signed iPhone app (`.ipa`). Replace this with your actual signed PieApp IPA.

- `manifest.plist`  
  OTA manifest listing the `.ipa` URL and app metadata.  
  **Replace** `https://YOUR_GITHUB_URL/pieapp_ota_package/PieApp.ipa` with the raw URL to your PieApp IPA.

- `index.html`  
  Simple installer page.  
  **Replace** `https://YOUR_GITHUB_URL/pieapp_ota_package/manifest.plist` with the raw URL to your manifest.

## Usage

1. Commit all files to GitHub under a folder named `pieapp_ota_package`.
2. Enable GitHub Pages (point to the `main` branch → `/` or `docs/` folder).
3. Access `index.html` from Safari on your iPhone:
   ```
   https://<username>.github.io/<repo>/pieapp_ota_package/index.html
   ```
4. Tap **Install PieApp** to begin OTA installation.

**Note:** Ensure PieApp IPA is signed with a provisioning profile that includes the target iPhone devices.
