# Tabless theme for Windows 11 File Explorer Styler

A theme that recreates the old 21H2-22H2 File Explorer command bar before tabs were added.

**Author**: [SandTechStuff](https://github.com/SandTechStuff)

![Screenshot](screenshot.png)

## Optional mods for additional functionality

![Screenshot](screenshot-classic-nav-bar.png)

To get a more accurate look of the old command bar, you can use File Explorer Styler in combination with the Classic Explorer navigation bar.

1. Install the [Classic Explorer navigation bar](https://windhawk.net/mods/explorer-frame-classic) mod. Set `Explorer Style` to `Classic Navigation bar`.

2. In the File Explorer Styler mod, select the `Tabless` theme.

3. In the File Explorer Styler mod, scroll down to the "Style constants" section and add these:

    `NavigationBarGrid=1`

    `CommandBarGrid=2`

To restore regular Mica instead of MicaAlt on the command bar, you can use the Translucent Windows mod.

1. Install the [Translucent Windows](https://windhawk.net/mods/translucent-windows) mod.
<!-- 2. Disable "Immersive darkmode titlebar" -->
<!-- Current version of the mod in the repo does not have this option -->
2. Scroll down to "Process Rules".
3. In the "Process" box, type `explorer.exe`.
4. In the "Effects" dropdown, select `Mica`.

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
styleConstants:
  - NavigationBarGrid=2
  - CommandBarGrid=1
controlStyles:
  - target: Microsoft.UI.Xaml.Controls.Grid#CommandBarControlRootGrid
    styles:
      - Background=Transparent
  - target: Microsoft.UI.Xaml.Controls.Grid#ContentRoot
    styles:
      - Background=Transparent
  - target: FileExplorerExtensions.NavigationBarControl
    styles:
      - Grid.Row=$NavigationBarGrid
  - target: FileExplorerExtensions.CommandBarControl
    styles:
      - Grid.Row=$CommandBarGrid
  - target: Microsoft.UI.Xaml.Controls.Grid#TabContainerGrid > Border
    styles:
      - Visibility=Collapsed
  - target: Microsoft.UI.Xaml.Controls.Grid#TabContainer > Microsoft.UI.Xaml.Controls.Button#CloseButton
    styles:
      - Visibility=Collapsed
  - target: Microsoft.UI.Xaml.Controls.TabViewItem > Microsoft.UI.Xaml.Controls.Grid#LayoutRoot > Microsoft.UI.Xaml.Controls.Canvas
    styles:
      - Opacity=0
  - target: Grid#NavigationBarControlGrid
    styles:
      - Background:=<SolidColorBrush Color="{ThemeResource SystemChromeLowColor}" />
  - target: Microsoft.UI.Xaml.Controls.Grid#TabContainer
    styles:
      - BorderThickness=0
  - target: Microsoft.UI.Xaml.Controls.ContentPresenter > Microsoft.UI.Xaml.Controls.StackPanel > Microsoft.UI.Xaml.Controls.TextBlock
    styles:
      - FontFamily=Segoe UI, Segoe Fluent Icons
      - FontWeight=Normal
  - target: Microsoft.UI.Xaml.Controls.Grid#CommandBarControlRootGrid
    styles:
      - BorderThickness=0,0,0,1
  - target: FileExplorerExtensions.FileExplorerTabControl
    styles:
      - Height=36
  - target: Microsoft.UI.Xaml.Controls.Grid#TabContainer
    styles:
      - Padding=1,0,0,1
  - target: Microsoft.UI.Xaml.Controls.Viewbox#IconBox
    styles:
      - Margin=0,0,4,0
  - target: Microsoft.UI.Xaml.Controls.TabViewItem
    styles:
      - Margin=0,-8,0,0
```
</details>
