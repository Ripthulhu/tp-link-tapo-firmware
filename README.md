# TP-Link Tapo Firmware Directory

Simple searchable directory of public firmware object keys found under `https://download.tplinkcloud.com/`.

Generated on 2026-06-23.

## Files

- `all_firmware.txt` - every `firmware/` object key found from the source data.
- `tapo_firmware.txt` - Tapo/TC camera firmware keys.
- `tapo_firmware.csv` - Tapo-focused table with parsed model/build/release hints, exact object keys, direct download URLs, source, HTTP status, content length, and last-modified headers where available.

## Counts

- Firmware objects: 15268
- Tapo/TC firmware objects: 1261
- Tapo/TC URLs returning HTTP 200 on 2026-06-23: 1252
- Tapo/TC URLs returning HTTP 403 on 2026-06-23: 9

## Sources

- `tapo-firmware/Directory` public `all_keys.txt` snapshot.
- Local 2026 FAQ 4191 sweep artifacts from prior Tapo firmware research. These include newer exact keys under paths such as `firmware/assigned/...`.

## Notes

Public downloads work when the exact object key is known, but anonymous directory listing is not currently exposed. The CloudFront download host returns an empty body for root/prefix/list-style requests, and direct S3 `ListBucket` requests return `AccessDenied`. This repo is therefore a best-effort index of public object keys we could discover, not an official TP-Link catalog. Direct URLs use this form:

```text
https://download.tplinkcloud.com/<object-key>
```

Reference project: https://github.com/tapo-firmware/Directory
