# AddressSearchOnly theme for Windows 11 File Explorer Styler

A minimal theme displaying only the address bar and search box for the Windows 11 File Explorer Styler mod.

**Author**: [navandstokes](https://github.com/navandstokes)

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
  "controlStyles[0].styles[0]": "Visibility=Collapsed",
  "controlStyles[1].target": "FileExplorerExtensions.NavigationBarControl",
  "controlStyles[1].styles[0]": "Grid.Row=0",
  "controlStyles[1].styles[1]": "Background=Transparent",
  "controlStyles[1].styles[2]": "MinHeight=48",
  "controlStyles[1].styles[3]": "Margin=0,26,0,1",
  "controlStyles[2].target": "Grid#NavigationBarControlGrid",
  "controlStyles[2].styles[0]": "Background=Transparent",
  "controlStyles[3].target": "FileExplorerExtensions.FileExplorerTabControl",
  "controlStyles[3].styles[0]": "Visibility=Collapsed",
  "controlStyles[4].target": "AppBarButton#refreshButton",
  "controlStyles[4].styles[0]": "Visibility=Collapsed",
  "controlStyles[5].target": "AppBarButton#upButton",
  "controlStyles[5].styles[0]": "Visibility=Collapsed",
  "controlStyles[6].target": "AppBarButton#backButton",
  "controlStyles[6].styles[0]": "Visibility=Collapsed",
  "controlStyles[7].target": "AppBarButton#forwardButton",
  "controlStyles[7].styles[0]": "Visibility=Collapsed",
  "explorerFrameContainerHeight": 80
}
```
</details>