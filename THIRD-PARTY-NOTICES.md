# Third-party components

Alzirr includes components under their original licenses. Application source licensing does not replace these licenses.

- AndroidX Core, Activity, WebKit, Room, WorkManager and Lifecycle: [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), Android Open Source Project contributors. Exact pinned versions are recorded in the private Android build manifest.
- Kotlin libraries: [Apache License 2.0](https://github.com/JetBrains/kotlin/blob/master/license/LICENSE.txt), JetBrains and contributors.
- Preact, bundled web runtime: [MIT](https://github.com/preactjs/preact/blob/main/LICENSE), Preact contributors.
- Alzirr Extension SDK dependencies Ajv and Zod: their respective [Ajv MIT](https://github.com/ajv-validator/ajv/blob/master/LICENSE) and [Zod MIT](https://github.com/colinhacks/zod/blob/main/LICENSE) licenses.

The APK uses system fonts and bundles its own UI; it does not require a remote font download. Build tools are not included as executable APK components. The SDK’s MIT license is distributed with its package. Dependency/license inventories should be regenerated for each later release.
