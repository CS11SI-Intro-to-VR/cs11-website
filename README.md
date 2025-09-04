# CS11 VR Course Website

This is the official website for Stanford CS11: "How to Make VR - Introduction to Virtual Reality Design and Development". The website features an interactive three.js background with animated particles and bloom effects.

## Project Structure

### 📁 Core Website Files

- **`index.html`** - Main homepage with course information and application details
- **`syllabus.html`** - Class materials and syllabus page
- **`index.css`** - Custom styles for the website

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

## Development Notes

### File Organization

- All three.js related files are now organized in the `threejs/` folder for better maintainability
- Core website functionality remains in the root directory
- Vendor libraries are kept in the `vendor/` folder

## Getting Started

1. **Local Development**: Simply open `index.html` in a modern web browser
2. **Web Server**: For full functionality, serve the files through a web server (due to CORS restrictions with fonts)
3. **WebGL**: Ensure your browser supports WebGL for the three.js animation
