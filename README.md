# ATM Simulation (C++)

[![CI](https://github.com/subhanbhatti50134-jpg/ATM-Stimulation/actions/workflows/ci.yml/badge.svg)](https://github.com/subhanbhatti50134-jpg/ATM-Stimulation/actions/workflows/ci.yml)

![Project banner for ATM Simulation](docs/images/atm-stimulation-banner.png)

A beginner C++ console project that simulates an ATM: PIN-protected login,
balance inquiry, cash deposits, and withdrawals, built with OOP principles.

## What it does

- PIN-protected login (example PIN: `1234`)
- Check current balance
- Deposit money (validates positive amounts)
- Withdraw money (validates sufficient funds and positive amounts)
- Logout
- Console menu to drive the session

## Who it's for

Students learning C++ classes, encapsulation, input validation, and menu-driven
console applications.

## Features

- `ATM` class: balance, PIN, authentication state; `deposit()`, `withdraw()`,
  `checkBalance()`, `authenticate()`
- `ATMController` class: menu loop, screen clearing, input handling
- Input validation: rejects non-positive and over-balance withdrawals
- Authentication guard: balance and transactions require a successful login

## Compile and run

Prerequisites: a C++ compiler (e.g. `g++`).

```bash
# clone
git clone https://github.com/subhanbhatti50134-jpg/ATM-Stimulation.git
cd ATM-Stimulation

# compile
g++ "ATM Stimulation.cpp" -o atm_simulation

# run
./atm_simulation
```

Windows (PowerShell):

```powershell
g++ "ATM Stimulation.cpp" -o atm_simulation.exe
.\atm_simulation.exe
```

> The example PIN is hardcoded as `1234` for demonstration purposes. Change it
> (and add real authentication) before using this for anything beyond a
> learning exercise.

## Notes

- This is a learning project: state is in memory only (resets on exit), and the
  PIN is hardcoded. No database, file storage, or real banking integration.
- The file `Code` in this repository appears to be an alternate/duplicate export
  of the same program; `ATM Stimulation.cpp` is the primary source.
- Compilation was not tested in this environment; the GitHub Actions workflow
  verifies it builds with `g++`.

## License

This repository does not yet carry an open-source license. See
`LICENSE_DECISION.md` for recommended options.
