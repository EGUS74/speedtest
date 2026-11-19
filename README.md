# Speedtest

A small Python project that measures your internet download and upload speed using [`speedtest-cli`](https://pypi.org/project/speedtest-cli/).

It has two parts:

1. **Command-line version** (`main.py`, `main.ipynb`): runs a test and prints the speeds.
2. **Desktop app** (`app.ipynb`, in progress): a window built with [customtkinter](https://github.com/TomSchimansky/CustomTkinter) where you click a button to run the test and see the speeds.

## Setup

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install customtkinter speedtest-cli
```

On macOS with Homebrew Python, the desktop app also needs Tk:

```bash
brew install python-tk@3.15
```

## Usage

Command-line version:

```bash
python main.py
```

Example output:

```
Download Speed: 94.52 Mbps
Upload Speed: 21.37 Mbps
```

Desktop app: open `app.ipynb` in Jupyter/VS Code and run the cells.

## Roadmap

- [x] Open an empty window
- [ ] Add a "Test speed" button
- [ ] Run the speed test when the button is clicked
- [ ] Show download and upload speeds in the window
- [ ] Run the test in a background thread so the window doesn't freeze

## Files

- `main.py`: command-line script
- `main.ipynb`: notebook version of the script
- `app.ipynb`: desktop UI (work in progress)
