# PSQR

A simple PowerShell module for generating QR codes in the terminal.

## Installation

Install from the PowerShell Gallery:

```powershell
Install-Module -Name PSQR
```

## Prerequisites

PSQR requires the `qrencode` utility to be installed on your system.

- **macOS:** `brew install qrencode`
- **Linux:** `sudo apt-get install qrencode`
- **Windows:** `scoop install qrencode` or `choco install qrencode` or `winget install -e --id PedroAlbanese.QREncode`

## Usage

Generate a QR code from text or pipeline input:

```powershell
New-PSQR -Text "Hello, World!"
"https://github.com/jakehildreth" | New-PSQR
```

## Requirements

- PowerShell 5.1 or higher
- qrencode utility (see Prerequisites above)
- Cross-platform compatible (Windows, Linux, macOS)

## Notes

This module uses the industry-standard `qrencode` utility to generate proper QR codes that are scannable by all standard QR code readers. The QR codes are displayed using Unicode block characters directly in the terminal.

## License

Copyright (c) 2026 Jake Hildreth. All rights reserved.
