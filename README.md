# CS11 VR Course Website

This is the official website for Stanford CS11: "How to Make VR - Introduction to Virtual Reality Design and Development". The website features an interactive three.js background with animated particles and bloom effects.

## Project Structure

### 📁 Core Website Files

- **`index.html`** - Main homepage with course information and application details
- **`syllabus.html`** - Class materials and syllabus page
- **`resources.html`** - Resources and tutorials for students
- **`index.css`** - Custom styles for the website

### 📁 Three.js Animation System (`threejs/`)

The website features a beautiful animated background built with three.js. All related files are organized in the `threejs/` folder:

#### `threejs/lib/` - Core Libraries

- **`three.min.js`** - Core three.js library for 3D graphics
- **`Detector.js`** - WebGL support detection
- **`stats.min.js`** - Performance monitoring (FPS counter)
- **`dat.gui.min.js`** - Debug GUI for development

#### `threejs/shaders/` - Visual Effects

- **`EffectComposer.js`** - Post-processing pipeline manager
- **`RenderPass.js`** - Basic scene rendering pass
- **`ShaderPass.js`** - Custom shader effects framework
- **`CopyShader.js`** - Screen copying utilities
- **`LuminosityHighPassShader.js`** - Bright area detection for bloom
- **`UnrealBloomPass.js`** - Main bloom glow effect

#### `threejs/assets/` - Textures and Fonts

- **`particle-white.png`** - White particle texture for floating particles
- **`Quicksand Light_Regular.json`** - Font file for the 3D "CS11: How to Make VR" title

#### `three_index.js` - Main Scene Script

The main scene file that creates:

- **Floating Particles**: 40 animated particles with purple color (#5f0089)
- **3D Text**: Animated course title with normal material
- **Bloom Effects**: Post-processing glow effects
- **Camera Animation**: Subtle floating motion for the text
- **Responsive Design**: Adapts to mobile/desktop screen sizes

### 📁 Website Assets

#### `img/` - Images

- **`logo-trans.png`** - Stanford CS11 logo (transparent background)
- **`vr-for-everyone.jpg`** - Homepage hero image
- **`kingdom-watcher.png`** - VR game screenshot
- **`ar-meta.jpg`** - AR/Meta technology image
- **`greybox.jpg`** - Greyboxing tutorial image (used in resources page)

#### `css/` - Stylesheets

- **`one-page-wonder.min.css`** - Bootstrap template styles

#### `vendor/` - Third-party Libraries

- **`bootstrap/`** - Bootstrap CSS and JS framework
- **`jquery/`** - jQuery library

## Technical Features

### Three.js Background Animation

The website's signature feature is an interactive 3D background that includes:

- **Particle System**: 40 floating particles with physics-based movement
- **Bloom Post-Processing**: Creates a soft glow effect around bright objects
- **3D Typography**: Course title rendered as 3D geometry with animated floating motion
- **Responsive Animation**: Adapts particle count and text size for mobile devices
- **Performance Optimized**: Uses efficient rendering techniques for smooth animation

### Browser Compatibility

- **WebGL Required**: The three.js animation requires WebGL support
- **Fallback**: Detector.js provides WebGL capability detection
- **Mobile Optimized**: Responsive design works on mobile devices

## Development Notes

### File Organization

- All three.js related files are now organized in the `threejs/` folder for better maintainability
- Core website functionality remains in the root directory
- Vendor libraries are kept in the `vendor/` folder

## Getting Started

1. **Local Development**: Simply open `index.html` in a modern web browser
2. **Web Server**: For full functionality, serve the files through a web server (due to CORS restrictions with fonts)
3. **WebGL**: Ensure your browser supports WebGL for the three.js animation
