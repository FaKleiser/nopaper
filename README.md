# nopaper

No one likes paper documents. 
nopaper helps getting rid of paper documents on Windows, in particular. 
Ever struggled with proprietary PDF scanners?
Then setup nopaper to work for you, leveraging awesome Open Source products to create high quality PDF scans.

Features:

- Scan with [NAPS2](https://www.naps2.com) profiles
- OCR documents
- Compress scanned PDF documents
- Save as [PDF/A](https://en.wikipedia.org/wiki/PDF/A)
- Multipage scans. nopaper automatically appends to existing PDF documents

## Getting Started

nopaper requires NAPS2 and Windows Subsystem for Linux (WSL).

1. Install [NAPS2](https://www.naps2.com) for Windows and make sure that `NAPS2.Console.exe` is on the path.
2. Open NAPS2 and configure a profile called `document.flatbed` that is able to scan a document to your liking.
3. Open a WSL and: `sudo apt install ghostscript poppler-utils`

## Usage

To scan a document, open a WSL shell and execute:

```bash
./nopaper <filename>
```

If `filename` already exists, nopaper will append to the existing file.