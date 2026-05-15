# kindle_Capture

Standalone Windows executable that walks through every page of a Kindle
for PC book and screenshots each one.

For personal use only — books you own. Don't redistribute the captures;
Kindle DRM exists for a reason.

**Latest release: [v0.0.1](https://github.com/MasakatsuFunaki/kindle_Capture/releases/tag/v0.0.1)** —
all releases under [tags](https://github.com/MasakatsuFunaki/kindle_Capture/tags).

## Files

| File | What it does |
|---|---|
| `capture.exe`           | Captures every page of the active Kindle window into PNGs |
| `config.json.template`  | Copy to `config.json`, edit `total_pages` to match the book |

## Setup

1. Download the two files into a folder.
2. Copy `config.json.template` to `config.json`. Open the book in
   Kindle for PC, look at the footer (`Page X of N`), and put `N`
   into `config.json` as `total_pages`.

## Run

```powershell
capture.exe                              # capture the current book end-to-end
capture.exe --probe                      # one page only, sanity check
capture.exe --pages 50                   # cap at 50 pages
capture.exe --pages 50 --start 100       # subrange
```

Don't type during a capture run — keystrokes go to Kindle.

## Source

Source code stays local and is not published. This `main` branch ships
only the binaries; each tagged commit is one release.
