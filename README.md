# Daily Expenses Android app

This project wraps the supplied `Daily expenses.html` app in a lightweight Android WebView app. The current version includes adding, editing, and deleting expenses; daily budget tracking; weekly/monthly summaries; and manual JSON backup/restore. Expense entries and settings use local storage inside the app and are intended to stay on this device.

## Build an APK without installing Android Studio locally

1. Create a new GitHub repository.
2. Extract this ZIP and upload all files/folders to the repository root. Commit to the `main` branch.
3. Open the repository on GitHub → **Actions** → **Build Daily Expenses APK** → **Run workflow** (or wait for the push-triggered build).
4. When the workflow finishes, open the run and download the `DailyExpenses-debug-apk` artifact.
5. Extract the downloaded artifact ZIP on your phone and install `app-debug.apk`. If Android asks, allow installation from that source.

## Notes

- This is a debug APK for personal use, not a Play Store release.
- The HTML references Google Fonts; it falls back to system fonts if offline.
- Use **Prepare backup** to generate JSON, then copy the text into a safe note/file. To restore, paste the saved JSON into the same box and tap **Restore backup**. Restore replaces current local expenses.
- Data is stored locally in this app's WebView storage. Clearing app data or uninstalling the app may erase saved expenses; keep backups.
- Before relying on it for important records, test adding, editing, deleting, backup/restore, changing budget/currency, and reopening the app.
