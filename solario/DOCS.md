# Solario Local documentation

## Access

After installation, start Solario Local and open it through Home Assistant ingress.

Direct LAN access is optional and disabled by default. To enable it, open the Solario Local app configuration in Home Assistant, assign a host port to `3000/tcp` under Network, save, and restart the app if Home Assistant requests it. The Web UI link then resolves to `http://<HOME_ASSISTANT_IP>:<PORT>`.

## First setup

Complete the first administrator setup only from the protected Home Assistant ingress interface. Direct LAN requests are deliberately not allowed to create the first administrator. After setup, the direct LAN interface can be used with the normal Solario login.

Keep access and recovery credentials in a safe place.

## Configuration

Solario can automatically discover exact Home Assistant energy metrics. Optional entity fields are available for manual overrides when needed.

## Updates

Home Assistant will offer a new version when this repository publishes a newer app version and matching container image.

## Security

The direct LAN listener is intended only for trusted private networks. Do not forward its port from the router to the public internet. Home Assistant ingress remains the recommended access path when direct LAN access is not needed.

Report suspected security issues privately rather than posting credentials, tokens, or exploit details in public issues.
