# Firefox Glassmorphic New Tab Page Customization

This `userContent.css` creates a fully transparent, glassmorphic new tab page in Firefox:
- Only your pinned top sites are shown (large glossy tiles)
- Search bar is completely removed
- Everything is perfectly centered
- Pure wallpaper visibility with subtle glass effects that match a glossy floating tab/theme setup
- Ideal for vibrant/dark wallpapers (like cyberpunk styles)

## Features
- No search bar — pure minimal top sites grid
- Tiles have matching glass blur, borders, and shadows
- Full title wrapping (no truncated text)
- Responsive grid that works with any number of pinned sites
- Hover lift effects for premium feel

## Requirements & Complementary Extensions
- This works best with a custom `userChrome.css` that makes Firefox toolbars/tabs transparent and glossy (floating pill tabs).
- For **website transparency** (making web pages semi-transparent to show your wallpaper), use the excellent extension:  
  [transparent-zen by frostybiscuit](https://github.com/frostybiscuit/transparent-zen)  
  It perfectly complements this new tab style by applying transparency to actual websites.

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

4. **Add the userContent.css file**
   - Inside the `chrome` folder, create a new file named `userContent.css`
   - Copy and paste the full CSS code from above into this file
   - Save the file

5. **Restart Firefox**
   - Completely close and reopen Firefox

6. **(Optional) Install transparent-zen for website transparency**
   - Visit: https://github.com/frostybiscuit/transparent-zen
   - Follow the installation instructions there (usually via Firefox Add-ons or manual user.js tweak)
   - This will make actual web pages transparent, completing the full "glass OS" look with your wallpaper shining through everywhere.

## Customization Tips
- To move the tiles higher/lower: change `padding: 80px 40px 60px` in the `body` rule (first number is top padding)
- To make tiles larger/smaller: adjust `width`/`height` in `.top-site-outer .tile` and the icon sizes
- To change glass strength: tweak the `rgba` opacity values or `blur()` amounts

Enjoy your clean, minimalist, cyberpunk-inspired Firefox new tab!
