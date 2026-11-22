# 02 – First boot & system updates

```bash
sudo dnf upgrade --refresh -y
sudo reboot
```

## Speed up dnf
Add to `/etc/dnf/dnf.conf`:
```ini
max_parallel_downloads=10
fastestmirror=True
```

## Set hostname
```bash
sudo hostnamectl set-hostname <name>
```

## Firmware updates
```bash
sudo fwupdmgr refresh --force && sudo fwupdmgr get-updates && sudo fwupdmgr update
```

## Notes
