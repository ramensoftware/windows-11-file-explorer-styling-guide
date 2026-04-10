# AddressSearchOnly theme for Windows 11 File Explorer Styler

A minimal theme displaying only the address bar and search box for the Windows 11 File Explorer Styler mod.

**Author**: [navandstokes](https://github.com/navandstokes)

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
* Go to the "Advanced" tab.
* Copy the content below to the text box under "Mod settings" and click "Save".

<details>
<summary>Content to import (click to expand)</summary>

```yaml
controlStyles:
  - target: FileExplorerExtensions.NavigationBarControl
    styles:
      - Grid.Row=0
      - Background=Transparent
      - MinHeight=48
      - Margin=0,26,0,1
  - target: Grid#NavigationBarControlGrid
    styles:
      - Background=Transparent
  - target: FileExplorerExtensions.FileExplorerTabControl
    styles:
      - Visibility=Collapsed
  - target: AppBarButton#refreshButton
    styles:
      - Visibility=Collapsed
  - target: AppBarButton#upButton
    styles:
      - Visibility=Collapsed
  - target: AppBarButton#backButton
    styles:
      - Visibility=Collapsed
  - target: AppBarButton#forwardButton
    styles:
      - Visibility=Collapsed
explorerFrameContainerHeight: 80
```
</details>
