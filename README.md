# Fancy Clothes

A local preview of a saved **Snug Wrld** storefront snapshot. The page in `site/` is an exported Next.js page with its static assets; this repository does not contain the original Next.js application source or build setup.

The Python helper in `serve.py` uses only the standard library. It serves the saved files locally and handles the exported page's `/_next/image` requests by mapping them to the image files in the snapshot.

## Preview

[Open the GitHub Pages preview](https://masoumeh-ashrafi.github.io/fancy-clothes/)

The preview shows the saved snapshot. It does not connect to a live store or inventory.

## Run locally

Requires Python 3.7 or newer. No packages need to be installed.

### macOS

Double-click `start-mac.command`, or run:

```bash
python3 serve.py
```

### Windows

Double-click `start-windows.bat`, or run:

```bat
python serve.py
```

The helper opens `http://localhost:8080` in your browser. Close the terminal window or press `Ctrl+C` to stop it.

To use another port, pass it as an argument:

```bash
python3 serve.py 3000
```

On Windows, use `python serve.py 3000`.

## Repository contents

- `site/` — exported page and saved static assets
- `serve.py` — local preview server and image request mapping
- `start-mac.command` — macOS launcher
- `start-windows.bat` — Windows launcher

## Credit

The saved page identifies the original storefront as **Snug Wrld**. This repository is a static snapshot with a local preview helper, not the original storefront source code.

Maintained by [Masoumeh Ashrafi](https://github.com/masoumeh-ashrafi).