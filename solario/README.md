# Solario Local

Solario Local connects Home Assistant energy data with the Solario local dashboard and optional Solario cloud services.

## Installation

This app is distributed as a pre-built multi-architecture container image and supports `amd64` and `aarch64` Home Assistant systems.

The protected Home Assistant ingress is always available. Optional direct LAN access is also supported: after the first setup, assign a host port to `3000/tcp` in the app Network settings and open the displayed Web UI address. The direct port is disabled by default.

## First setup

Create the first Solario administrator only through Home Assistant ingress. This prevents another device on the same local network from claiming a fresh installation before its owner does. After the administrator exists, direct LAN access uses the normal Solario login.

## Release status

Version 0.6.29 is prepared for release but must not be published to the default branch until the private source security integration, CI/build checks, and matching public container image are complete.
