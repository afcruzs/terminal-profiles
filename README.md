## My profiles for the new [Microsoft Terminal](https://devblogs.microsoft.com/commandline/windows-terminal-microsoft-store-preview-release/)

Besides the automatically generated cmd, ps and ubuntu I have added:

- Git bash
- Anaconda

Quick script to copy `profiles.json` from this repo to the location in your machine:

`Copy-Item profiles.json (Join-Path (Get-ChildItem -Path $env:userprofile\AppData\Local\Packages -Filter "Microsoft.WindowsTerminal*" -Directory).Fullname "RoamingState") -Force`