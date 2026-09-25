# Video Timeline Editor Web App

A powerful, browser-based video editing tool that lets you arrange, preview, and export video clips directly in your web browser. No server-side processing required - everything runs locally on your machine.

![Video Timeline Editor](https://via.placeholder.com/800x400?text=Video+Timeline+Editor)

## ✨ Features

- **Drag & Drop Interface** - Easily add video files by dragging them into the application
- **Visual Timeline** - Arrange and reorder clips with intuitive drag-and-drop controls
- **Clip Preview** - Click any clip to preview it in the video player
- **Keyboard Shortcuts** - Press Delete/Backspace to remove selected clips
- **Playback Controls** - Play and pause your timeline with dedicated buttons
- **Export to WEBM** - Combine all clips into a single WEBM video file with audio
- **Real-time Progress** - Visual feedback during playback and export
- **Responsive Design** - Works on desktop and mobile devices

## 🚀 Live Demo

Try it live at: [GitHub Pages Link Coming Soon]

## 📋 Prerequisites

- A modern web browser (Chrome, Firefox, Edge, or Safari)
- JavaScript enabled
- WebM-compatible browser for export functionality

## 🛠️ Installation

1. Clone the repository:
```bash
git clone https://github.com/souzamonteiro/videotimelineeditorwebapp.git
```

2. Navigate to the project directory:
```bash
cd videotimelineeditorwebapp
```

3. Open `index.html` in your web browser, or serve it using a local server:
```bash
# Using Python 3
python -m http.server 8000

# Using Node.js
npx http-server
```

4. Visit `http://localhost:8000` in your browser

## 📖 Usage Guide

### Adding Videos
- Drag and drop video files into the drop zone
- Click the drop zone to browse and select files
- Supported formats: MP4, WebM, OGG, and other browser-supported video formats

### Arranging Clips
- Drag clips left or right on the timeline to reorder them
- Click any clip to preview it in the video player
- Press Delete or Backspace to remove the selected clip

### Playing Your Timeline
- Click the **Play** button to start playback from the selected clip
- Click **Pause** to stop playback
- The progress bar shows current playback position

### Exporting
1. Arrange your clips in the desired order
2. Click **Export as WEBM**
3. Wait for the export process to complete
4. Your browser will automatically download the combined video

## 🔧 Technical Details

### Built With
- Pure HTML5, CSS3, and JavaScript
- Web Audio API for audio processing
- MediaRecorder API for video export
- Canvas API for video compositing

### Browser Support
- Chrome 50+
- Firefox 50+
- Edge 79+
- Safari 14+

### Export Specifications
- Format: WebM
- Video Codec: VP9 (fallback to VP8)
- Audio Codec: Opus
- Frame Rate: 30 fps

## 🚧 Limitations

- Maximum video resolution and length depend on your browser and system resources
- Export time increases with the number and length of clips
- Some video formats may not be supported depending on your browser
- Audio may not be available in all browsers due to autoplay policies

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.

```
Copyright 2026 Roberto Luiz Souza Monteiro

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```

## 📞 Contact

Project Link: [https://github.com/souzamonteiro/videotimelineeditorwebapp](https://github.com/souzamonteiro/videotimelineeditorwebapp)

## 🙏 Acknowledgments

- Thanks to all contributors who help improve this project
- Inspired by the need for simple, browser-based video editing tools

---

**Note**: This is a client-side application. All video processing happens in your browser, and your videos never leave your computer.
## Maia Reel visual theme

The interface uses the shared Maia Reel dark theme in `www/maia-reel.css`,
loaded after the app's layout styles. It is a local static asset: no CDN, build
step or new server is needed. Media processing and user-selected video title
styles remain under the original application code's control.

The canonical stylesheet and deployment instructions are maintained in the
sibling `maia-edge-apps-deployment` repository, in `themes/maia-reel.css` and
`docs/MEDIA-THEME.md`. The PWA cache has a new version and is scoped to this app.
