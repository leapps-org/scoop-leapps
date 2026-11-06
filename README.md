# LEAPPs Scoop Bucket

Scoop manifests for installing LEAPPs tools and LAVA on Windows.

## Need Scoop?

Scoop is a command-line package manager for Windows. It installs apps into your
user profile, keeps command-line tools on your PATH, and can update installed
tools with a single command.

Install Scoop first if you do not already have it: https://scoop.sh

## Add the bucket

```powershell
scoop bucket add leapps https://github.com/leapps-org/scoop-leapps
```

## Install

```powershell
scoop install leapps/aleapp
scoop install leapps/dleapp
scoop install leapps/gleapp
scoop install leapps/ileapp
scoop install leapps/rleapp
scoop install leapps/vleapp
scoop install leapps/lava
```

Each LEAPPs package provides both the command-line tool on your PATH and a Start
Menu shortcut. Open the shortcut or run the tool without arguments to launch its
graphical interface. For ALEAPP, DLEAPP, iLEAPP, RLEAPP, and VLEAPP, pass arguments
to use the command line. GLEAPP's Windows build opens its desktop interface by
default; `gleapp web` opens its browser interface.

GLEAPP is available for Windows x64. The other LEAPPs packages also provide
native Windows ARM64 builds.

## Migrate from the separate GUI packages

The `-gui` packages have been replaced by the combined packages. If you have one
installed, uninstall it and install the corresponding combined package. For example:

```powershell
scoop update
scoop uninstall aleapp-gui
scoop install leapps/aleapp
```

Use the same steps for `ileapp-gui`, `rleapp-gui`, or `vleapp-gui`, replacing
the package names accordingly. If the combined package is already installed,
run `scoop update aleapp` instead of the install command.

## Update

Refresh bucket metadata and update installed LEAPPs tools with:

```powershell
scoop update
scoop update aleapp dleapp gleapp ileapp rleapp vleapp lava
```

To update every installed Scoop app, run:

```powershell
scoop update *
```
