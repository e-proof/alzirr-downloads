# Alzirr 0.1.0 preview

Signed Android APK with 12 language packs and a PC web dashboard. The service supports provider BYOK, task/conversation checkpoints, file versions, phone/cloud ownership transfer, bounded child agents, permission gates, Gmail/Outlook OAuth, HTTPS/MCP/SSH connectors, schedules and subscription/credit accounting.

This is a **preview requiring a configured HTTPS Alzirr server**, not a live hosted-service announcement. No public production endpoint, API-provider keys, mail accounts, S3 bucket or Paddle merchant configuration is included.

- Android 8+, app ID `com.alzirr.app`, version `0.1.0`, versionCode `1`.
- APK: 478,692 bytes; APK signature scheme v2, RSA 4096-bit identity.
- Certificate SHA-256: `d20eb4bb3253ab0571abb96ba1ac7cb94b2de9e06e1198fbecbe7c63b3a628c8`.
- Same-key updates were exercised on Android API 36 emulator. Keep this signing identity for later updates.
- 49 workspace tests (11 PostgreSQL integration), 3 standalone SDK tests, 6 Android unit tests passed. Android lint: 0 errors / 24 warnings.
- TR/AR mobile and desktop browser smoke passed without browser exceptions.
- Emulator warm sample: 2.151 seconds; real-device power and speed acceptance remains pending.

Phone execution pauses in the background. Cloud execution can continue independently; device tools wait for the app. Automatic full-mailbox mirroring, unrestricted/private-app data access, unattended cross-app background control, native PC and iOS apps are not included. Unknown model reservations and non-runner external effects need operator reconciliation. Hosted integration and real Linux/gVisor verification remain deployment work.

The SDK archive is MIT licensed and includes JavaScript and TypeScript definitions only. Application binaries use the included preview binary license. Signing keys, user data and private core source are excluded from this public release.
