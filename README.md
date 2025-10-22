# miniPaint - Online Image Editor

![miniPaint](images/favicon.png)

**miniPaint** is a free, open-source online image editor that lets you create and edit images using HTML5 technologies. It's a browser-based alternative to Photoshop that requires no installation and runs entirely in your web browser.

## 🌟 Key Features

- **100% Browser-Based** - No installation required, works instantly in your browser
- **Professional Photo Editing** - Advanced editing tools similar to desktop applications
- **Multi-Layer Support** - Complete layer management system
- **40+ Effects & Filters** - Including Instagram-style filters and professional effects
- **Multi-Language** - Supports 16+ languages including English, Chinese, Japanese, Korean, and more
- **Free & Open Source** - MIT licensed

## 📋 Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Development](#development)
- [Usage](#usage)
- [Tools & Capabilities](#tools--capabilities)
- [Browser Support](#browser-support)
- [Contributing](#contributing)
- [License](#license)

## ✨ Features

### Drawing Tools
- **Brush Tools**: Brush, Pencil, Eraser
- **Fill Tools**: Fill, Gradient
- **Clone Tool**: Clone stamp for duplicating image areas
- **Selection Tools**: Rectangle select, Magic wand, Color picker
- **Shape Tools**: 20+ shapes including:
  - Arrow, Bezier Curve, Callout
  - Ellipse, Rectangle, Polygon
  - Heart, Star, Moon, Hexagon
  - And many more geometric shapes
- **Text Tool**: Add and edit text with custom fonts
- **Special Effects**: Blur, Sharpen, Desaturate, Bulge/Pinch

### File Operations
- **Create & Open**:
  - New document creation
  - Open from local file/directory
  - Open from webcam
  - Open from URL or Data URL
  - Image search functionality
- **Save & Export**:
  - Export to multiple formats (PNG, JPG, GIF, etc.)
  - Save as Data URL
  - Print support
  - Quick save/load (F9/F10)

### Edit Functions
- Undo/Redo (Ctrl+Z / Ctrl+Y)
- Copy/Paste with clipboard support
- Selection operations (Delete, Copy, Select All)
- Delete, Copy, and manipulate selections

### Image Processing

#### Basic Operations
- Canvas size adjustment
- Trim/Crop images
- Resize with quality preservation
- Rotate at any angle
- Flip (Vertical/Horizontal)
- Translate/Move images
- Opacity adjustment

#### Color Adjustments
- Color corrections panel
- Auto adjust colors
- Decrease color depth
- Color palette management
- Histogram analysis

### Layer Management
- **Multi-layer editing system** with full control:
  - Create, duplicate, delete layers
  - Show/hide layer visibility
  - Reorder layers (move up/down)
  - Layer composition modes
  - Rename layers
  - Clear layer content
  - Convert to raster
  - Merge down & flatten image
  - Layer differences detection

### Effects & Filters (40+)

#### Common Filters
- Gaussian Blur
- Brightness & Contrast
- Grayscale
- Hue Rotate
- Negative/Invert
- Saturate
- Sepia
- Shadow

#### Instagram-Style Filters
- 1977
- Aden
- Clarendon
- Gingham
- Inkwell
- Lo-fi
- Toaster
- Valencia
- X-Pro II

#### Advanced Effects
- Black and White conversion
- Borders
- Blueprint effect
- Box Blur
- Denoise
- Dither
- Dot Screen
- Edge detection
- Emboss
- Enrich
- Grains/Film grain
- Heatmap
- Mosaic/Pixelate
- Night Vision
- Oil painting effect
- Pencil sketch
- Sharpen
- Solarize
- Tilt Shift
- Vignette
- Vibrance
- Vintage
- Zoom Blur

### Advanced Tools
- **Sprites**: Sprite sheet management
- **Key-Points**: Annotation and marking
- **Content Fill**: Smart content-aware fill
- **Color Zoom**: Magnify color details
- **Replace Color**: Selective color replacement
- **Restore Alpha**: Alpha channel restoration

### View & Navigation
- **Zoom Controls**:
  - Zoom in/out
  - Original size (100%)
  - Fit to window
- **Grid Display**: Customizable grid overlay
- **Guides**: Insert, update, and remove guides
- **Ruler**: Show/hide rulers
- **Full Screen Mode**: Distraction-free editing
- **Preview Panel**: Real-time preview of changes

### Additional Features
- **Animation Support**: Create and edit animations
- **Keyboard Shortcuts**: Complete shortcut system for faster workflow
- **Search Function**: Quick search for tools and functions (F3)
- **Responsive Design**: Works on desktop and mobile devices
- **Settings Panel**: Customizable preferences
- **EXIF Data Support**: Read and preserve image metadata

## 🚀 Installation

### Quick Start (Static Files)

1. Clone the repository:
```bash
git clone https://github.com/viliusle/miniPaint.git
cd miniPaint
```

2. Open `index.html` in your web browser

That's it! No build process required for basic usage.

### Development Setup

For development with hot reload:

1. Install dependencies:
```bash
npm install
```

2. Start development server:
```bash
npm run server
```

3. Build for production:
```bash
npm run build
```

The production build will be created in the `dist/` directory.

## 💻 Development

### Project Structure

```
miniPaint/
├── dist/                   # Compiled production files
├── src/
│   ├── css/               # Stylesheets
│   ├── js/
│   │   ├── actions/       # Redux-style actions
│   │   ├── core/          # Core functionality
│   │   ├── modules/       # Feature modules
│   │   │   ├── edit/      # Edit operations
│   │   │   ├── effects/   # Image effects
│   │   │   ├── file/      # File operations
│   │   │   ├── image/     # Image processing
│   │   │   └── layer/     # Layer management
│   │   ├── tools/         # Drawing tools
│   │   └── languages/     # Translations
│   ├── app.js             # Application entry
│   └── config.js          # Configuration
├── images/                # Icons and assets
├── examples/              # Usage examples
├── index.html            # Main HTML file
└── package.json          # Dependencies
```

### Tech Stack

- **HTML5 Canvas**: Core rendering engine
- **JavaScript (ES6+)**: Modern JavaScript with Babel transpilation
- **Webpack 5**: Module bundler
- **jQuery**: DOM manipulation (being phased out)
- **Key Libraries**:
  - `pica`: High-quality image resizing
  - `gif.js`: GIF animation support
  - `exif-js`: EXIF metadata reading
  - `alertifyjs`: User notifications
  - `file-saver`: File download functionality

### Available Scripts

```bash
# Start development server with hot reload
npm run server

# Build for development (unminified)
npm run dev

# Build for production (minified)
npm run build
```

## 📖 Usage

### Basic Workflow

1. **Create or Open an Image**:
   - File → New (create blank canvas)
   - File → Open → Open File (load existing image)
   - File → Open from Webcam (capture from camera)

2. **Edit Your Image**:
   - Select tools from the left sidebar
   - Adjust tool properties in the top attributes bar
   - Use layers panel on the right for layer management

3. **Apply Effects**:
   - Effects menu → Choose from 40+ effects
   - Adjust effect parameters in the dialog
   - Preview changes in real-time

4. **Save Your Work**:
   - File → Export (Ctrl+S) - choose format
   - File → Quick Save (F9) - save current state
   - File → Save As Data URL - get base64 string

### Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Ctrl+Z` | Undo |
| `Ctrl+Y` | Redo |
| `Ctrl+C` | Copy to clipboard |
| `Ctrl+V` | Paste |
| `Ctrl+A` | Select all |
| `Del` | Delete selection |
| `O` | Open file |
| `S` | Export |
| `N` | New layer |
| `D` | Duplicate layer |
| `R` | Resize image |
| `T` | Trim image |
| `F` | Auto adjust colors |
| `I` | Image information |
| `G` | Toggle grid |
| `F3` | Search |
| `F9` | Quick save |
| `F10` | Quick load |

View all shortcuts: Help → Keyboard Shortcuts

## 🌐 Browser Support

miniPaint works in all modern browsers that support:
- HTML5 Canvas
- ES6 JavaScript (or browsers with Babel polyfills)
- FileReader API
- Blob API

**Recommended Browsers**:
- Chrome/Edge (Latest)
- Firefox (Latest)
- Safari (Latest)
- Opera (Latest)

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork the repository**
2. **Create a feature branch**: `git checkout -b feature/amazing-feature`
3. **Commit your changes**: `git commit -m 'Add amazing feature'`
4. **Push to the branch**: `git push origin feature/amazing-feature`
5. **Open a Pull Request**

### Development Guidelines

- Follow the existing code style
- Test your changes in multiple browsers
- Update documentation as needed
- Add comments for complex logic


⭐ If you find miniPaint useful, please consider giving it a star on GitHub!