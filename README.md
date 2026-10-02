# Keepwell

Tidy files, nothing lost. Keepwell sorts messy folders (Downloads, Desktop…) by type and your own rules, cleans
junk safely, uninstalls apps with their leftovers, and puts things back from the Trash — with a preview before
anything moves and Undo for every change. It runs entirely on your computer.

## Install

**Mac** — open Terminal (Applications → Utilities) and paste:

```bash
curl -fsSL https://github.com/h-thavy/keepwell/releases/latest/download/install.sh | bash
```

**Windows** — open PowerShell (Start → type “PowerShell”) and paste:

```powershell
irm https://github.com/h-thavy/keepwell/releases/latest/download/install.ps1 | iex
```

That's it: Keepwell installs and opens in your browser. Nothing else to install — it brings its own Python.
Run the same line again any time to update.

<details>
<summary>Prefer downloading by hand?</summary>

Download **Keepwell-macOS.zip** or **Keepwell-Windows.zip** from the
[latest release](https://github.com/h-thavy/keepwell/releases/latest) and follow *How to open Keepwell.txt* inside.
Because Keepwell isn't notarized by Apple, macOS asks once: try to open it, then click **Open Anyway** at the
bottom of System Settings → Privacy & Security. (The one-line installer above avoids this.)
</details>

## Requirements

macOS 11 or newer (Apple Silicon or Intel) · Windows 10 or newer.

## Remove Keepwell

Click **Quit** at the bottom of its sidebar, then delete **Keepwell** from Applications (Mac) or run
`Remove-Item -Recurse "$env:LOCALAPPDATA\Programs\Keepwell"` (Windows). Its settings and history are in
`~/.keepwell` (Mac) or `%USERPROFILE%\.keepwell` (Windows) — delete that folder too to remove everything.
