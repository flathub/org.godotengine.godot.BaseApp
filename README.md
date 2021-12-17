# Godot Engine BaseApp

This is a base application that can be used in other Flatpak manifests to package
Godot projects as Flatpaks. This repository does not contain Godot's editor functionality.
To install the Godot editor as a Flatpak, see [flathub/org.godotengine.godot](https://github.com/flathub/org.godotengine.godot)
instead.

This repository contains several branches (one per minor Godot version,
following the `branch/<major.minor>` naming convention). To avoid
compatibility issues, you should use the same branch as the one that was used to
originally export the project.

## Limitations

- No C#/Mono support ([flathub/org.godotengine.Godot#8](https://github.com/flathub/org.godotengine.Godot/issues/8)).
