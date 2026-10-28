# SayQL Community Edition

SayQL is the safe way for people and AI to query any database, even production. The desktop app writes SQL as you type plain English, with the AI you choose, and runs it read-only by default. It works with PostgreSQL, MySQL, SQLite, SQL Server and Azure SQL.

- **Quick mode** writes the SQL as you type; nothing changes in your database unless you confirm it.
- **Agent mode (beta)** investigates harder questions ("why did signups drop last week?") in read-only steps and answers with the queries behind it. It's off until you turn it on per connection, and you choose what the AI may see.
- **MCP** lets Claude, Cursor and other AI apps use your saved connections, read-only, with your never-send columns kept private.
- **Voice input** is transcribed on your computer; audio never leaves it.
- **SayQL for teams** lets your people and your AI query your databases, production included, with rules the AI can't cross and a record of every query, on a server your company runs. Sign in to use the database connections your team shares. Teams set one up with `curl -fsSL https://sayql.dev/install | sh` ([setup guide](https://sayql.dev/docs/teams/#set-up-a-team-server)).

**Free forever, for personal and commercial use.**

This repository hosts SayQL's downloads and automatic updates. The source code is at **[dithzz/sayql](https://github.com/dithzz/sayql)**, open source under the Apache License 2.0.

## Download

Get the latest version from **[Releases](https://github.com/dithzz/sayql-releases/releases/latest)**:

| Platform | File |
| --- | --- |
| macOS (Apple silicon) | `SayQL_x.y.z_aarch64.dmg` |
| macOS (Intel) | `SayQL_x.y.z_x64.dmg` |
| Windows | `SayQL_x.y.z_x64-setup.exe` or `.msi` |
| Linux | `.AppImage`, `.deb` or `.rpm` |

## First launch

Early-access builds aren't code-signed yet, so your computer asks you to confirm the first launch. You only do this once.

- **macOS:** open SayQL and close the warning. Then go to System Settings → Privacy & Security and click **Open Anyway**.
- **Windows:** on "Windows protected your PC", click **More info**, then **Run anyway**.
- **Linux:** make the `.AppImage` executable (`chmod +x`) and run it, or install the `.deb` or `.rpm`. For MCP, use the `.deb` or `.rpm`: the AppImage runs from a new folder each time.

After an update, macOS may ask once whether SayQL can use its saved passwords in your keychain. Click **Always Allow**.

## Updates

SayQL checks for updates when it starts and offers **Update to x.y.z** in the status bar. Every update is signed, and SayQL refuses any update whose signature doesn't match.
