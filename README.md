# QEntry releases

Installer packages for **QEntry**, queue management for bank branches, clinics, pharmacies and restaurants: ticket kiosk, counter caller, waiting-room display with Indonesian voice announcements, counter tablets, restaurant waitlist and an admin dashboard. QEntry runs on one server PC in your own network.

This repository holds no source code. Download a package from **Releases**.

## Which file

| File | Server PC | Realtime |
|---|---|---|
| `qentry-<version>-windows.zip` | Windows 10/11 | WebSocket |
| `qentry-<version>-linux.zip` | Linux | WebSocket |
| `qentry-<version>-sse-windows.zip` | Windows 10/11 | Server-Sent Events |
| `qentry-<version>-sse-linux.zip` | Linux | Server-Sent Events |

Both variants work the same for users. Take the one your supplier recommends; the SSE variant needs no WebSocket support in a proxy in front of the server.

## Install or update

1. Install Docker (Docker Desktop on Windows).
2. Unzip into a folder named `qentry`. An update unzipped over it keeps the server's own `.env`.
3. Run `install.bat` (Windows) or `install.sh` (Linux).
4. Open `http://<server>/dashboard/` and activate the license with the key from your supplier.

`SERVER_GUIDE.md` and `USER_GUIDE.md` in the zip explain the rest (Bahasa Indonesia: `SERVER_GUIDE.id.md`, `USER_GUIDE.id.md`).

## License

QEntry is proprietary software. Copyright (c) 2026 Cipta Bramana. All rights reserved.

Each installation needs a license key for its server PC, from the Licensor or an authorized supplier. Use is governed by the [QEntry Software License Agreement](LICENSE) (Bahasa Indonesia and English; the Indonesian text prevails). In short: you may run QEntry on the licensed server and its connected devices for your own queues; you may not copy, modify, reverse engineer, resell, or redistribute it, or bypass the license check. Open-source components keep their own licenses, listed in [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).

Support, installation and license renewals: contact your QEntry supplier.
