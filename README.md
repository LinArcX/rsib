<h4 align="center">
  <img src="https://img.shields.io/github/languages/top/LinArcX/strepl.svg"/>  <img src="https://img.shields.io/github/repo-size/LinArcX/strepl.svg"/>  <img src="https://img.shields.io/github/tag/LinArcX/strepl.svg?colorB=green"/>
</h4>

# strepl
Replace strings in binary files.

# compile
1. First, you should load appropriate environment variables.(that contains the address of `cl.exe`, `linker.exe`, ...).

    To do that you have two options:

    1.1. Via CMD:

        cmd.exe /E:ON /V:ON /k .\msvc2019-64bit.cmd

    1.2. Via PowerShell:

        Invoke-CmdScript "C:\Program Files (x86)\Microsoft Visual Studio\2019\Community\VC\Auxiliary\Build\vcvars64.bat"

2. Change to root directory of the project.
3. `nmake.exe .\Makefile.win`

    It will create __strepl.exe__ in _release_ directory.

# Append strepl.exe to PATH environment variable
`[Environment]::SetEnvironmentVariable("PATH", "$ENV:PATH;D:\workspace\c++\cpp\projects\active\strepl\release", "MACHINE")`

## License
![License](https://img.shields.io/github/license/LinArcX/strepl.svg)
