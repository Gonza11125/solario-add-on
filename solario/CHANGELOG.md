# Changelog

## 0.6.29

- Added pre-built signed multi-architecture Home Assistant distribution for `amd64` and `aarch64`.
- First administrator setup is restricted to protected Home Assistant ingress.
- Added optional direct LAN access through port `3000/tcp`, disabled by default and intended only for trusted private networks.
- Hardened local sessions, recovery invalidation, Home Assistant command validation and delivery, runtime supervision, dependency auditing, and process credential isolation.
