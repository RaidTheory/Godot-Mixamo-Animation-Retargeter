# Mixamo Animation Retargeter for Godot 4.3

This plugin simplifies the process of importing and retargeting Mixamo animations in Godot 4.x projects.

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/WpSPJ_OKadM/0.jpg)](https://youtu.be/WpSPJ_OKadM)



## Features

- Adds a "Retarget Mixamo Animation" option to the right-click menu for FBX files in the FileSystem dock.
- Automatically sets up the correct import settings for Mixamo animations.
- Supports batch processing of multiple FBX files.
- Saves retargeted animations as separate .res files that can be added to Animation Libraries.

## Installation

1. Download or clone this repository.
2. Copy the `addons/mixamo_animation_retargeter` folder into your Godot project's `addons` folder.
3. Enable the plugin in Project Settings -> Plugins.

## Usage

1. Import your Mixamo FBX file(s) into your Godot project using ufbx.
2. In the FileSystem dock, right-click on the FBX file(s) you want to retarget.
3. Select "Retarget Mixamo Animation" from the context menu.
4. Choose a destination folder for the exported animation(s).
5. The plugin will automatically update the import settings, retarget the animation(s), and save them as .res files in the specified folder.
6. Ensure your character model has a Skeleton3D node named "Skeleton" for the exported animations to work correctly. 
7. Ensure your Character Skeleton is also retargeted using Bone Mapping. This ensures both the animation and the skeleton will share the same bone names.
8. Add the exported .res files to an AnimationLibrary and you should be able to play the animations in your scene.

## Requirements

- Godot 4.3

## Configuration

The plugin uses a predefined bone map for Mixamo animations. If you need to customize the bone mapping, you can modify the `mixamo_bone_map.tres` file in the plugin folder.

## Known Issues

- Untested with older Godot versions.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

GNU GPLv3

## Credits

Developed by Matt Marcin @ RaidTheory

## Disclaimer

This plugin is not affiliated with or endorsed by Mixamo or Adobe. Mixamo and its logo are registered trademarks of Adobe Inc. All rights to Mixamo assets and branding belong to Adobe Inc.
