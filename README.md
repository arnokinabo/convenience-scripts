# Convenience Scripts

A collection of small helper scripts and guides for day-to-day development and server operations.

They are written for Linux/Unix environments (Bash + standard GNU tools). They may also work on macOS, or under Windows, through WSL or Git Bash, though these remain untested.

## ⚙️ Setup

After cloning this repo, ensure the scripts are executable:
```bash
chmod +x ~/convenience-scripts/*
```

Add the script folder to your `$PATH` by appending this line to your shell config (`~/.bashrc`, `~/.zshrc` or other):

```bash
export PATH="$HOME/convenience-scripts:$PATH"
```

Then reload:

```bash
source ~/.bashrc
```

Now you can call the scripts directly from anywhere:

```bash
docker-runtime arnie's-container
```

---

## 📜 Scripts

### `docker-runtime`

Reports the runtime (elapsed or completed duration) of a Docker container and shows logs.

```bash
# Basic usage (status + last 50 logs)
docker-runtime <container_name>

# Follow logs live while running
docker-runtime <container_name> --follow
```

### `file-sync`

Safely copy or sync large/growing files (e.g. SQLite databases) or entire folders across devices, say, your local host to a remote VM. Requires that `rsync` be installed on both devices. Source and destination paths, and others are set in the script itself. Includes cron job usage for an envisaged data transfer pipeline.

```bash
# Basic usage
file-sync
```

---

## 📖 Guides

### `network-share`

Setup guide for NFS folder sharing with automount over any IP-reachable network (LAN/VPN/Tailscale). Includes troubleshooting for cloud VM environments where reverse DNS may not work.

---

## 🚧 Future Scripts

Hopefully this repo grows with more utility scripts over time.

---

<div align="center">
    <em>Built with ❤️ for the robust and pretty — code that works and looks good doing it.</em>
</div>
