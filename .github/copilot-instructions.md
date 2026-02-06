# GitHub Copilot Instructions for IronVector Webpage

## HTML Preview Setup

This repository contains a static HTML webpage (`IronVector.html`). Here are the recommended methods to preview the HTML file during development:

### Method 1: Using Python's Built-in HTTP Server (Recommended)

Python 3 includes a simple HTTP server that can serve static files:

```bash
# Navigate to the repository root
cd <repository-directory>

# Start the server (Python 3)
python3 -m http.server 8000

# The page will be available at: http://localhost:8000/IronVector.html
```

### Method 2: Using Node.js HTTP Server

If you have Node.js installed, you can use the `http-server` package:

```bash
# Install http-server globally (one-time setup)
npm install -g http-server

# Run the server
http-server -p 8000

# The page will be available at: http://localhost:8000/IronVector.html
```

### Method 3: Using VS Code Live Server Extension

1. Install the "Live Server" extension in VS Code
2. Right-click on `IronVector.html`
3. Select "Open with Live Server"
4. The page will open in your default browser with live reload enabled

### Method 4: Direct Browser Opening

For quick previews without a server:

```bash
# Linux
xdg-open IronVector.html

# macOS
open IronVector.html

# Windows
start IronVector.html
```

**Note:** Some features may not work correctly when opening HTML files directly (e.g., CORS restrictions, certain JavaScript features). Using a local server is recommended.

## Development Workflow

1. Make changes to `IronVector.html`
2. Refresh your browser to see updates
3. Use browser developer tools (F12) to inspect and debug

## Repository Structure

- `IronVector.html` - Main landing page for the IronVector iOS app
- `README.md` - Repository documentation

## When Working with HTML Files

- Always preview changes in a browser before committing
- Test responsiveness using browser dev tools
- Check console for JavaScript errors
- Validate HTML using W3C validator if making structural changes
