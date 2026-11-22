# 04 – Packages & apps

## DNF packages
```bash
sudo dnf install -y git curl wget vim htop tmux zsh
```

## Media: VLC
Requires RPM Fusion + codecs first (see [03](03-repositories-and-codecs.md)).
```bash
sudo dnf install -y vlc
```
Verify video playback:
```bash
vlc --version
vlc <some-video.mp4>      # check picture + audio
vainfo                    # hardware decode (needs libva-utils)
```
If video is black/stuttering: Tools → Preferences → Input/Codecs → Hardware-accelerated decoding → try Disable / VA-API.

## Torrent: qBittorrent
```bash
sudo dnf install -y qbittorrent
```
- Default WebUI/ports: Tools → Options → Connection (set listening port, open it in firewalld if needed):
```bash
sudo firewall-cmd --permanent --add-port=<port>/tcp --add-port=<port>/udp && sudo firewall-cmd --reload
```

## Flatpak apps
```bash
flatpak install -y flathub <app-id>
```

## Other (manual) installs
| App | Method | Notes |
|-----|--------|-------|
|     |        |       |
