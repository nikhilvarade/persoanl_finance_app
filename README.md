# Privacy Finance for Android

Privacy Finance is an offline-first personal finance tracker for Android. It helps you review transactions, group eligible bank SMS transactions by account, view spending insights, and import supported bank statements.

> **Testing build:** This project is still being tested. Confirm that the APK installs and opens correctly on your phone before relying on it. Always verify imported transactions against your bank's original records.

## Download

Download the latest APK from the [Releases page](https://github.com/nikhilvarade/persoanl_finance_app/releases/latest).

Only install APKs published in this repository's Releases. The APK must be signed by the project maintainer. Android may show a warning because the APK is installed outside an app store.

## Install on Android

1. Open the latest release on your Android phone and download the `.apk` file.
2. Open the downloaded file from your browser's Downloads list or the Files app.
3. If Android asks, allow that browser or file app to install unknown apps. This setting is specific to the source app and can be turned off again after installation.
4. Return to the installer and tap **Install**.
5. Open Privacy Finance. Allow SMS or notification access only if you want those features.

Settings names vary slightly by Android version and phone manufacturer.

## Features

- Record, search, edit, and review income and expense transactions.
- View spending summaries, category charts, account summaries, and transaction history.
- Import CSV files and selectable-text PDF bank statements. Scanned/image-only PDFs are not supported because OCR is not included.
- Recognize eligible bank SMS alerts after SMS permission is granted and automatic recognition is enabled. The app uses debit/credit cues, an amount, and an account reference to identify candidate transactions.
- Share a selected SMS or email alert to the app for recognition. The app does not sign in to or read email inboxes.
- Export a transaction backup as an Excel `.xlsx` file.

## Privacy and data handling

- The app is designed to process its transaction data on the device and does not declare Android Internet permission in its current manifest.
- SMS recognition is optional and requires Android SMS permissions. The app is intended to save transaction details and a masked account suffix, not the complete SMS text or full account number. Check each recognized transaction in the app.
- The local transaction database is **not encrypted by the app** in this version. Protect your phone with its screen lock.
- Excel backup files are **not encrypted**. Keep exported files in a location you trust and do not share them publicly.
- Email messages are not read automatically. You must share or select message text yourself.

## Important notes

- Bank SMS formats vary. Some alerts may not be recognized, and a recognized description or category may need correction.
- Statement formats vary. Review the import preview before saving transactions.
- If Android reports that an update cannot be installed, the APK may have been signed with a different key from the installed copy. Updates must be signed with the same release key. Do not uninstall an existing copy if you need to preserve its locally stored transactions unless you have first made a backup.
- This app is a personal tracking tool, not a bank service or financial advice. It does not verify transactions with your bank.

## Releases

Each release has a version tag and notes describing its changes. Use the newest compatible release for updates. Keep the app's signing key private; the maintainer will use it to sign future updates.

## Feedback

For a problem, open an issue in this repository and include the app version, Android version, and steps to reproduce it. **Do not post bank SMS text, account numbers, passwords, keystore files, or transaction exports in an issue.**
