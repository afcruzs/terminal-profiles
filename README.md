## My profiles for the new [Microsoft Terminal](https://devblogs.microsoft.com/commandline/windows-terminal-microsoft-store-preview-release/)

Besides the automatically generated cmd, ps and ubuntu I have added:

- [Git bash](https://github.com/afcruzs/terminal-profiles/blob/7f1619f5f4618211064ed2d64de9f04cdfa7e207/profiles.json#L241)
- [Anaconda 3 prompt](https://github.com/afcruzs/terminal-profiles/blob/7f1619f5f4618211064ed2d64de9f04cdfa7e207/profiles.json#L259)

Quick PS script to copy `profiles.json` from this repo to the location in your machine:

`Copy-Item profiles.json (Join-Path (Get-ChildItem -Path $env:userprofile\AppData\Local\Packages -Filter "Microsoft.WindowsTerminal*" -Directory).Fullname "RoamingState") -Force`
