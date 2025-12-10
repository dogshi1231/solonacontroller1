# ⚡ Solana Neon PS4 Controller Skin

A vibrant neon-themed PS4 DualShock 4 controller skin for GamepadViewer, inspired by the Solana blockchain's signature purple and teal color scheme.

![Solana Neon Skin Preview](assets/solana-logo.png)

## 🌟 Features

- **Neon Gradient Effects**: Vibrant purple (#7928CA, #9945FF) and teal (#00FFA3, #0AEFFF) gradients throughout
- **Glowing Components**: All buttons, sticks, D-pad, and triggers feature subtle neon glow effects
- **Smooth Animations**: Responsive press states with scale and glow transitions
- **Touchpad Display**: Centered "SOLANA" text with gradient coloring
- **Drop Shadow Glow**: Controller-wide neon aura for immersion
- **Color-Coded Buttons**:
  - **A Button**: Cyan (#00FFA3)
  - **B Button**: Purple (#7928CA)
  - **X Button**: Sky Blue (#0AEFFF)
  - **Y Button**: Violet (#9945FF)

## 📁 Repository Structure

```
solonacontroller1/
├── css/
│   └── solana-edit.css        # Main CSS styling override
├── assets/
│   └── solana-logo.png        # Solana-themed logo/branding
├── demo/
│   └── index.html             # Demo page and interactive preview
├── README.md                  # This file
└── [SVG asset files]          # Controller SVG base files
    ├── base.svgz
    ├── bumper.svgz
    ├── dpad.svgz
    ├── disconnected.svgz
    ├── face.svgz
    ├── start.svgz
    ├── sticks.svgz
    ├── touchpad.svgz
    └── triggers.svgz
```

## 🚀 Quick Start

### Installation

1. **Clone or download this repository**:
   ```bash
   git clone https://github.com/dogshi1231/solonacontroller1.git
   cd solonacontroller1
   ```

2. **Use with GamepadViewer**:
   - Navigate to [GamepadViewer](https://gamepadviewer.com/)
   - Load the controller skin by selecting the custom CSS file: `css/solana-edit.css`
   - Connect your PS4 controller and enjoy!

### Local Testing

Open `demo/index.html` in your browser to preview the controller skin with all styling applied.

## 🎨 Customization

To customize colors, edit `css/solana-edit.css` and modify these key color values:

- **Primary Purple**: `#7928CA` (or change to `#9945FF` for brighter variant)
- **Accent Teal**: `#00FFA3`
- **Secondary Cyan**: `#0AEFFF`

### Common Customizations

**Change Button Colors**:
```css
.ds4 .a {
  background: radial-gradient(circle at 30% 30%, #YOUR_COLOR, #DARKER_SHADE) !important;
}
```

**Adjust Glow Intensity**:
```css
.controller.ds4 {
  filter: drop-shadow(0 0 20px rgba(153, 69, 255, 0.6)) 
          drop-shadow(0 0 40px rgba(0, 255, 163, 0.3));
  /* Increase blur radius (20px) for more glow */
}
```

**Modify Glow Colors**:
Update the `rgba()` values in any `box-shadow` or `drop-shadow` declarations.

## 🔧 Technical Details

### CSS Architecture

- **No HTML modifications**: Pure CSS override using GamepadViewer's existing DOM structure
- **Pseudo-elements**: Uses `::before` for glow effects without altering the DOM
- **CSS Gradients**: Linear and radial gradients for depth and realism
- **Box Shadows**: Multiple layered shadows for complex glow effects
- **Transitions**: Smooth 0.1-0.2s transitions for press states

### Supported Controllers

This skin is optimized for:
- **PS4 DualShock 4 (DS4)** controllers
- Compatible with GamepadViewer's DS4 layout

### Browser Compatibility

- Chrome/Chromium 90+
- Firefox 88+
- Safari 14+
- Edge 90+

## 📊 Color Palette Reference

| Component | Primary | Secondary | Glow |
|-----------|---------|-----------|------|
| A Button | #00FFA3 | #009973 | rgba(0, 255, 163, 0.9) |
| B Button | #7928CA | #5a1fa0 | rgba(121, 40, 202, 0.9) |
| X Button | #0AEFFF | #0099cc | rgba(10, 239, 255, 0.9) |
| Y Button | #9945FF | #6b20d6 | rgba(153, 69, 255, 0.9) |
| Sticks | #1a1a2e | #0f0f1e | rgba(0, 255, 163, 0.4) |
| D-Pad | Linear Gradient | Purple→Teal | rgba(153, 69, 255, 0.6) |
| Touchpad | Linear Gradient | Purple→Teal | rgba(153, 69, 255, 0.8) |

## 🎯 Known Limitations

- Controller base SVG files must remain unchanged (these are provided by GamepadViewer)
- Glow effects are CSS-based and may vary by browser and GPU
- Some mobile browsers may have reduced performance with multiple drop-shadow filters

## 📝 Contributing

Want to improve this skin? Feel free to:
- Report issues or suggestions
- Submit pull requests with enhancements
- Share variations of the color scheme

## 📜 License

This project is provided as-is for community use. Solana is a registered trademark of Solana Foundation.

## 🔗 Resources

- [GamepadViewer](https://gamepadviewer.com/) - The controller overlay platform
- [Solana Ecosystem](https://solana.com/) - Learn more about Solana
- [PS4 DualShock 4 Controller](https://www.playstation.com/en-us/accessories/dualshock-4-wireless-controller/) - Official controller info

## ⚡ Credits

Created for the Solana gaming community. Inspired by the vibrant energy and innovation of the Solana blockchain.

---

**Enjoy your neon-lit gaming experience!** 🎮✨
