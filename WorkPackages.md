# Work Packages
The following will install the standard set of packages that I use at work.

First ensure that chocolatey is installed:
```sh
@powershell -NoProfile -ExecutionPolicy Bypass -Command "iex ((new-object net.webclient).DownloadString('https://chocolatey.org/install.ps1'))" && SET PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin
```

Next run the following to install packages
```sh
cinst awscli ConEmu GoogleChrome greenshot HipChat lastpass linqpad notepadplusplus windirstat -y
cinst git -params '"/GitAndUnixToolsOnPath /NoAutoCrlf"' -y
cinst poshgit -y
```
