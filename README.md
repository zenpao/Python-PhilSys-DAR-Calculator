# Python-PhilSys-DAR-Calculator

A command-line calculator for tallying PhilSys registration Daily Accomplishment Report (DAR) figures — RKO (Registration Kiosk Officer) counts, age group breakdowns, and biometric exemptions — with running totals for Step 2 registration.

**A ready-to-use executable is available in [`/dist`](./dist) — no Python installation required.**

## Features

- **RKO entries:** add per-RKO counts for Assisted Step 1, Online, Walk-In registrants (and their institutional equivalents), with an auto-computed total per entry
- **Age Group entries:** add counts for ages 5–14, 15–59, and 60+, with an auto-computed total
- **Biometric Exemption entries:** add fingerprint and iris exemption counts across the same three age brackets, with an auto-computed total
- **View table:** displays all RKO, age group, and biometric exemption entries in table form, along with the running grand total for each category
- **Delete an RKO entry** by its entry number
- All counts are zero-padded to 4 digits for consistent display

## Tech Stack

- **Python 3** (standard library only — no external dependencies)

## Prerequisites

- Python 3 (only needed if running from source — the packaged executable in `/dist` requires no Python installation)

## Installation

Clone the repository:

```bash
git clone https://github.com/paoradox/Python-PhilSys-DAR-Calculator.git
cd Python-PhilSys-DAR-Calculator
```

No dependencies to install — the script only uses Python's standard library.

## Usage

### Option 1: Run from source

```bash
python darcalculator.py
```

You'll see a menu:

```
a. Check table
b. Add a RKO
c. Add Total Age Group
d. Add Total Biometric Exemption
e. Delete RKO Output
f. Exit
```

Enter a letter to choose an action, and follow the prompts to enter the relevant counts. Choose `a` at any time to view the current table and running totals.

### Option 2: Run the packaged executable

A pre-built Windows executable, `darcalculator.exe`, is available in [`/dist`](./dist) — run it directly, no Python installation required.

## Project Structure

```
Python-PhilSys-DAR-Calculator/
├── dist/
│   └── darcalculator.exe   # Packaged executable
├── build/
│   └── darcalculator/      # PyInstaller build artifacts
├── darcalculator.py        # Main script
├── darcalculator.spec      # PyInstaller build spec
└── ico.ico                 # App icon
```

## License

Not specified.
