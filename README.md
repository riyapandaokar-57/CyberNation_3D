# CyberFiction - Interactive Scroll Animation Website

An immersive, scroll-driven web experience showcasing advanced canvas animations and smooth scrolling effects. This project was created for educational purposes to learn and demonstrate modern web animation techniques.

## 🚀 Features

- **Canvas Frame Animation**: 300-frame sequence animation that responds to scroll position
- **Smooth Scrolling**: Implemented using Locomotive Scroll for buttery-smooth navigation
- **Scroll-Triggered Animations**: GSAP ScrollTrigger integration for synchronized effects
- **Section Pinning**: Fixed sections that create engaging storytelling moments
- **Parallax Effects**: Dynamic text animations with stroke effects
- **Fully Responsive**: Adapts seamlessly to different screen sizes
- **Modern UI/UX**: Clean, minimalist design with attention to typography

## 🛠️ Tech Stack

- **HTML5 Canvas** - Frame-by-frame animation rendering
- **JavaScript (ES6+)** - Core functionality and animation logic
- **GSAP 3.11.5** - Professional-grade animation library
- **ScrollTrigger** - Scroll-based animation trigger plugin
- **Locomotive Scroll 3.5.4** - Smooth scrolling library
- **CSS3** - Styling and animations

## 📋 Prerequisites

- Modern web browser (Chrome, Firefox, Safari, Edge)
- Local web server (optional, for development)

## 🔧 Installation

1. **Download or clone the repository**
   ```bash
   cd cyberfiction
   ```

2. **Open the project**
   - Simply open `index.html` in your browser, or
   - Use a local development server:
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js (http-server)
   npx http-server
   ```

3. **View in browser**
   - Navigate to `http://localhost:8000` (or your server's address)

## 📁 Project Structure

```
cyberfiction/
│
├── index.html          # Main HTML file
├── style.css           # Styling and layout
└── script.js           # JavaScript logic and animations
```

## 🎨 Key Components

### Canvas Animation
- Loads 300 PNG frames dynamically
- Renders frames based on scroll position
- Scales images to maintain aspect ratio

### Smooth Scrolling
- Locomotive Scroll creates inertia-based scrolling
- Integrated with GSAP ScrollTrigger for precise control

### Section Animations
- **Page 1**: Keyword showcase with dual-column layout
- **Page 2**: "Have Fun" section with descriptive text
- **Page 3**: Playground concept finale

## 🎯 Customization

### Change Animation Frames
Update the `files()` function in `script.js` to point to your image sequence:
```javascript
function files(index) {
  var data = `
     ./your-image0001.png
     ./your-image0002.png
     // ... add your frames
  `;
  return data.split("\n")[index];
}
```

### Adjust Scroll Speed
Modify the `scrub` value in ScrollTrigger:
```javascript
scrollTrigger: {
  scrub: 0.15,  // Lower = faster, Higher = slower
  // ...
}
```

### Change Colors
Edit the CSS variables or directly modify colors in `style.css`:
```css
#page {
  background-color: #f1f1f1;  /* Change background */
}
```

## 🌐 Browser Support

- Chrome (recommended)
- Firefox
- Safari
- Edge
- Opera

## 📱 Responsive Design

The project automatically adapts to different screen sizes through:
- Viewport-relative units (vh, vw)
- Canvas resize event handling
- Flexible typography scaling

## ⚡ Performance Optimization

- Images are preloaded for smooth animation
- Canvas rendering is optimized with proper scaling
- GSAP's `scrub` property creates efficient scroll-linked animations

## 📚 Learning Outcomes

This project demonstrates:
- Advanced scroll-based animations
- Canvas API manipulation
- Integration of multiple JavaScript libraries
- Responsive web design principles
- Modern CSS techniques

## 📝 Educational Purpose

This project is a clone created solely for educational purposes to practice and understand:
- Modern web animation techniques
- Scroll-triggered interactions
- Canvas-based rendering
- Library integration (GSAP, Locomotive Scroll)

## 🙏 Acknowledgments

- GSAP for the powerful animation library
- Locomotive Scroll for smooth scrolling capabilities
- The web development community for tutorials and inspiration
