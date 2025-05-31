# Minimal Explorer11 theme for Windows 11 File Explorer Styler

A minimalistic theme for windows 11 file explorer styler mod.

**Author**: [Undisputed00x](https://github.com/Undisputed00x)

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
  "controlStyles[0].target": "AppBarButton#backButton > Grid#Root@CommonStates > Border#AppBarButtonInnerBorder",
  "controlStyles[0].styles[0]": "Background@Normal:=<AcrylicBrush TintColor=\"Transparent\" Opacity=\"0.07\"/>",
  "controlStyles[0].styles[1]": "Background@PointerOver:=<AcrylicBrush TintColor=\"Transparent\" Opacity=\"0.12\"/>",
  "controlStyles[0].styles[2]": "Background@Pressed:=<AcrylicBrush TintColor=\"Transparent\" Opacity=\"0.12\"/>",
  "controlStyles[0].styles[3]": "Background@Disabled:=<AcrylicBrush TintColor=\"Transparent\" Opacity=\"0.05\"/>",
  "controlStyles[1].target": "AppBarButton#forwardButton > Grid#Root@CommonStates > Border#AppBarButtonInnerBorder",
  "controlStyles[1].styles[0]": "Background@Normal:=<AcrylicBrush TintColor=\"Transparent\" Opacity=\"0.05\"/>",
  "controlStyles[1].styles[1]": "Background@PointerOver:=<AcrylicBrush TintColor=\"Transparent\" Opacity=\"0.12\"/>",
  "controlStyles[1].styles[2]": "Background@Pressed:=<AcrylicBrush TintColor=\"Transparent\" Opacity=\"0.12\"/>",
  "controlStyles[1].styles[3]": "Background@Disabled:=<AcrylicBrush TintColor=\"Transparent\" Opacity=\"0.05\"/>",
  "controlStyles[2].target": "AppBarButton#refreshButton",
  "controlStyles[2].styles[0]": "Visibility=Collapsed",
  "controlStyles[3].target": "AppBarButton#upButton",
  "controlStyles[3].styles[0]": "Visibility=Collapsed",
  "controlStyles[4].target": "Border#BottomBorderLine",
  "controlStyles[4].styles[0]": "Visibility=Collapsed",
  "controlStyles[5].target": "FileExplorerExtensions.CommandBarControl",
  "controlStyles[5].styles[0]": "Visibility=Collapsed",
  "controlStyles[6].target": "FileExplorerExtensions.AddressBarControl > Grid#PART_LayoutRoot > Grid#NormalModeGrid",
  "controlStyles[6].styles[0]": "BorderThickness=0,0,0,1",
  "controlStyles[6].styles[1]": "BorderBrush=#A0A0A0",
  "controlStyles[7].target": "Grid#DetailsViewControlRootGrid",
  "controlStyles[7].styles[0]": "Background=Transparent",
  "controlStyles[8].target": "Grid#TabContainerGrid > Border#LeftBottomBorderLine",
  "controlStyles[8].styles[0]": "Visibility=Collapsed",
  "controlStyles[9].target": "Grid#TabContainerGrid > Border#RightBottomBorderLine",
  "controlStyles[9].styles[0]": "Visibility=Collapsed",
  "controlStyles[10].target": "StackPanel#DetailsViewThumbnail > Grid",
  "controlStyles[10].styles[0]": "Background=Transparent",
  "controlStyles[11].target": "TabViewItem",
  "controlStyles[11].styles[0]": "Margin=0,0,3,0",
  "controlStyles[12].target": "TabViewItem > Grid#LayoutRoot",
  "controlStyles[12].styles[0]": "CornerRadius=4",
  "controlStyles[12].styles[1]": "Margin=0,-3,0,3",
  "controlStyles[12].styles[2]": "Height=28",
  "controlStyles[13].target": "TabViewItem > Grid#LayoutRoot > Canvas",
  "controlStyles[13].styles[0]": "Visibility=Collapsed",
  "controlStyles[14].target": "TabViewItem > Grid#LayoutRoot > Grid#TabContainer",
  "controlStyles[14].styles[0]": "Background=Transparent",
  "controlStyles[14].styles[1]": "BorderBrush=Transparent",
  "controlStyles[15].target": "TabViewItem > Grid#LayoutRoot@CommonStates",
  "controlStyles[15].styles[0]": "Background@Selected:=<SolidColorBrush Color=\"#808080\" Opacity=\"0.35\"/>",
  "controlStyles[15].styles[1]": "Background@PointerOverSelected:=<SolidColorBrush Color=\"#808080\" Opacity=\"0.35\"/>",
  "controlStyles[15].styles[2]": "Background@PointerOver:=<AcrylicBrush TintColor=\"Transparent\" Opacity=\"0.13\"/>",
  "controlStyles[15].styles[3]": "Background@Normal:=<AcrylicBrush TintColor=\"Transparent\" Opacity=\"0.05\"/>",
  "controlStyles[15].styles[4]": "Background@PressedSelected:=<SolidColorBrush Color=\"#808080\" Opacity=\"0.35\"/>",
  "controlStyles[16].target": "Grid#FileExplorerAddressBarGrid",
  "controlStyles[16].styles[0]": "Grid.ColumnSpan=2",
  "controlStyles[16].styles[1]": "Margin=0,0,10,0",
  "controlStyles[17].target": "AutoSuggestBox#FileExplorerSearchBox",
  "controlStyles[17].styles[0]": "Visibility=Collapsed",
  "controlStyles[18].target": "AppBarButton#backButton > Grid#Root",
  "controlStyles[18].styles[0]": "Padding=2",
  "controlStyles[19].target": "AppBarButton#forwardButton > Grid#Root",
  "controlStyles[19].styles[0]": "Padding=2",
  "controlStyles[20].target": "AppBarButton#forwardButton > Grid#Root > Grid#ContentRoot > Viewbox#ContentViewbox",
  "controlStyles[20].styles[0]": "Margin=9",
  "controlStyles[21].target": "AppBarButton#backButton > Grid#Root > Grid#ContentRoot > Viewbox#ContentViewbox",
  "controlStyles[21].styles[0]": "Margin=9",
  "controlStyles[22].target": "Grid#PART_LayoutRoot",
  "controlStyles[22].styles[0]": "MinHeight=28",
  "controlStyles[22].styles[1]": "Height=28",
  "controlStyles[23].target": "Grid#TabContainerGrid > Border > Button#AddButton",
  "controlStyles[23].styles[0]": "Margin=0,0,20,4",
  "controlStyles[24].target": "Border#ScrollIncreaseButtonContainer",
  "controlStyles[24].styles[0]": "Margin=0,0,0,4",
  "controlStyles[25].target": "Border#ScrollDecreaseButtonContainer",
  "controlStyles[25].styles[0]": "Margin=0,0,0,4",
  "controlStyles[26].target": "Grid#FileExplorerAddressBarGrid",
  "controlStyles[26].styles[0]": "Visibility=Collapsed",
  "controlStyles[27].target": "FileExplorerExtensions.NavigationBarControl#NavigationBarControl",
  "controlStyles[27].styles[0]": "Grid.Row=0",
  "controlStyles[27].styles[1]": "Grid.RowSpan=2",
  "controlStyles[28].target": "FileExplorerExtensions.FileExplorerTabControl",
  "controlStyles[28].styles[0]": "Margin=100,0,0,-15",
  "controlStyles[28].styles[1]": "Grid.RowSpan=2",
  "controlStyles[29].target": "FileExplorerExtensions.NavigationBarControl > Grid#NavigationBarControlGrid",
  "controlStyles[29].styles[0]": "Margin=0,0,0,-18",
  "controlStyles[29].styles[1]": "Background=Transparent",
  "controlStyles[29].styles[2]": "Width=100",
  "controlStyles[29].styles[3]": "HorizontalAlignment=0",
  "explorerFrameContainerHeight": 42
}
```
