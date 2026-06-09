# 432Cue Firmware

Official firmware **binaries** for the **432Cue** wireless presenter cue/control system
by **432 Audio**.

> This repository contains compiled firmware images only — **no source code**.
> It exists so 432Cue devices can be updated in the field without a laptop.

## How updates work

432Cue receivers update **over the air, with no cloud and no internet on the device**.

**Easiest — one tap from the device's own page:** connect to the receiver's Wi‑Fi
(`432Cue-XXXX`), open `http://192.168.4.1` → **Device**. If a newer version exists, an
**"Update available"** banner appears — tap **Update now** and it fetches and flashes itself.
(The phone needs internet; the receiver does not.)

**Manual** (fallback / offline): download the latest `.bin` below, then on the device page →
**Device → Firmware update → Manual update** → pick the file → enter the PIN → **Upload & flash**.
- **Phone tip:** make sure the file is actually **downloaded to local storage** (not a cloud
  placeholder), or the upload can fail on the device's offline Wi‑Fi.

Nothing crosses the internet during the flash itself — the image goes straight to the receiver
over the local connection.

## Latest firmware

| Product | Version | Download |
|---|---|---|
| Receiver | **0.1.6** | [432cue-receiver-0.1.6.bin](firmware/432cue-receiver-0.1.6.bin) |

Machine-readable version info: [`manifest.json`](manifest.json).

## Verifying a download (optional)

Each release lists a SHA‑256. To verify on Windows:

```powershell
Get-FileHash .\432cue-receiver-0.1.6.bin -Algorithm SHA256
```

---

© 432 Audio. Firmware binaries for authorised 432Cue hardware.
