# FileFlow — Ulauncher Extension
Fast file and folder search for Ulauncher using `plocate`/`locate`, with support for mounted hardware drives and an intelligent "Open With" menu.

## Features
- **Fast Indexed Search:** Uses `plocate` or `locate` for instant results.
- **Hardware Drive Scanning:** Automatically finds files on mounted media (`/run/media`, `/media`, `/mnt`).
- **Dynamic "Open With" Menu:** Intelligently suggests installed applications based on file type.
- **Configurable Search Modes:**
  - **Normal:** Combined indexed and hardware search.
  - **Directory-Only:** `s <dir_keyword> <pattern>`
  - **Hardware-Only:** `s <hw_keyword> <pattern>`
  - **Combined:** `s <hw_keyword> <dir_keyword> <pattern>`
  - **Raw:** `s r <args>` for direct `locate` commands.
- **Customizable Keywords:** Set your own keywords for `dir` and `hw` searches in preferences.

## Usage
- **Default Keyword:** `s`
- **Open File:** `Enter`
- **More Options:** `Alt+Enter` to access "Open With..." and "Open Folder Location".
- **Copy All Paths:** `Ctrl+Enter`

**Note:** Direct drag-and-drop is not supported due to a Ulauncher API limitation.

## Installation
1.  **Install Dependencies:**
    - **Debian/Ubuntu:** `sudo apt install plocate`
    - **Fedora/RHEL:** `sudo dnf install plocate`
    - **Arch Linux:** `sudo pacman -S plocate`
2.  **Update Database:** `sudo updatedb`
3.  **Install Extension:** Add the extension URL in Ulauncher's preferences or copy it to `~/.local/share/ulauncher/extensions/`.

## Configuration
Adjust the following in the extension's preferences:
- **Keyword:** The main activation keyword (default: `s`).
- **Limit:** Maximum number of results.
- **Directory search keyword:** (default: `dir`).
- **Hardware search keyword:** (default: `hw`).

## Acknowledgments
- Based on the original work by [hassanradwannn](https://github.com/hassanradwannn).
- Icons from [Flaticon](https://www.flaticon.com/).
