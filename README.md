# 🎡 Spin Wheel - Interactive Decision Maker

A modern, sleek, and fully-featured spin wheel application built with pure HTML, CSS, and JavaScript. Perfect for making decisions, running giveaways, or just having fun!

---

## ✨ Features

### 🎨 Design & UI
- **Modern Black Theme** - Sleek dark interface with white accents
- **Poppins Font** - Clean, modern typography throughout
- **Smooth Animations** - 60fps CSS animations with zero lag
- **Glassmorphism Effects** - Subtle transparency and blur effects
- **Responsive Layout** - Works perfectly on desktop, tablet, and mobile
- **Staggered Load Animations** - Beautiful entrance effects when page loads

### 🎯 Wheel Features
- **Customizable Segments** - Add unlimited choices (no limit)
- **Vibrant Colors** - 18 beautiful preset colors that cycle through segments
- **Enhanced Visuals**:
  - Subtle white border ring
  - Thicker segment dividers (4px)
  - Strong text shadows for readability
  - Inner ring detail on center circle
  - Glowing effect while spinning
- **Smooth Rotation** - Ease-out cubic animation for realistic spin
- **Random Results** - Fair and unpredictable outcomes

### 🎵 Audio Effects
- **Tick Sounds** - Satisfying click sound as wheel passes each segment
- **Win Sound** - Celebratory chord arpeggio when result is revealed
- **Web Audio API** - Synthesized sounds (no external files needed)

### 🎉 Confetti Celebration
- **150 Confetti Pieces** - Colorful celebration on every spin
- **Varied Shapes** - Mix of circles and squares
- **Random Colors** - Uses the same vibrant palette as the wheel
- **Smooth Animation** - 3-second fall with rotation and fade
- **Performance Optimized** - Staggered creation prevents lag

### 💾 Data Persistence
- **LocalStorage Integration** - Automatically saves your choices
- **Auto-Load** - Choices restore when you revisit the page
- **No Server Required** - Everything runs client-side

### 📱 Mobile Optimization
- **Touch-Friendly** - All buttons and interactions optimized for touch
- **No Tap Highlight** - Removed blue flash on mobile taps
- **Proper Hover Detection** - Hover effects only on devices with mouse
- **Active State Feedback** - Instant visual feedback on tap
- **Scroll Prevention** - No horizontal scrolling
- **Auto Scroll to Top** - Page always starts at the top on load/refresh
- **Touch Action Manipulation** - Prevents double-tap zoom

### 🎭 Interactive Elements

#### Spin Button
- Uppercase "SPIN" text with letter spacing
- Scale and lift animation on hover (desktop only)
- Press-down effect on click
- Disabled state while spinning
- Slide-up entrance animation

#### Manage Choices Section
- Add new choices via input field
- Remove individual choices with delete buttons
- Minimum 2 choices required
- Each choice slides in when added
- Hover effects on choice items (desktop)
- Compact, clean list design

#### Input Field
- Focus state with border highlight and glow
- Placeholder text brightens on hover
- Enter key support for quick adding
- Scale effect on focus (desktop only)

---

## 🎬 Animations

### Page Load Sequence
1. **Title** - Fades in from top (0.6s)
2. **Container** - Fades in with scale (0.8s)
3. **Left Section** - Slides in from left (0.6s, 0.1s delay)
4. **Wheel** - Zooms in with fade (0.7s, 0.2s delay)
5. **Input Group** - Slides up (0.5s, 0.2s delay)
6. **Right Section** - Slides in from right (0.6s, 0.3s delay)
7. **Pointer** - Drops from top (0.5s, 0.4s delay)
8. **Choices List** - Fades in (0.5s, 0.4s delay)
9. **Button** - Slides up (0.5s, 0.5s delay)

### Continuous Animations
- **Pointer Pulse** - Subtle shadow pulse (2s infinite)
- **Wheel Glow** - Pulsing glow while spinning (0.5s infinite)

### Interaction Animations
- **Button Hover** - Scale up + lift + shadow (desktop)
- **Button Active** - Scale down press effect
- **Choice Item Slide** - Slides in from left when added
- **Choice Hover** - Slide right + background tint (desktop)
- **Result Pop** - Bouncy scale-in effect
- **Confetti Fall** - 3s rotation and fall with fade

---

## 🛠️ Technical Details

### Technologies Used
- **HTML5** - Semantic markup
- **CSS3** - Modern styling with animations
- **JavaScript (ES6+)** - Vanilla JS, no frameworks
- **Canvas API** - For drawing the wheel
- **Web Audio API** - For sound effects
- **LocalStorage API** - For data persistence

### Browser Compatibility
- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

### Performance Optimizations
- **CSS Animations Only** - Hardware accelerated
- **RequestAnimationFrame** - Smooth wheel rotation
- **Staggered Confetti** - 15ms delay between pieces
- **Font Smoothing** - Antialiased text rendering
- **Touch Action** - Prevents unnecessary gestures
- **Scroll Restoration** - Manual control for consistent behavior

---

## 📋 How to Use

### Basic Usage
1. Open `spinwheel.html` in any modern web browser
2. The wheel comes with 8 default prizes
3. Click the **SPIN** button to spin the wheel
4. Wait for the result with confetti celebration!

### Customizing Choices
1. Type your choice in the input field under "Manage Choices"
2. Click **Add** or press **Enter**
3. Your choice appears in the list below
4. Click **Remove** next to any choice to delete it
5. Changes are automatically saved

### Tips
- You need at least 2 choices to spin
- There's no maximum limit on choices
- Colors automatically cycle through 18 vibrant options
- Your choices persist even after closing the browser
- Works offline - no internet required

---

## 🎨 Color Palette

The wheel uses 18 beautiful colors that cycle through segments:

```
#FF6B6B  #4ECDC4  #45B7D1  #FFA07A  #98D8C8  #F7DC6F
#BB8FCE  #85C1E2  #F06292  #AED581  #FF8A80  #82B1FF
#B9F6CA  #FFD180  #FF80AB  #EA80FC  #80D8FF  #CCFF90
```

Confetti uses a subset of 7 colors for variety.

---

## 📱 Responsive Breakpoints

### Desktop (> 768px)
- Two-column grid layout
- Wheel max width: 400px
- Full hover effects enabled
- Title: 42px
- Result text: 28px

### Mobile (≤ 768px)
- Single-column stack layout
- Wheel max width: 280px
- Hover effects disabled
- Title: 28px
- Result text: 20px
- Compact spacing

---

## 🔧 Customization Guide

### Change Colors
Edit the `colors` array in JavaScript:
```javascript
const colors = ['#FF6B6B', '#4ECDC4', ...];
```

### Adjust Spin Duration
Modify `spinDuration` variable:
```javascript
const spinDuration = 4000; // milliseconds
```

### Change Default Choices
Edit the `segments` array:
```javascript
let segments = ['Option 1', 'Option 2', ...];
```

### Modify Confetti Amount
Change the loop count:
```javascript
for (let i = 0; i < 150; i++) { // Change 150
```

---

## 🎯 Key Features Breakdown

### Wheel Mechanics
- **Rotation Calculation** - Uses modulo arithmetic for accurate positioning
- **Pointer Detection** - Calculates winning segment based on top pointer position
- **Easing Function** - Cubic ease-out for natural deceleration
- **Random Spins** - 5-10 full rotations plus random angle

### Sound System
- **Oscillator-Based** - Creates tones programmatically
- **Tick Sound** - 800Hz sine wave, 0.05s duration
- **Win Sound** - C5-E5-G5 arpeggio chord
- **Gain Control** - Volume management for pleasant audio

### State Management
- **isSpinning Flag** - Prevents multiple simultaneous spins
- **Button Disable** - UI feedback during spin
- **LocalStorage Sync** - Automatic save on every change
- **Canvas State** - Proper save/restore for transformations

---

## 🚀 Deployment

### Local Hosting
Simply open `spinwheel.html` in a browser - no server needed!

### Web Server
Upload `spinwheel.html` to any web hosting:
- Works with GitHub Pages
- Compatible with Netlify, Vercel
- No build process required
- Single file deployment

### Python HTTP Server
```bash
python3 -m http.server 8000
```
Then visit: `http://localhost:8000/spinwheel.html`

---

## 📊 File Structure

```
/root/test/
├── spinwheel.html    # Main application (complete, standalone)
├── index.html        # Redirect to spinwheel.html
└── text.txt          # This README
```

---

## 🎓 Code Highlights

### Canvas Rendering
- High-quality image smoothing enabled
- Proper text alignment and baseline
- Shadow effects for depth
- Rotation transformations for text placement

### Animation System
- CSS keyframe animations for UI
- JavaScript requestAnimationFrame for wheel
- Staggered timing for load sequence
- Smooth 60fps performance

### Accessibility
- Semantic HTML structure
- Keyboard support (Enter key)
- Clear visual feedback
- High contrast text

---

## 🐛 Known Limitations

- Audio requires user interaction (browser policy)
- Canvas text rendering varies slightly by browser
- LocalStorage limited to ~5-10MB (more than enough)
- Very long choice names may truncate

---

## 💡 Future Enhancement Ideas

- Export/import choice lists
- Custom color picker
- Sound on/off toggle
- History of past results
- Multiple wheel templates
- Share results feature
- Dark/light theme toggle
- Weighted probabilities

---

## 📄 License

This is a custom-built application. Free to use and modify for personal or commercial projects.

---

## 🙏 Credits

- **Font**: Poppins by Google Fonts
- **Design**: Modern minimalist aesthetic
- **Sounds**: Web Audio API synthesis
- **Built with**: Pure HTML, CSS, JavaScript

---

## 📞 Support

For issues or questions:
1. Check browser console for errors
2. Ensure JavaScript is enabled
3. Try clearing browser cache
4. Test in different browser

---

**Enjoy spinning! 🎉**

Made with ❤️ for decision-making fun!
