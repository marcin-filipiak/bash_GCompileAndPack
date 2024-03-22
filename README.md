# GCompileAndPack

## Overview
GCompileAndPack is a shell script designed to automate the process of compiling C++ code and packaging it into a Debian (.deb) package. It simplifies the tasks of compilation, execution, and package creation into a single script.

## Prerequisites
- GNU Compiler Collection (g++)
- dpkg-deb

## Usage
1. Ensure that your C++ source file is located in the `src/` directory and named according to the convention specified in the `control` file.
2. Run the script using the following command:
    ```bash
    ./GCompileAndPack.sh
    ```
3. Follow the on-screen prompts to compile and execute the program.
4. Optionally, create a Debian package (.deb) by responding to the prompt.

## Features
- Automated compilation of C++ source code.
- Execution of the compiled program.
- Optional creation of a Debian package (.deb) for distribution.

## Script Structure
1. **Initialization**: Sets up necessary variables and clears the terminal.
2. **Compilation**: Compiles the C++ source code using g++.
3. **Execution**: Executes the compiled program.
4. **Debian Package Creation**: Prompts the user to create a .deb package and, if chosen, generates the package using dpkg-deb.

## Example Usage
```bash
./GCompileAndPack.sh
```
## Notes

This script assumes that the necessary files and directories (e.g., src/, control) are present in the directory structure.
Ensure that the permissions for the script are set to allow execution (chmod +x GCompileAndPack).
