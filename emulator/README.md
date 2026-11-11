# BVM
## Hackaday Supercon 2022 Badge Virtual Machine

This project aims to provide a vm for the [2022 Hackaday Supercon Badge](https://hackaday.io/project/182568-badge-for-2020-supercon-years-of-lockdown) to aid in programming and debugging. It is not fully tested and is a work-in-progress.

## Installation

Python 3.6 (or greater) is required.

pillow is required: pip install pillow

## Python package

The headless emulator core (`badge`, `bvmCPU`, and `bvmParser`) can be
installed without Tk or Pillow:

```bash
pip install "git+https://github.com/Hack-a-Day/2022-Supercon6-Badge-Tools.git#subdirectory=emulator"
```

The Tk GUI (`bvm.py`) still requires Pillow and a working Tk installation, and
should be run from a source checkout.

## Running

Run the program with `python bvm.py [input.bin]`.

Example: `python bvm.py heart.bin` will launch the BVM, reading a text file called `heart.bin` which is an assembled binary file containing machine code ready to be flashed onto a hardware badge. 

