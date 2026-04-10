# MicaBar theme for Windows 11 File Explorer Styler

A simple theme that adds Mica to the command bar in File Explorer.

**Author**: [SandTechStuff](https://github.com/SandTechStuff)

![Screenshot](screenshot.png)

## Theme selection

The theme is integrated into the mod and can be selected directly from the mod's
settings:

* Open the Windows 11 File Explorer Styler mod in Windhawk.
* Go to the "Settings" tab.
* Select the theme and save the settings.

## Manual installation

The theme styles can also be imported manually. To do that, follow these steps:

* Open the Windows 11 File Explorer Styler mod in Windhawk.
* Go to the "Settings" tab and select "Textual mode".
* Copy the content below to the text box and click "Save settings".

<details>
<summary>Content to import (click to expand)</summary>

```yaml
controlStyles:
  - target: Grid#CommandBarControlRootGrid
    styles:
      - Background:=<SolidColorBrush Color="{ThemeResource LayerOnMicaBaseAltFillColorDefault}"/>
      - BorderThickness=0,0,0,1
  - target: CommandBar#FileExplorerCommandBar
    styles:
      - Background=Transparent
```
</details>
