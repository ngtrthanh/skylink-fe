# Skylink FE

Real-time aircraft tracking frontend for [skylink-core](https://github.com/ngtrthanh/skylink).

## Deploy to Cloudflare Pages

1. Connect this repo to CF Pages
2. Build command: (none — static files)
3. Output directory: `/`
4. Set `window.SKYLINK_API` in `index.html` to your backend URL

## Configuration

Edit `index.html` to set the API endpoint:
```js
window.SKYLINK_API = 'https://skylink-api.hpradar.com';
```

Leave empty for same-origin (when proxied via nginx).

## Features

- 81 aircraft shape icons (SDF sprite, retina @2x)
- WebSocket real-time updates with viewport bbox
- Flight trace rendering on click
- MapManager: style switcher, projection toggle
- 462K aircraft type database → icon mapping (99% coverage)
