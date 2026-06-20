# Paste As Image

A zero-dependency Windows utility that lets you paste the image on your clipboard directly into a File Explorer directory as a new `.png` file via the right-click context menu.

## Installation
1. Double-click `PasteAsImage.reg` to merge it into your registry.
2. No admin privileges required (installs to `HKEY_CURRENT_USER`).

## Usage
1. Copy an image to your clipboard (e.g., using Snipping Tool or right-clicking an image online).
2. Right-click the background of any folder in File Explorer (or right-click a specific folder).
3. Select **Paste as new Image**.
4. The image is saved as `PastedImage_YYYYMMDD_HHMMSS.png`.

## Uninstallation
Delete the following keys from your registry:
- `HKEY_CURRENT_USER\Software\Classes\Directory\Background\shell\PasteAsImage`
- `HKEY_CURRENT_USER\Software\Classes\Directory\shell\PasteAsImage`

## Paste & Overwrite
1. Right-click an existing image file in Explorer.
2. Select **Paste & Overwrite**.
3. Accept the confirmation prompt.
4. The image will be replaced with the contents of your clipboard.
