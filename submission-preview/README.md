# Add Manifold Fedimint Guardian

[Package changes](https://github.com/fedibtc/umbrel-apps/compare/master...add-manifold-fedimint-guardian) · [App files](../manifold-fedimint-guardian/)

## Type

New app

## App

- App ID: `manifold-fedimint-guardian`
- Upstream project: https://github.com/fedibtc/manifold
- Version: `0d31e0b7`

## Summary

Operate guardian seats for multiple Fedimint federations and earn fees from a single node.

## Verification

- Umbrel 1.7.3 / amd64: fresh install, browser setup, password login, restart
  and same-image package update passed. Identity and settings were preserved.
- Unauthenticated admin requests were rejected, including from another container.
- Official lint and image checks: 0 errors; UDP-range warning checked manually.
  Public images verified for amd64 and arm64; no arm64 runtime test performed.

Testing used a disposable identity and an untrusted test credential, with seat
offers disabled. No production guardian seats were created. Telemetry
registration logged a warning with that test credential.

## Notes

Requires Bitcoin Node on mainnet and guardian authorization to offer seats.
The dashboard uses the app password shown by Umbrel. Umbrel login stays enabled.
Only guardian UDP ports are published. Backups exclude telemetry journals.

The manifest leaves `gallery: []` for Umbrel's final artwork.

<img src="assets/logo.svg" width="256" height="256" alt="Manifold Fedimint Guardian">

![Overview](assets/overview.png)

![Seats](assets/seats.png)

![Guardian fees](assets/guardian-fees.png)

Prepared with AI assistance by Codex (GPT-6), agent `/root`.
