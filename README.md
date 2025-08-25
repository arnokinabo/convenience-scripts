# Convenience Scripts

A collection of small helper scripts for day-to-day development and server operations.

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

---

## 🚧 Future Scripts

Hopefully this repo grows with more utility scripts over time.

---

<div align="center">
    <em>Built with ❤️ for the robust and pretty — code that works and looks good doing it.</em>
</div>
