# Starnet Office - rilis

Repo ini hanya berisi **rilis siap pakai** Starnet Office (dibuat otomatis oleh CI). Tidak perlu token.

## Windows

Buka **PowerShell** biasa (jangan *Run as administrator*), lalu:

```powershell
irm https://github.com/sigitholic/starnet-releases/releases/latest/download/install.ps1 | iex
```

Update: dobel-klik **Starnet - Update** di desktop. Kembali ke versi sebelumnya: **Starnet - Kembalikan Versi**.

## Linux (server, VPS, mini PC; x64/ARM64, systemd)

```sh
curl -fsSL https://github.com/sigitholic/starnet-releases/releases/latest/download/install.sh | sudo bash
```

Update: `sudo /opt/starnet-office/update.sh`. Kembali ke versi sebelumnya: `sudo /opt/starnet-office/rollback.sh`.

## Docker

```sh
curl -fsSL https://github.com/sigitholic/starnet-releases/releases/latest/download/install-docker.sh | bash
```

Update: `./starnet-office/update.sh`.

## Isi setiap rilis

- `starnet-bundle.zip`: Paperclip versi Starnet + plugin + adapter (sudah jadi)
- `latest.json`: versi, ukuran, dan SHA-256 paket (dicek installer)
- skrip installer dari commit yang sama
