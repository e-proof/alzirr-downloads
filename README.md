# Alzirr

A small Android personal agent with optional cloud execution. **Phone mode works without an Alzirr account or Alzirr server.**

[Download the signed APK](https://github.com/e-proof/alzirr-downloads/releases/download/v0.1.1/alzirr-0.1.1-android.apk) · [Release notes](https://github.com/e-proof/alzirr-downloads/releases/tag/v0.1.1) · [Open Extension SDK](https://github.com/e-proof/alzirr-sdk)

Android 8+. APK: **705,751 bytes** (about 0.71 MB). Languages: Türkçe, English, Deutsch, Français, Español, Português, العربية, Русский, हिन्दी, 日本語, 한국어, 中文; Arabic RTL.

## Install and use

1. Download the APK and allow installation from your browser/file app. Check SHA256SUMS.txt if you verify downloads.
2. Install and open Alzirr. Existing 0.1.0 installations can update with this APK using the same signing identity.
3. In Connections, save your own model-provider API key. The key is encrypted using Android Keystore; model requests go directly to your provider. Provider usage charges apply separately.
4. Create a task. Conversations, approved tool results, checkpoints and documents are stored on your phone and survive reopening. Word, Excel, Markdown and text documents can be generated locally.
5. Grant the Android capabilities and action permissions needed for a task. Each action approval applies to that exact action.

The APK includes no on-device language model: new model responses require internet and your provider key. Saved work and documents remain available offline. It has no installation fee. Hosted execution is optional and requires a configured HTTPS Alzirr service, an account, subscription and credits. **No public production SaaS endpoint is included.**

To synchronize or continue a phone task in cloud, connect to your service in Account, then use the task's sync/handoff controls. Work, checkpoints, stable action results and files move together; provider keys stay on the phone. The service validates the account and execution ownership, and stale cloud data cannot silently overwrite changed phone work.

Phone execution runs while the app is visible and pauses in the background. Opt-in background refresh follows Android scheduling. Cloud can continue while the phone is off; device tools wait for the app. Android permissions govern contacts, calendars, selected files, notifications and visible non-password app controls.

## Türkçe

[APK'yı indir](https://github.com/e-proof/alzirr-downloads/releases/download/v0.1.1/alzirr-0.1.1-android.apk). Açmak ve telefonda kullanmak için Alzirr hesabı veya sunucu adresi gerekmez. Bağlantılar ekranından kendi model anahtarını ekle; görevler, konuşmalar ve belgeler telefonda saklanır. Anahtar Android Keystore ile korunur, model isteği doğrudan sağlayıcıya gider.

APK içinde yerel dil modeli yoktur; yeni model yanıtı internet ve sağlayıcı anahtarı ister. Kayıtlı çalışmalar çevrimdışı açılır. Bulutla eşitleme ve ücretli sunucu kullanımı isteğe bağlıdır. Bu önizlemeye canlı genel SaaS adresi dahil değildir. Telefon yürütmesi uygulama görünürken çalışır, arka planda durur. iPhone APK çalıştırmaz; PC için web paneli vardır.

## Preview evidence and remaining scope

60 workspace tests (including 12 real PostgreSQL integration tests), 8 Android release unit tests and 11 skill checks passed. Android lint: 0 errors / 25 warnings. Native Room/Keystore execution, approved Word creation using a provider fixture and force-stop recovery passed on the Android API 36 test emulator. A real native HTTPS request with an invalid QA key returned HTTP 401; successful real inference is not yet verified. Signed APK update and offline launch passed.

Real-phone battery/performance and normal-device release debugging acceptance remain pending. Full mailbox mirroring, IMAP/SMTP, resumable large-file sync, native PC/iOS, Go/WSS connector, direct Codex App Server and WebRTC voice are not included. Phone files are limited to 1 MB. Live payments, OAuth/mail, production storage, public hosting and Linux/gVisor require operator validation. This preview does not provide unrestricted private-app data access or unattended cross-app background execution.

Application source is private; the SDK is independently MIT licensed. See [binary license](BINARY-LICENSE.md), [component notices](THIRD-PARTY-NOTICES.md), [license texts](THIRD-PARTY-LICENSES.txt) and [checksums](SHA256SUMS.txt).
