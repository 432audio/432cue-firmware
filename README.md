# 432Cue Firmware

Official firmware **binaries** for the **432Cue** wireless presenter cue/control system
by **432 Audio**.

> This repository contains compiled firmware images only — **no source code**.
> It exists so 432Cue devices can be updated in the field without a laptop.

## How updates work

432Cue receivers update **over the air, with no cloud and no internet on the device**:

1. Download the latest `.bin` (links below) onto a phone or laptop.
   - **Phone tip:** make sure the file is actually **downloaded to local storage**
     (not a cloud placeholder), or the upload will fail on the device's offline Wi‑Fi.
2. Connect to the receiver's own Wi‑Fi (`432Cue-XXXX`) and open `http://192.168.4.1`.
3. **Device → Firmware update** → pick the `.bin` → enter the update PIN → **Upload & flash**.
4. The receiver flashes itself and reboots. The running version is shown on the OLED.

Nothing is sent to or from the internet during the update — the file goes straight from
your device to the receiver over its local access point.

## Latest firmware

| Product | Version | Download |
|---|---|---|
| Receiver | **0.1.5** | [432cue-receiver-0.1.5.bin](firmware/432cue-receiver-0.1.5.bin) |

Machine-readable version info: [`manifest.json`](manifest.json).

## Verifying a download (optional)

Each release lists a SHA‑256. To verify on Windows:

```powershell
Get-FileHash .\432cue-receiver-0.1.2.bin -Algorithm SHA256
```

---

© 432 Audio. Firmware binaries for authorised 432Cue hardware.
