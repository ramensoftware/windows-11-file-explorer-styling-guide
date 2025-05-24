# PreTabs theme for Windows 11 File Explorer Styler

A theme that recreates the old 21H2-22H2 File Explorer command bar.

**Author**: [SandTechStuff](https://github.com/SandTechStuff)

![Screenshot](screenshot.png)

## Theme selection

The theme is integrated into the mod, and can be simply selected from the mod's
settings:

* Open the Windows 11 File Explorer Styler mod in Windhawk.
* Go to the "Settings" tab.
* Select the theme and save the settings.

## Optional mods for additional functionality

To get a more accurate look to the old command bar, you can use File Explorer Styler in combination with Classic Explorer navigation bar.

1. Install the [Classic Explorer navigation bar](https://windhawk.net/mods/explorer-frame-classic) mod. Set `Explorer Style` to `Classic Navigation bar`.

2. In the File Explorer Styler mod, Select the `PreTabs` theme.

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

## Manual installation

The theme styles can also be imported manually. To do that, follow these steps:

* Open the Windows 11 File Explorer Styler mod in Windhawk.
* Go to the "Advanced" tab.
* Copy the content below to the text box under "Mod settings" and click "Save".

<details>
<summary>Content to import (click to expand)</summary>

```json
{
	"controlStyles[0].target": "Microsoft.UI.Xaml.Controls.Grid#CommandBarControlRootGrid",
	"controlStyles[0].styles[0]": "Background=Transparent",
	"controlStyles[1].target": "Microsoft.UI.Xaml.Controls.Grid#ContentRoot",
	"controlStyles[1].styles[0]": "Background=Transparent",
	"controlStyles[2].target": "FileExplorerExtensions.NavigationBarControl",
	"controlStyles[2].styles[0]": "Grid.Row=$NavigationBarGrid",
	"controlStyles[3].target": "FileExplorerExtensions.CommandBarControl",
	"controlStyles[3].styles[0]": "Grid.Row=$CommandBarGrid",
	"controlStyles[4].target": "Microsoft.UI.Xaml.Controls.Grid#TabContainerGrid > Border",
	"controlStyles[4].styles[0]": "Visibility=Collapsed",
	"controlStyles[5].target": "Microsoft.UI.Xaml.Controls.Grid#TabContainer > Microsoft.UI.Xaml.Controls.Button#CloseButton",
	"controlStyles[5].styles[0]": "Visibility=Collapsed",
	"controlStyles[6].target": "Microsoft.UI.Xaml.Controls.TabViewItem > Microsoft.UI.Xaml.Controls.Grid#LayoutRoot > Microsoft.UI.Xaml.Controls.Canvas",
	"controlStyles[6].styles[0]": "Opacity=0",
	"controlStyles[7].target": "Grid#NavigationBarControlGrid",
	"controlStyles[7].styles[0]": "Background:=<SolidColorBrush Color=\"{ThemeResource SystemChromeLowColor}\" />",
	"controlStyles[8].target": "Microsoft.UI.Xaml.Controls.Grid#TabContainer",
	"controlStyles[8].styles[0]": "BorderThickness=0",
	"controlStyles[9].target": "Microsoft.UI.Xaml.Controls.ContentPresenter > Microsoft.UI.Xaml.Controls.StackPanel > Microsoft.UI.Xaml.Controls.TextBlock",
	"controlStyles[9].styles[0]": "FontFamily=Segoe UI, Segoe Fluent Icons",
	"controlStyles[9].styles[1]": "FontWeight=Normal",
	"controlStyles[10].target": "Microsoft.UI.Xaml.Controls.Grid#CommandBarControlRootGrid",
	"controlStyles[10].styles[0]": "BorderThickness=0,0,0,1",
	"controlStyles[11].target": "FileExplorerExtensions.FileExplorerTabControl",
	"controlStyles[11].styles[0]": "Height=36",
	"controlStyles[12].target": "Microsoft.UI.Xaml.Controls.Grid#TabContainer",
	"controlStyles[12].styles[0]": "Padding=1,0,0,1",
	"controlStyles[13].target": "Microsoft.UI.Xaml.Controls.Viewbox#IconBox",
	"controlStyles[13].styles[0]": "Margin=0,0,4,0",
	"controlStyles[14].target": "Microsoft.UI.Xaml.Controls.TabViewItem",
	"controlStyles[14].styles[0]": "Margin=0,-8,0,0",
	"styleConstants[0]": "NavigationBarGrid=2",
	"styleConstants[1]": "CommandBarGrid=1",
	"explorerFrameContainerHeight": 0
}
```
