# Sayql Community Edition

Sayql is a desktop database client that writes SQL as you type plain English, with the AI you choose. It works with PostgreSQL, MySQL, SQLite, SQL Server and Azure SQL.

**Free forever, for personal and commercial use.**

This repository hosts Sayql's downloads and automatic updates. It has no source code.

## Download

Get the latest version from **[Releases](https://github.com/dithzz/sayql-releases/releases/latest)**:

| Platform | File |
| --- | --- |
| macOS (Apple silicon) | `Sayql_x.y.z_aarch64.dmg` |
| macOS (Intel) | `Sayql_x.y.z_x64.dmg` |
| Windows | `Sayql_x.y.z_x64-setup.exe` or `.msi` |
| Linux | `.AppImage` or `.deb` |

## First launch

Early-access builds aren't code-signed yet, so your computer asks you to confirm the first launch. You only do this once.

- **macOS:** open Sayql and close the warning. Then go to System Settings → Privacy & Security and click **Open Anyway**.
- **Windows:** on "Windows protected your PC", click **More info**, then **Run anyway**.
- **Linux:** make the `.AppImage` executable (`chmod +x`) and run it, or install the `.deb`.

After an update, macOS may ask once whether Sayql can use its saved passwords in your keychain. Click **Always Allow**.

## Updates

Sayql checks for updates when it starts and offers **Update to x.y.z** in the status bar. Every update is signed, and Sayql refuses any update whose signature doesn't match.
