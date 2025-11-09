# 👏 Clap Counter App

A modern, interactive web application that counts claps in real-time using your computer's microphone. Built with vanilla HTML, CSS, and JavaScript - no frameworks required!

![Clap Counter Demo](https://img.shields.io/badge/Status-Active-success)
![License](https://img.shields.io/badge/License-MIT-blue)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## ✨ Features

- 🎤 **Real-time Audio Detection** - Uses Web Audio API to detect claps through your microphone
- 📊 **Live Audio Visualizer** - Visual representation of sound levels
- ⚙️ **Customizable Settings**:
  - Adjustable sensitivity slider
  - Configurable cooldown timer
- 🎨 **Modern UI/UX** - Beautiful gradient design with smooth animations
- 📱 **Responsive Design** - Works on desktop and mobile devices
- 🔒 **Privacy First** - All audio processing happens locally in your browser
- 🚀 **Zero Dependencies** - Pure vanilla JavaScript, no frameworks needed

## 🚀 Quick Start

### Option 1: Open Directly in Browser
1. Download the `index.html` file
2. Double-click to open in your default browser
3. Click "Start Listening" and allow microphone access
4. Start clapping! 👏

### Option 2: Using VS Code Live Server
1. Install the [Live Server extension](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
2. Open the HTML file in VS Code
3. Right-click and select "Open with Live Server"
4. The app will launch in your browser

### Option 3: Using Python HTTP Server
```bash
# Navigate to the project directory
cd path/to/clap-counter

# Start a local server
python -m http.server 8000

# Open browser to http://localhost:8000
```

### Option 4: Using Node.js HTTP Server
```bash
# Install http-server globally (one-time)
npm install -g http-server

# Run the server
http-server

# Open browser to displayed URL
```

## 🌐 Deploy to Production

### GitHub Pages (Recommended)

1. **Create a GitHub repository**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/Ghazi-code7/clap-counter.git
   git push -u origin main
   ```

2. **Enable GitHub Pages**
   - Go to repository Settings → Pages
   - Select `main` branch as source
   - Save and wait 1-2 minutes

3. **Access your app**
   - URL: `https://Ghazi-code7.github.io/clap-counter`

### Netlify (Easiest)

1. Visit [netlify.com](https://netlify.com)
2. Sign up for free account
3. Drag and drop your HTML file
4. Get instant live URL!

### Vercel

```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel
```

## 📖 How to Use

1. **Start Listening**: Click the "Start Listening" button
2. **Grant Permissions**: Allow microphone access when prompted by your browser
3. **Clap Away**: Start clapping your hands near your device
4. **Watch the Counter**: See the count increase with each clap
5. **Adjust Settings**: Use the sensitivity and cooldown sliders to fine-tune detection
6. **Reset**: Click "Reset" to start counting from zero

## ⚙️ Settings Explained

### Sensitivity (10-100)
- **Lower values** = More sensitive (picks up softer sounds)
- **Higher values** = Less sensitive (requires louder claps)
- **Default**: 50
- **Tip**: Adjust if the app is too sensitive or not detecting claps

### Cooldown (100-1000ms)
- Minimum time between detected claps
- Prevents counting a single clap multiple times
- **Default**: 300ms
- **Tip**: Increase if double-counting occurs, decrease for faster clapping

## 🛠️ Technical Details

### Technologies Used
- **HTML5** - Structure and markup
- **CSS3** - Styling with gradients and animations
- **JavaScript (ES6+)** - Logic and audio processing
- **Web Audio API** - Microphone access and audio analysis

### Browser Compatibility
- ✅ Chrome 74+
- ✅ Firefox 69+
- ✅ Safari 14.1+
- ✅ Edge 79+
- ⚠️ Requires HTTPS for microphone access (except localhost)

### How It Works

1. **Audio Capture**: Uses `getUserMedia()` to access microphone
2. **Analysis**: Web Audio API's `AnalyserNode` processes audio in real-time
3. **Detection**: Calculates RMS (Root Mean Square) amplitude
4. **Threshold Comparison**: Compares amplitude against sensitivity setting
5. **Cooldown Check**: Prevents double-counting using timestamp comparison
6. **Visual Feedback**: Updates counter and triggers animations

## 🔒 Privacy & Security

- ✅ All audio processing happens **locally** in your browser
- ✅ No audio data is recorded or transmitted
- ✅ No external APIs or third-party services
- ✅ Microphone access requested only when you click "Start Listening"
- ✅ You can revoke microphone permissions anytime in browser settings

## 🐛 Troubleshooting

### Microphone Access Denied
- Check browser permissions (usually a camera icon in address bar)
- Ensure you're using HTTPS or localhost
- Try a different browser

### Claps Not Detected
- Increase sensitivity (lower the threshold value)
- Clap louder or closer to the microphone
- Check if your microphone is working in other apps

### Too Sensitive / False Positives
- Decrease sensitivity (increase the threshold value)
- Increase cooldown time
- Reduce background noise

### App Not Loading
- Ensure JavaScript is enabled in your browser
- Try clearing browser cache
- Check browser console for errors (F12)

## 🎯 Use Cases

- 🎪 Entertainment and party games
- 👶 Baby learning apps
- 🎓 Educational tools for children
- 🎤 Sound detection demonstrations
- 🧪 Audio API experimentation
- 💪 Workout counting (clap burpees!)

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Ideas for Contributions
- Add sound effects for clap detection
- Implement clap pattern recognition
- Add dark/light mode toggle
- Create clapping speed analytics
- Add export/save counter data
- Multi-language support

## 📝 License

This project is licensed under the MIT License - see below for details:

```
MIT License

Copyright (c) 2025 Clap Counter App

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## 📧 Contact & Support

- **Issues**: Open an issue on GitHub
- **Questions**: Start a discussion in the repository
- **Email**: ideafuel008@gmail.com

## 🌟 Acknowledgments

- Inspired by interactive audio applications
- Built with love using Web Audio API
- Thanks to the open-source community

## 📊 Project Stats

- **Lines of Code**: ~300
- **File Size**: ~10KB
- **Load Time**: <100ms
- **Dependencies**: 0

---

Made with 💜 and 👏 | [Live Demo](#) | [Report Bug](#) | [Request Feature](#)

**⭐ Star this repo if you found it helpful!**
