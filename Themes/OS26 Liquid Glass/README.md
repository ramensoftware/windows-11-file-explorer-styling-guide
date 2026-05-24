# My Custom Glass Theme

A clean, acrylic/blur style theme for Windows 11 File Explorer.

## Theme selection
The theme is integrated into the mod and can be selected directly from the mod's settings.

## Manual Import
To do that manually, follow these steps:
- Open the Windows 11 File Explorer Styler mod in Windhawk.
- Go to the "Settings" tab and select "Textual mode".
- Copy the content below to the text box and click "Save settings".

<details>
<summary>Content to import (click to expand)</summary>

```yaml
explorerFrameContainerHeight: 0
controlStyles:
  - target: "CommandBar#FileExplorerCommandBar "
    styles:
      - Background=Transparent
      - HorizontalAlignment = 1
  - target: "CommandBar#FileExplorerSecondaryCommandBar"
    styles:
      - Background=Transparent
      - MinHeight=0
  - target: "Grid#TabContainerGrid > Border#LeftBottomBorderLine"
    styles:
      - Visibility=Collapsed
  - target: "Grid#TabContainerGrid > Border#RightBottomBorderLine"
    styles:
      - Visibility=Collapsed
  - target: "TabViewItem"
    styles:
      - Margin=0,0,8,0
  - target: "TabViewItem > Grid#LayoutRoot"
    styles:
      - CornerRadius=12
      - Margin=2,4,0,4
      - Height=27
      - BorderThickness=1
      - BorderBrush:=<LinearGradientBrush StartPoint="0,0" EndPoint="1,1"><GradientStop Color="#80ffffff" Offset="0.0" /><GradientStop Color="{ThemeResource SurfaceStrokeColorDefault}" Offset="0.55" /><GradientStop Color="#80ffffff" Offset="1" /></LinearGradientBrush>
  - target: "TabViewItem > Grid#LayoutRoot > Canvas"
    styles:
      - Visibility=Collapsed
  - target: "TabViewItem > Grid#LayoutRoot > Grid#TabContainer"
    styles:
      - Background = Transparent 
      - BorderThickness = 0
  - target: "TabViewItem > Grid#LayoutRoot@CommonStates"
    styles:
      - Background@Selected:=<WindhawkBlur BlurAmount="15" TintColor="#25ffffff" />
      - Background@PointerOverSelected:=<WindhawkBlur BlurAmount="15" TintColor="#35ffffff" />
      - Background@Normal:=<WindhawkBlur BlurAmount="15" TintColor="#15ffffff" />
  - target: "Grid#TabContainerGrid > Border > Button#AddButton"
    styles:
      - Visibility = 0
      - Margin = 0,0,0,3
  - target: "Grid#CommandBarControlRootGrid"
    styles:
      - Background=Transparent 
  - target: "Grid#NavigationBarControlGrid"
    styles:
      - Background=Transparent 
  - target: "Grid#PART_LayoutRoot"
    styles:
      - Background :=<WindhawkBlur BlurAmount="15" TintColor="#25ffffff" />
      - CornerRadius = 14
      - BorderThickness = 1
      - BorderBrush:=<LinearGradientBrush StartPoint="0,0" EndPoint="1,1"><GradientStop Color="#80ffffff" Offset="0.0" /><GradientStop Color="{ThemeResource SurfaceStrokeColorDefault}" Offset="0.55" /><GradientStop Color="#80ffffff" Offset="1" /></LinearGradientBrush>
  - target: "FileExplorerExtensions.CommandBarControl"
    styles:
      - Margin = 0,0,0,0
  - target: "AutoSuggestBox#FileExplorerSearchBox > Grid#LayoutRoot > TextBox > Grid@CommonStates > Border#BorderElement"
    styles:
      - Background :=<WindhawkBlur BlurAmount="15" TintColor="#25ffffff" />
      - CornerRadius = 14
      - BorderThickness = 1
      - BorderBrush:=<LinearGradientBrush StartPoint="0,0" EndPoint="1,1"><GradientStop Color="#80ffffff" Offset="0.0" /><GradientStop Color="{ThemeResource SurfaceStrokeColorDefault}" Offset="0.55" /><GradientStop Color="#80ffffff" Offset="1" /></LinearGradientBrush>
  - target: "Microsoft.UI.Xaml.Controls.AppBarButton"
    styles:
      - Background :=<WindhawkBlur BlurAmount="15" TintColor="#25ffffff" />
      - CornerRadius = 12
      - BorderThickness = 1
      - Margin = 3,0,3,1
      - BorderBrush:=<LinearGradientBrush StartPoint="0,0" EndPoint="1,1"><GradientStop Color="#80ffffff" Offset="0.0" /><GradientStop Color="{ThemeResource SurfaceStrokeColorDefault}" Offset="0.55" /><GradientStop Color="#80ffffff" Offset="1" /></LinearGradientBrush>
  - target: "Microsoft.UI.Xaml.Controls.AppBarToggleButton"
    styles:
      - Background :=<WindhawkBlur BlurAmount="15" TintColor="#25ffffff" />
      - CornerRadius = 12
      - BorderThickness = 1
      - Margin = 3,0,3,1
      - BorderBrush:=<LinearGradientBrush StartPoint="0,0" EndPoint="1,1"><GradientStop Color="#80ffffff" Offset="0.0" /><GradientStop Color="{ThemeResource SurfaceStrokeColorDefault}" Offset="0.55" /><GradientStop Color="#80ffffff" Offset="1" /></LinearGradientBrush>
  - target: "Button#MoreButton"
    styles:
      - Visibility=Collapsed
  - target: "Microsoft.UI.Xaml.Controls.AppBarSeparator"
    styles:
      - Visibility = Collapsed
  - target: "Microsoft.UI.Xaml.Controls.AppBarButton#backButton"
    styles:
      - Margin = 0,9,9,0
  - target: "Microsoft.UI.Xaml.Controls.AppBarButton#forwardButton"
    styles:
      - Margin = 0,9,9,0
  - target: "Microsoft.UI.Xaml.Controls.AppBarButton#upButton"
    styles:
      - Margin = 0,9,9,0
  - target: "Microsoft.UI.Xaml.Controls.AppBarButton#refreshButton"
    styles:
      - Margin = 0,9,9,0
