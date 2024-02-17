# Godot Engine BaseApp

This is a base application that can be used in other Flatpak manifests to package
Godot projects as Flatpaks. This repository does not contain Godot's editor functionality.
To install the Godot editor as a Flatpak, see [flathub/org.godotengine.godot](https://github.com/flathub/org.godotengine.godot)
instead.

This repository contains several branches (one per minor Godot version,
following the `branch/<major.minor>` naming convention). To avoid
compatibility issues, you should use the same branch as the one that was used to
originally export the project.

Variant based on updated runtime have the `-`version suffix. For example `3.5-23.08` is Godot
3.5 for Freedesktop SDK 23.08.

## How to use

Install the the `.pck` as `/app/bin/godot-runner.pck`. Alternatively
you can create a wrapper script to call `godot-runner` with `--main-pack.

You shoudln't be installing the binary that godot exorted.  This allow
the flatpak to run on the two supported platforms, ie both x86_64 and
aarch64 at the time of writing.

## Limitations

- No C#/Mono support ([flathub/org.godotengine.Godot#8](https://github.com/flathub/org.godotengine.Godot/issues/8)).
