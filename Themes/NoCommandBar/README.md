# NoCommandBar theme for Windows 11 File Explorer Styler

A simple theme that removes the command bar from File Explorer.

**Author**: [SandTechStuff](https://github.com/SandTechStuff)

![Screenshot](screenshot.png)

## Theme selection

The theme is integrated into the mod, and can be simply selected from the mod's
settings:

* Open the Windows 11 File Explorer Styler mod in Windhawk.
* Go to the "Settings" tab.
* Select the theme and save the settings.

## Manual installation

The theme styles can also be imported manually. To do that, follow these steps:

* Open the Windows 11 File Explorer Styler mod in Windhawk.
* Go to the "Advanced" tab.
* Copy the content below to the text box under "Mod settings" and click "Save".

<details>
<summary>Content to import (click to expand)</summary>

```json
{
	"controlStyles[0].target": "FileExplorerExtensions.CommandBarControl",
	"controlStyles[0].styles[0]": "Visibility=Collapsed",
	"controlStyles[1].target": "FileExplorerExtensions.NavigationBarControl",
	"controlStyles[1].styles[0]": "Grid.RowSpan=2",
	"explorerFrameContainerHeight": 87
}
```
