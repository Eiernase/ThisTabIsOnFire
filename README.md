# Psychological Tab Manager
This is the firefox port of the chromium extension found on [this repository](https://github.com/Eiernase/NeverGonnaCloseATab/).

# Installation
## Firefox Add-on Store
Simply install it from [the listing](https://addons.mozilla.org/en-US/firefox/addon/psychological-tab-manager/) in the Firefox Add-on Store.

## Manually
You can install the extension unpacked, but it will be removed after a restart. If you're using the Dev or Nightly build, you can go to about:config and set xpinstall.signatures.required to false and drop the .zip file into about:addons and it will stay installed.

1. Download source code
2. Unpack
3. Go to about:debugging#/runtime/this-firefox
4. Click on "Load Temporary Add-on"
5. Select any file from the extension

# Known Issues & Workarounds
## Selecting custom sounds
You might notice that it is not possible to select a custom sound, since the popup window closes when opening the file picker. 
You can get around this by following these steps: 

1. Go to about:debugging#/runtime/this-firefox
2. Find 'Psychological Tab Manager' and click on "Inspect"
3. Click on the three dots '...' in the top right corner
4. Enable "Disable Popup Auto-Hide"

This property resets when you close the developer console.
