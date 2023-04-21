# Section Dropper

Is a windows dropper designed to operate on memory based execution rather than disk driven execution which can avoid being flagged as malicious from  static analysis by the windows defender. We have used here a .exe file type as dropper format and used a section in the PE file named .rsrc wherein we have stored the payload. 

Keep in mind the payload size need to the very tiny one (approx: 344 B) named favicon.ico is payload here. You can use multiple variety of payload and play around your circumstances from [here](https://github.com/rapid7/metasploit-framework/tree/master/modules/payloads/singles/windows/x64) or design your own custom payload.

## Table of Contents

- Installation
- Usage
- Reference
- Demo

## Requirements

1. Python 3.x
2. Any C++ x64 compiler

## Installation

1. Clone the repository
2. Compile the `compile.bat` file 
3. Run the generated dropper exe file and track the process with PHBear and Process hacker

## Usage

This project can definitely help you in widen the knowledge of malware development and their working on the windows environment. 

## Demo
Video Demo : https://vimeo.com/manage/videos/819970794

## References

- Inspired from Sektor7 Malware Development Essentials
- Supporting Website
    - [https://learn.microsoft.com/en-us/windows/win32/api/memoryapi/nf-memoryapi-virtualalloc](https://learn.microsoft.com/en-us/windows/win32/api/memoryapi/nf-memoryapi-virtualalloc)
    - [https://learn.microsoft.com/en-us/windows/win32/api/memoryapi/nf-memoryapi-writeprocessmemory](https://learn.microsoft.com/en-us/windows/win32/api/memoryapi/nf-memoryapi-writeprocessmemory)
    - [https://learn.microsoft.com/en-us/windows/win32/api/processthreadsapi/nf-processthreadsapi-createremotethread](https://learn.microsoft.com/en-us/windows/win32/api/processthreadsapi/nf-processthreadsapi-createremotethread)
    - [https://github.com/rapid7/metasploit-framework/tree/master/modules/payloads/singles/windows/x64](https://github.com/rapid7/metasploit-framework/tree/master/modules/payloads/singles/windows/x64)
    - [https://github.com/corkami/pics/blob/master/binary/pe101/README.md](https://github.com/corkami/pics/blob/master/binary/pe101/README.md)

## Disclaimer

Strictly for education purpose only be open to experiment in your own environment
