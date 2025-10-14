# MicaBar theme for Windows 11 File Explorer Styler

A simple theme that adds Mica to the command bar in File Explorer.

**Author**: [SandTechStuff](https://github.com/SandTechStuff)

![Screenshot](screenshot.png)

## Theme selection

The theme is integrated into the mod and can simply be selected from the mod's
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
	"controlStyles[0].target": "Grid#CommandBarControlRootGrid",
	"controlStyles[0].styles[0]": "Background:=<SolidColorBrush Color=\"{ThemeResource LayerOnMicaBaseAltFillColorDefault}\"/>",
	"controlStyles[0].styles[1]": "BorderThickness=0,0,0,1",
	"controlStyles[1].target": "CommandBar#FileExplorerCommandBar",
	"controlStyles[1].styles[0]": "Background=Transparent",
	"explorerFrameContainerHeight": 0
}
```
</details>
