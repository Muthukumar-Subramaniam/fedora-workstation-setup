# 03 – Repositories & codecs

## RPM Fusion
```bash
sudo dnf install -y \
  https://mirrors.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm \
  https://mirrors.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm
```

## Flathub
```bash
flatpak remote-add --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo
```

## Multimedia codecs
```bash
sudo dnf swap ffmpeg-free ffmpeg --allowerasing
sudo dnf group install multimedia
```

## GPU drivers
<!-- NVIDIA / AMD / Intel notes -->

## Notes
