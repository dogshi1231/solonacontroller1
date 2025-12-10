# GitHub Pages Setup Guide - Solana Neon Skin

## Quick Setup

Your GPV-compatible CSS file has been created in:
```
docs/solana.css
```

## GitHub Pages Configuration

### Step 1: Commit & Push to GitHub
```powershell
git add .
git commit -m "Add GitHub Pages setup with Solana Neon skin"
git push origin main
```

### Step 2: Enable GitHub Pages
1. Go to your GitHub repository
2. Click **Settings** → **Pages**
3. Under "Source", select:
   - **Branch**: `main`
   - **Folder**: `/docs`
4. Click **Save**

GitHub will display: `Your site is live at https://yourusername.github.io/solonacontroller1/`

## Use in GamepadViewer

### Once GitHub Pages is Live

Your CSS will be available at:
```
https://yourusername.github.io/solonacontroller1/solana.css
```

Use this URL in GamepadViewer:
```
https://gamepadviewer.com/?p=1&s=5&editcss=https://yourusername.github.io/solonacontroller1/solana.css
```

## What Changed

✅ **CSS Updated For:**
- All image URLs point to GamepadViewer's CDN (proper CORS headers)
- Full `.ds4` controller structure support
- Neon Solana color scheme (purple/teal/cyan)
- Press states and animations
- Half-controller mode

## Alternative: Instant Testing with Pastebin

If you want to test immediately:

1. Go to https://pastebin.com
2. Paste the contents of `docs/solana.css`
3. Click "Create New Paste"
4. Click **RAW** button to get the raw URL
5. Use in GamepadViewer:
```
https://gamepadviewer.com/?p=1&s=5&editcss=https://pastebin.com/raw/XXXXXXXXXX
```

## Troubleshooting

**Q: Skin not showing?**
- A: Make sure GitHub Pages is enabled in Settings → Pages
- Wait 1-2 minutes for GitHub Pages to deploy

**Q: Still CORS errors?**
- A: Pastebin RAW URLs have proper CORS headers and work 100% with GamepadViewer

**Q: Colors not right?**
- A: Check your browser console for CSS loading errors
- Clear browser cache (Ctrl+Shift+Del)

## Color Reference

- **A Button**: #00FFA3 (Cyan/Green)
- **B Button**: #7928CA (Purple)
- **X Button**: #0AEFFF (Sky Blue)
- **Y Button**: #9945FF (Violet)
- **Base**: Purple/Teal gradient with neon glow effects
