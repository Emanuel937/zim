# AutoCompiler Script - zim

**Author: Emanuel Abizimi**

## Description

`ZIM` is a Bash script designed to monitor changes to a specific file and automatically restart the compilation or execution process using the specified compiler or interpreter. This tool is useful for developers working in languages like PHP, Python, or others, where source files need to be frequently reloaded.

---

## Features

- Continuous monitoring of changes to a given file.
- Automatic restart of the process when the file is updated.
- Supports any compiler or interpreter (e.g., PHP, Python, etc.).
- Error handling in case of non-existent files or incorrect arguments.

---

## Prerequisites

- Linux or macOS operating system with Bash.
- Access to an interpreter or compiler for the target language (e.g., PHP 8, Python 3, etc.).

---

## Installation

1. Download the script and ensure it is executable:
   ```bash
   chmod +x zim
