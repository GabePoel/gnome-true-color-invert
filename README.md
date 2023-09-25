# True Color Window Inverter

**This is a fork of JackKenney/true-color-window-invert due to 2+ years of inactivity on the project**

GNOME shell extension for inverting window colors in hue preserving manner. Effectively a manual dark theme for GNOME windows.

Available on the GNOME Extensions website here:

https://extensions.gnome.org/extension/5829/true-color-invert/

## Supported Versions

- Gnome 3.32 (deprecated)
- Gnome 3.36 (deprecated)
- Gnome 3.38 (deprecated)
- Gnome 40
- Gnome 41
- Gnome 42
- Gnome 43
- Gnome 44
- Gnome 45 (Experimental | Untested)

Deprecated versions should work, but will not be supported nor will they recieve any further updates.

## Keyboard Shortcut

`Super + I`

## Debugging

Errors will print out here:
```bash
journalctl -f -o cat /usr/bin/gnome-shell
```

## Contributing

Before submitting pull requests, please run:

```bash
glib-compile-schemas schemas/
```

To recompile the `gschemas`.
This step is not neccesary if the 'build.sh' is used, as it's included in the script

## Building for Release

To make the ZIP for the GNOME Shell Extension website: 

1. `sh build.sh`
2. Tag `main` at that time with a release tag according to the revisions made.
