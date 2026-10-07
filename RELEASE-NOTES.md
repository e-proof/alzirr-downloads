# Alzirr 0.1.1 preview

[Download page](https://e-proof.github.io/alzirr-downloads/) · [APK](https://e-proof.github.io/alzirr-downloads/alzirr-0.1.1-android.apk) · [ZIP alternative](https://e-proof.github.io/alzirr-downloads/alzirr-0.1.1-android.zip). No GitHub account is required. The mirror and ZIP use the original, unchanged signed APK; ZIP includes license notices and the APK checksum. Extract the APK from ZIP before installing.

Android phone mode now starts and runs without an Alzirr server or account. Provider keys remain encrypted on the phone; native HTTPS connects directly to OpenAI, Anthropic, Gemini or a compatible provider. New model responses still need internet and your own provider key; no on-device language model is bundled.

Tasks, conversations, permissions, tool/model results, checkpoints, child work and Word/Excel/Markdown/text documents are kept locally. Optional server sync transfers a task family with stable action IDs and checksummed artifacts, without credentials or a model charge. Transfer and handoff intent survive lost replies; stale cloud copies cannot overwrite changed phone work. Background task snapshots are separated from the local execution ledger. Small-screen layout overflow was corrected.

- Android 8+, app ID com.alzirr.app, version 0.1.1, versionCode 2.
- APK: **705,751 bytes**; APK signature scheme v2, RSA 4096-bit identity.
- APK SHA-256: eb82c004ffbc1ddba51ce11bb4dabcade883b83991446ffc53ab1c23650ce930.
- Certificate SHA-256 unchanged: d20eb4bb3253ab0571abb96ba1ac7cb94b2de9e06e1198fbecbe7c63b3a628c8.
- Installed over versionCode 1 on the owned Android API 36 emulator; no uninstall needed.
- 60 workspace tests, including 12 real PostgreSQL integration tests; 8 Android release tests and 11 skills passed. Lint: 0 errors / 25 warnings.
- No-account mobile flow, 320 px layout, offline stored files and Arabic RTL passed.
- Actual debug APK used native Room/Keystore to create approved Word with a model fixture; force-stop/restart retained the answer and file without replay or Alzirr network calls.
- One real native HTTPS request with an invalid QA key returned HTTP 401. This confirms direct transport, not successful paid inference.
- Signed APK rendered offline; crash buffer was empty. Cold emulator sample: 3.769 seconds; physical performance and battery targets remain unverified.

Phone execution remains foreground-driven. No public production SaaS endpoint, model keys, mail accounts, S3 or Paddle merchant configuration is included. Live provider responses, OAuth/mail, payments, hosted storage, physical-device permission/battery flows and actual Linux/gVisor need operator acceptance. Release manifest is not debuggable and its code disables WebView debugging; the userdebug emulator overrides that setting, so normal-device socket absence was not verified.

The wider product plan still lacks IMAP/SMTP/full mailbox sync, resumable large files, Go/WSS PC connector, direct Codex App Server, WebRTC voice, complete sync/cloud resource permissions and administrative prices/spend budgets. This is a corrected standalone-phone preview, not completion of the whole platform. SDK remains at 0.1.0; its source and archive are available from the existing SDK release. Signing material, private source and user data are excluded.
