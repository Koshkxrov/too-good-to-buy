# PWA Setup Instructions

## Files Created/Updated

### 1. Web Manifest (`manifest.webmanifest`)
- Defines the app as a PWA with standalone display
- Theme color: #0e7c71 (teal)
- Icons: 192x192 and 512x512 PNG files

### 2. Service Worker (`sw.js`)
- Minimal service worker for offline functionality
- Caches essential files for offline use
- Handles install, fetch, and activate events

### 3. Updated HTML Files
All HTML files now include:
- PWA meta tags for iOS full-screen support
- `viewport-fit=cover` for safe area handling
- Apple touch icons and favicon links
- Service worker registration

### 4. CSS Updates
- `100dvh` instead of `100vh` for better mobile support
- `env(safe-area-inset-*)` for iOS safe areas
- Proper padding to avoid Safari UI elements

## Icon Generation

1. Open `generate-icons.html` in a browser
2. Click "Download 192x192" and "Download 512x512"
3. Save the downloaded files as `icon-192.png` and `icon-512.png`
4. Place them in the root directory

## Installation

1. Serve the files from a web server (required for PWA)
2. Open in Safari on iOS
3. Tap "Add to Home Screen"
4. The app will open in full-screen mode

## Features

- ✅ Full-screen iOS app experience
- ✅ Offline functionality via service worker
- ✅ Safe area handling for notched devices
- ✅ Proper theme colors and icons
- ✅ Standalone display mode
- ✅ No Safari UI elements when installed

## Testing

- Test on iOS Safari for full-screen experience
- Test offline functionality by disabling network
- Verify icons appear correctly on home screen
- Check safe area handling on notched devices
