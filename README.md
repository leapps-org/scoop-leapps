# LEAPPs Scoop Bucket

Scoop manifests for installing LEAPPs tools and LAVA on Windows.

## Add the bucket

```powershell
scoop bucket add leapps https://github.com/leapps-org/scoop-leapps
```

## Install

```powershell
scoop install leapps/aleapp
scoop install leapps/aleapp-gui
scoop install leapps/ileapp
scoop install leapps/ileapp-gui
scoop install leapps/rleapp
scoop install leapps/rleapp-gui
scoop install leapps/vleapp
scoop install leapps/vleapp-gui
scoop install leapps/lava
```

The command-line LEAPPs manifests add the CLI binaries to your PATH. The GUI manifests add Start Menu shortcuts.

## Update

Refresh bucket metadata and update installed LEAPPs tools with:

```powershell
scoop update
scoop update aleapp ileapp rleapp vleapp lava
```

To update every installed Scoop app, run:

```powershell
scoop update *
```
