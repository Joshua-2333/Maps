# Maps

A simple Python automation script that opens an address in **OpenStreetMap** using either a command-line argument or the contents of your clipboard.

## Features

* Accepts an address from the command line.
* Falls back to the clipboard if no address is provided.
* Opens the address directly in your default web browser using OpenStreetMap.

## Requirements

* Python 3
* `pyperclip`

Install the required package:

```bash
pip install pyperclip
```

## Usage

### Search using a command-line argument

```bash
python showmap.py 1600 Pennsylvania Ave Washington DC
```

### Search using the clipboard

1. Copy an address to your clipboard.
2. Run:

```bash
python showmap.py
```

The script will automatically open your default web browser and search for the copied address on OpenStreetMap.

## Example

Input:

```text
777 Valencia St, San Francisco, CA 94110
```

The script opens:

```text
https://www.openstreetmap.org/search?query=777 Valencia St, San Francisco, CA 94110
```

## Project Structure

```text
Maps/
├── showmap.py
├── .gitignore
└── README.md
```

## Technologies Used

* Python
* `webbrowser`
* `sys`
* `pyperclip`

## Learning Objectives

This project demonstrates:

* Importing Python modules
* Reading command-line arguments with `sys.argv`
* Reading clipboard contents with `pyperclip`
* Opening web pages with `webbrowser`
* Basic conditional logic (`if` / `else`)
* Simple string manipulation
