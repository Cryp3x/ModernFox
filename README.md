# Modern Firefox Theme

- This is the first version so expect bugs.

<img width="2841" height="1749" alt="demo" src="https://github.com/user-attachments/assets/8fe54c8e-f6a5-4932-9043-bdbba016a100" />


## Requirements & Complementary Extensions
- For **website transparency** (making web pages semi-transparent to show your wallpaper), use the excellent extension:  
  [transparent-zen by frostybiscuit](https://github.com/frostybiscuit/transparent-zen)
- Additional about:config preferences (required for full transparency effects, especially browser window and tab content transparency on supported systems like Windows 11):
Go to about:config and set the following to true:
`browser.tabs.allow_transparent_browser`
`widget.transparent-windows`

For Mica effects (Windows 11 native blur/transparency in titlebar and UI):
`widget.windows.mica → true`
`widget.windows.mica.popups → 2`
`widget.windows.mica.toplevel-backdrop → 2`

## Installation Steps

1. **Enable userChrome/userContent customization in Firefox**
   - Open a new tab and go to `about:config`
   - Search for `toolkit.legacyUserProfileCustomizations.stylesheets`
   - Set it to `true` (double-click to toggle)

2. **Locate your Firefox profile folder**
   - Go to `about:support` in a new tab
   - Under "Profile Folder", click "Open Folder" (Windows) / "Show in Finder" (macOS) / open the path (Linux)

3. **Create the chrome folder (if it doesn't exist)**
   - Inside your profile folder, create a folder named `chrome` (lowercase)
   - Add userChrome.css and userContent.css files inside.

5. **Restart Firefox**
   - Completely close and reopen Firefox

6. **(Optional) Install transparent-zen for website transparency**
   - Visit: https://github.com/frostybiscuit/transparent-zen
   - Follow the installation instructions there.
   - This will make actual web pages transparent.
