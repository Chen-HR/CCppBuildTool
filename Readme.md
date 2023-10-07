# C/Cpp Build Tool

Tools for C/C++ compilation, construction and testing

## features

- Can automatically identify whether there are changes in the program code (including standard or self-made function libraries) to determine whether it needs to be recompiled
- Configurable compilation parameters
- Compilation is completed and can be executed automatically
- Configurable execution parameters, standard input and output

## Usage

```powershell
CCppTool++.ps1 $Action $FileBasenameNoExtension
CCppTool++.ps1 $Action $FileBasenameNoExtension $Compiler
CCppTool++.ps1 $Action $FileBasenameNoExtension $Compiler $Folder
```

## Execute event

- Pre-Processing
  - Remove previously compiled executable files
- Expand Preprocess
  - Generate to pre-processed files
- Compilation
  - Compile the specified file
- Test
  - Execute the specified file
- Post-Processing
  - Remove the executable file after the test is completed

## Action list

- `preprocess`
  - Expand Preprocess
- `build`
  - Pre-Processing
  - Compilation
- `compile`
  - Compilation
- `test`
  - Compilation
  - Test
- `test-flush`
  - Pre-Processing
  - Compilation
  - Test
  - Post-Processing
