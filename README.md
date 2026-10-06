# Alzirr

A small Android personal-agent preview, with work that can continue on a configured Alzirr cloud service. **This preview needs a configured HTTPS server. A public production endpoint is not included.**

[Download the signed Android APK](https://github.com/e-proof/alzirr-downloads/releases/download/v0.1.0/alzirr-0.1.0-android.apk) · [Release notes](https://github.com/e-proof/alzirr-downloads/releases/tag/v0.1.0) · [Open Extension SDK](https://github.com/e-proof/alzirr-sdk)

Android 8 or newer. APK: about **0.48 MB**. Interface languages: Türkçe, English, Deutsch, Français, Español, Português, العربية, Русский, हिन्दी, 日本語, 한국어, 中文. Arabic uses a right-to-left layout.

## Install

1. Download the APK from the release link. Check `SHA256SUMS.txt` if you verify downloads.
2. Allow Android installation for the browser/file app used to open this download, then install.
3. Open Alzirr, go to the account screen, and save the HTTPS address supplied by your Alzirr service operator.
4. Create an account. Connect your own model-provider API key for phone execution. Provider charges are separate from the application.
5. Grant only the Android capabilities and tool/resource permissions needed for your work. Email connection is completed through the signed-in web dashboard in the system browser.

The APK has no purchase fee. Hosted cloud execution is separate and requires an activated subscription and credits. Phone mode also uses the configured server for authentication, model routing and synchronization; there is no bundled offline language model. Work, conversation history, file versions and task checkpoints can be synchronized to that server.

Phone execution pauses in the background. Cloud execution can continue while the phone is off; phone capabilities wait for the app. Access to contacts, calendars, selected documents, notifications and visible non-password app controls depends on Android permissions. This preview does not provide unrestricted access to private app databases or unattended cross-app background control. Native PC/iOS applications and automatic full-mailbox mirroring are not included; the dashboard is available in a PC browser.

## Türkçe

[İmzalı APK’yı indir](https://github.com/e-proof/alzirr-downloads/releases/download/v0.1.0/alzirr-0.1.0-android.apk). Android 8+ üzerinde doğrudan kurulabilir. Uygulamayı açıp hesap ekranına hizmet sağlayıcınızın **HTTPS sunucu adresini** girin. Bu önizlemeye canlı genel SaaS adresi dahil değildir.

Telefon modu kendi model API anahtarınızı kullanır; sağlayıcı ücretleri ayrıdır. Ücretli bulut modu ayrıca abonelik ve kredi ister. Telefon, PC web paneli ve sunucu aynı görev geçmişini ve çalışma dosyalarını kullanabilir. Telefonda yürütme arka planda durur; bulut görevi devam edebilir. İzinler Android’in ve bağlı servislerin sınırlarına tabidir. iPhone APK çalıştırmaz.

## Preview validation

The private workspace passed 49 tests, including 11 real PostgreSQL integration tests; the standalone SDK passed 3 tests. The release passed 6 native unit tests and lint with 0 errors and 24 warnings. It was installed and updated on an Android API 36 emulator. APK signature verification passed. A warm-opening emulator sample was 2.151 seconds; real-phone battery and performance remain unmeasured.

Real provider, OAuth, hosted storage and Paddle merchant flows need operator validation before production service activation. The application source is private; the SDK is independently MIT licensed. See [binary license](BINARY-LICENSE.md), [component notices](THIRD-PARTY-NOTICES.md), [component license texts](THIRD-PARTY-LICENSES.txt) and [checksums](SHA256SUMS.txt).
