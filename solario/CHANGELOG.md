# Changelog

## 0.6.30

- Hardened Solario Local for the public Free release, including stricter Home Assistant trust boundaries, timestamp validation, online/offline freshness, rate limiting, process isolation, backup protection, and safer cloud unlink/relink behavior.
- Added reliable Solario automation execution with real Home Assistant acknowledgements, delayed commands, runtime reconciliation, and protection against stale frontend state overwriting server-owned execution history.
- Free now supports one Solario automation using safe Home Assistant targets (`switch`, `light`, `fan`, `input_boolean`, and `cover`) without enabling direct manual device control.
- Home Assistant automations do not consume the Free Solario automation quota and enable/disable actions now wait for a confirmed Home Assistant result.
- Removed unfinished automation actions and obsolete manual pairing flow from the Local user interface.
- Free includes 24-hour history; Local retention now also supports the longer Smart/Pro history windows for future paid plans.
- SMART and PRO are shown as upcoming while public paid upgrades are disabled.
- Improved first-run behavior, Solar Box isolation, restart safety, local Web UI checks, and multi-architecture image validation for `amd64` and `aarch64`.

## 0.6.29

- Added pre-built signed multi-architecture Home Assistant distribution for `amd64` and `aarch64`.
- First administrator setup is restricted to protected Home Assistant ingress.
- Added optional direct LAN access through port `3000/tcp`, disabled by default and intended only for trusted private networks.
- Hardened local sessions, recovery invalidation, Home Assistant command validation and delivery, runtime supervision, dependency auditing, and process credential isolation.
