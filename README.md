# quicktorrent

A command-line tool for macOS that launches qBittorrent to download a specific folder from torrent. Configure torrent path within bash file.

## 📦 Features

- Automatically launches `qBittorrent` if not already running
- Logs into the qBittorrent Web UI
- Uploads a predefined `.torrent` file
- Deselects all files in the torrent
- Selects and downloads only the folder you specify by name

## 🔧 Setup

1. **Install `jq`** (for JSON parsing):
   ```bash
   brew install jq
   ```

2. **Download and install `quicktorrent`:**
   ```bash
   chmod +x quicktorrent
   sudo mv quicktorrent /usr/local/bin/
   ```

3. **Edit the script:**
   - Set the path to your `.torrent` file
   - Set your Web UI username and password

## 🚀 Usage

```bash
quicktorrent "Folder Name To Download"
```

For example:
```bash
quicktorrent "Season 2"
```

This will set `qBittorrent` to download only the files inside the `Season 2` folder from the `.torrent`.

## 📝 Notes

- The Web UI must be enabled in qBittorrent (Preferences → Web UI).
- Assumes the folder you want is a **top-level folder** in the `.torrent`.
- The `.torrent` path is fixed in the script—ask for an argument version if needed.

