# OS26 Liquid Glass Explorer

This theme modifies key elements in the Windows 11 File Explorer to achieve a sleek, premium OS26 inspired Liquid Glass aesthetic with stylized elements.
## Explorer Previews
![preview1](Screenshot.png)

## Context Menu Previews
![Context Menu](context_menu.png)

## Support for Light Mode

Unfortunately, this mode do not work appropriately with the Light Mode. in the light mode, the ui elements will not contrast with the background and the style won't look any good.

## Blurbehind Requirements

To achieve the translucent effect in Explorer shown in the preview, you will need an external background blur tool:

* **Recommended:** The [Translucent Windows](https://windhawk.net/mods/translucent-windows) Windhawk mod (easiest to set up).
* **Alternative:** The third-party utility `ExplorerBlurMica`.

### Custom AccentBlurBehind Tinting
If translucent background makes text hard to read on light backgrounds, you can add a custom AccentBlurBehind code in the settings page of the Translucent windows Mod!
Here is the preview of the codes that can be used:-

* **Tint Code 1:** `B31A1A1A`  
  Preview: <img width="1324" height="702" alt="image" src="https://github.com/user-attachments/assets/782347de-2f31-44d0-abaf-78794050f4e7" />

* **Tint Code 2:** `761E1E1E`  
  Preview: <img width="1310" height="691" alt="image" src="https://github.com/user-attachments/assets/f1d9114e-d801-4b4b-a7e9-c1bbabfdf41d" />


---

## Theme Selection
Once merged, this theme will be integrated natively into the mod configuration and can be toggled directly from the main dropdown menu in the mod settings.

## Manual Installation / Testing
To test or apply this theme manually right now:
1. Open the **Windows 11 File Explorer Styler** mod in Windhawk.
2. Navigate to the **Settings** tab and toggle the viewing mode to **"Textual mode"**.
3. Clear the text area, copy the complete configuration block below, paste it inside, and hit **"Save settings"**.

<details>
<summary> Click to expand theme configuration code</summary>

```yaml
explorerFrameContainerHeight: 0
controlStyles:
  - target: "CommandBar#FileExplorerCommandBar"
    styles:
      - Background=Transparent
      - HorizontalAlignment=1
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
      - Background=Transparent
      - BorderThickness=0
  - target: "TabViewItem > Grid#LayoutRoot@CommonStates"
    styles:
      - Background@Selected:=<WindhawkBlur BlurAmount="15" TintColor="#25ffffff" />
      - Background@PointerOverSelected:=<WindhawkBlur BlurAmount="15" TintColor="#35ffffff" />
      - Background@Normal:=<WindhawkBlur BlurAmount="15" TintColor="#15ffffff" />
  - target: "Grid#TabContainerGrid > Border > Button#AddButton"
    styles:
      - Visibility=0
      - Margin=0,0,0,3
  - target: "Grid#CommandBarControlRootGrid"
    styles:
      - Background=Transparent
  - target: "Grid#NavigationBarControlGrid"
    styles:
      - Background=Transparent
  - target: "Grid#PART_LayoutRoot"
    styles:
      - Background:=<WindhawkBlur BlurAmount="15" TintColor="#25ffffff" />
      - CornerRadius=14
      - BorderThickness=1
      - BorderBrush:=<LinearGradientBrush StartPoint="0,0" EndPoint="1,1"><GradientStop Color="#80ffffff" Offset="0.0" /><GradientStop Color="{ThemeResource SurfaceStrokeColorDefault}" Offset="0.55" /><GradientStop Color="#80ffffff" Offset="1" /></LinearGradientBrush>
  - target: "FileExplorerExtensions.CommandBarControl"
    styles:
      - Margin=0,0,0,0
  - target: "AutoSuggestBox#FileExplorerSearchBox > Grid#LayoutRoot > TextBox > Grid@CommonStates > Border#BorderElement"
    styles:
      - Background:=<WindhawkBlur BlurAmount="15" TintColor="#25ffffff" />
      - CornerRadius=14
      - BorderThickness=1
      - BorderBrush:=<LinearGradientBrush StartPoint="0,0" EndPoint="1,1"><GradientStop Color="#80ffffff" Offset="0.0" /><GradientStop Color="{ThemeResource SurfaceStrokeColorDefault}" Offset="0.55" /><GradientStop Color="#80ffffff" Offset="1" /></LinearGradientBrush>
  - target: "Microsoft.UI.Xaml.Controls.AppBarButton"
    styles:
      - Background:=<WindhawkBlur BlurAmount="15" TintColor="#25ffffff" />
      - CornerRadius=12
      - BorderThickness=1
      - Margin=3,0,3,1
      - BorderBrush:=<LinearGradientBrush StartPoint="0,0" EndPoint="1,1"><GradientStop Color="#80ffffff" Offset="0.0" /><GradientStop Color="{ThemeResource SurfaceStrokeColorDefault}" Offset="0.55" /><GradientStop Color="#80ffffff" Offset="1" /></LinearGradientBrush>
  - target: "Microsoft.UI.Xaml.Controls.AppBarToggleButton"
    styles:
      - Background:=<WindhawkBlur BlurAmount="15" TintColor="#25ffffff" />
      - CornerRadius=12
      - BorderThickness=1
      - Margin=3,0,3,1
      - BorderBrush:=<LinearGradientBrush StartPoint="0,0" EndPoint="1,1"><GradientStop Color="#80ffffff" Offset="0.0" /><GradientStop Color="{ThemeResource SurfaceStrokeColorDefault}" Offset="0.55" /><GradientStop Color="#80ffffff" Offset="1" /></LinearGradientBrush>
  - target: "Button#MoreButton"
    styles:
      - Visibility=Collapsed
  - target: "Microsoft.UI.Xaml.Controls.AppBarSeparator"
    styles:
      - Visibility=Collapsed
  - target: "Microsoft.UI.Xaml.Controls.AppBarButton#backButton"
    styles:
      - Margin=0,9,9,0
  - target: "Microsoft.UI.Xaml.Controls.AppBarButton#forwardButton"
    styles:
      - Margin=0,9,9,0
  - target: "Microsoft.UI.Xaml.Controls.AppBarButton#upButton"
    styles:
      - Margin=0,9,9,0
  - target: "Microsoft.UI.Xaml.Controls.AppBarButton#refreshButton"
    styles:
      - Margin=0,9,9,0
