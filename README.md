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
- `HKEY_CURRENT_USER\Software\Classes\SystemFileAssociations\image\shell\PasteAndOverwrite`

## Paste & Overwrite
1. Right-click an existing image file in Explorer.
2. Select **Paste & Overwrite**.
3. A confirmation prompt will appear directly next to your mouse cursor (supports multi-monitor).
4. The image will be replaced with the contents of your clipboard. It will automatically save in the correct format (`.jpg`, `.gif`, `.bmp`, or `.png`) based on the target file's extension.
5. If your clipboard contains text instead of an image, you will get an error popup instead.
