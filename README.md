## My profiles for the new [Microsoft Terminal](https://devblogs.microsoft.com/commandline/windows-terminal-microsoft-store-preview-release/)

Besides the automatically generated cmd, ps and ubuntu I have added:

- [Git bash](https://github.com/afcruzs/terminal-profiles/blob/7f1619f5f4618211064ed2d64de9f04cdfa7e207/profiles.json#L241)
- [Anaconda 3 prompt](https://github.com/afcruzs/terminal-profiles/blob/7f1619f5f4618211064ed2d64de9f04cdfa7e207/profiles.json#L259)
- [Developer command prompt for VS 2017](https://github.com/afcruzs/terminal-profiles/blob/e9dd6aec28e2692c8c710bbaf3972e86da1d4b4a/profiles.json#L277): this is achieved with a workaround proposed [here](https://github.com/microsoft/terminal/issues/1447#issuecomment-504839617) around the parsing of these commands.

Quick PS script to copy `profiles.json` from this repo to the location in your machine:

`Copy-Item profiles.json (Join-Path (Get-ChildItem -Path $env:userprofile\AppData\Local\Packages -Filter "Microsoft.WindowsTerminal*" -Directory).Fullname "RoamingState") -Force`
