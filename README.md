# TP-Link Tapo Firmware Directory

Simple searchable directory of public firmware object keys found under `https://download.tplinkcloud.com/`.

Generated on 2026-06-23.

## Files

- `all_firmware.txt` - every `firmware/` object key found from the public key dump, plus newer firmware files discovered during local Tapo research.
- `tapo_firmware.txt` - `firmware/` keys whose filename contains `Tapo`.
- `tapo_firmware.csv` - Tapo-focused table with parsed model/build/release hints, direct download URLs, HTTP status, content length, and last-modified headers where available.

## Counts

- Firmware objects: 15188
- Tapo firmware objects: 1183
- Tapo URLs returning HTTP 200 on 2026-06-23: 1164
- Tapo URLs returning HTTP 403 on 2026-06-23: 19

## Notes

The bucket root and `firmware/` prefix currently do not allow anonymous directory listing. This repo is therefore a best-effort index of public object keys we could discover, not an official TP-Link catalog. Direct URLs use this form:

```text
https://download.tplinkcloud.com/<object-key>
```

Reference project: https://github.com/tapo-firmware/Directory
