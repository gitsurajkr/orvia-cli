<div align="center">

# orvia

**Orvia rooms, right in your terminal.**

Talk to anyone, then disappear. No account, no sign-up.
Messages are end-to-end encrypted, and rooms vanish when everyone leaves.

[orvia.live](https://orvia.live) · [Download a release](https://github.com/gitsurajkr/orvia-cli/releases/latest)

</div>

---

## Install

**macOS / Linux**

```sh
curl -fsSL https://orvia.live/install.sh | sh
```

**Windows (PowerShell)**

```powershell
irm https://orvia.live/install.ps1 | iex
```

No admin rights needed. The installer picks the right build for your machine,
checks its SHA-256 fingerprint, and refuses to install anything that doesn't match.

## Start

```sh
orvia
```

Pick a name, then **create a room** or **join one** with a code or link.
Share the code, and anyone can join from their terminal **or their browser**
at [orvia.live](https://orvia.live). Same rooms, same encryption.

```sh
orvia create              # start a room, you're the admin
orvia join AB12CD         # join with a code or link
orvia update              # get the latest version
```

## In a room

Messages are numbered, so you act on them by number. Type `/help` any time.

| You want to… | Type |
| --- | --- |
| Send a message | just type and press Enter |
| Reply | `/r thanks!` or `/reply 3 yes` |
| Edit or delete yours | `/edit 3 new text` · `/delete 3` |
| React | `/react 3 like` (love, laugh, fire, party…) |
| Share a file | `/send ~/photo.jpg` |
| Download a file | `/get 5` |
| See who's here | `/users` |
| Leave | `/quit` · `Ctrl+C` closes orvia |

**Room admins and moderators** can also `/approve`, `/deny`, `/kick` and `/mod` people.
Nobody gets in without the admin's approval.

## Privacy, honestly

- **Messages are end-to-end encrypted.** The server relays them but can't read them.
  Use `/fingerprint` to compare keys with someone over another channel.
- **Files are not end-to-end encrypted** (same as on the web) and are deleted after about 5 minutes.
- **No account, nothing to sign up for.** Your display name is stored only on your own computer.
- **Voice and video** live in the browser at [orvia.live](https://orvia.live).

## Updating

orvia checks for a new version once a day and tells you. It never updates itself
without asking. When you're ready:

```sh
orvia update
```

Set `ORVIA_NO_UPDATE_CHECK=1` to turn the check off.

## Supported systems

| | Intel / AMD | ARM |
| --- | --- | --- |
| **Windows** | ✓ | ✓ |
| **macOS** | ✓ | ✓ (Apple silicon) |
| **Linux** | ✓ | ✓ |

---

<div align="center">

This repository only hosts the downloadable builds.
Questions or problems? Visit [orvia.live](https://orvia.live).

</div>
