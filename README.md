# 🧲 Magnet Link Player

A simple, browser-based web application that allows you to stream and play videos from magnet links directly in your browser using WebTorrent technology.

## Features

- 🎬 **Stream Videos**: Play videos directly from magnet links without downloading the entire file
- 🚀 **Browser-Based**: No installation required - works entirely in your web browser
- 📊 **Real-time Stats**: Monitor download/upload speeds, peer count, and progress
- 📁 **Multi-file Support**: Automatically detects and lists all video files in a torrent
- 🎨 **Modern UI**: Clean, responsive design with a beautiful gradient interface
- ⚡ **WebRTC Technology**: Uses WebTorrent for fast, efficient peer-to-peer streaming

## How to Use

1. Open `index.html` in a modern web browser (Chrome, Firefox, Edge, or Opera)
2. Paste a magnet link into the input field
3. Click "Load Magnet Link" to start streaming
4. If the torrent contains multiple files, select the video you want to play
5. The video will start playing automatically as it downloads

## Supported Browsers

The application requires WebRTC support. Compatible browsers include:
- Google Chrome
- Mozilla Firefox
- Microsoft Edge
- Opera
- Brave

## Supported Video Formats

The player automatically detects and displays the following video formats:
- MP4
- WebM
- OGG
- MKV
- AVI
- MOV
- WMV
- FLV
- M4V

## Technology Stack

- **WebTorrent**: A streaming torrent client for the browser
- **HTML5 Video**: Native video playback
- **Vanilla JavaScript**: No frameworks required
- **CSS3**: Modern, responsive styling

## Local Development

Simply open the `index.html` file in your browser. No build process or server required!

For a better development experience, you can use a local server:

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js
npx http-server

# Using PHP
php -S localhost:8000
```

Then navigate to `http://localhost:8000` in your browser.

## Security & Privacy

- All streaming happens peer-to-peer through WebRTC
- No data is stored on external servers
- The application runs entirely in your browser
- Make sure you only load magnet links from trusted sources

## How It Works

1. **Magnet Link Parsing**: The application parses the magnet link to extract torrent information
2. **Peer Discovery**: Connects to WebTorrent trackers to find peers
3. **Piece Selection**: Intelligently downloads video pieces starting from the beginning
4. **Progressive Playback**: Streams video data to the HTML5 video player as it downloads
5. **P2P Sharing**: Simultaneously uploads downloaded pieces to other peers

## Limitations

- Requires a browser with WebRTC support
- Download speeds depend on torrent popularity and peer availability
- Large video files may take time to buffer initially
- Some browsers may limit the number of simultaneous connections

## Contributing

Contributions are welcome! Feel free to submit issues or pull requests.

## License

MIT License - feel free to use this project for any purpose.

## Disclaimer

This tool is for educational purposes. Please ensure you have the right to download and view any content you access through magnet links. Always respect copyright laws and content creator rights.