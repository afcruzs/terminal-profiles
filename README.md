## My profiles for the [Windows Terminal](https://docs.microsoft.com/en-us/windows/terminal/)

![](Capture.JPG)


Besides the automatically generated cmd, ps and ubuntu I have added:

- [Git bash](https://github.com/afcruzs/terminal-profiles/blob/7f1619f5f4618211064ed2d64de9f04cdfa7e207/profiles.json#L241)
- [Anaconda PS 3 prompt](https://github.com/afcruzs/terminal-profiles/blob/7f1619f5f4618211064ed2d64de9f04cdfa7e207/profiles.json#L259)
- [Developer command prompt for VS 2019](https://github.com/afcruzs/terminal-profiles/blob/e9dd6aec28e2692c8c710bbaf3972e86da1d4b4a/profiles.json#L277).

Quick PS script to copy `settings.json` from this repo to the location in your machine:

`Copy-Item settings.json (Join-Path (Get-ChildItem -Path $env:userprofile\AppData\Local\Packages -Filter "Microsoft.WindowsTerminal_*" -Directory).Fullname "LocalState") -Force`
