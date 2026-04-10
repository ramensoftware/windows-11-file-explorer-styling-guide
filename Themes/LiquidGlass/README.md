# LiquidGlass theme for Windows 11 File Explorer Styler

**Author**: [PhantomNimbi](https://github.com/PhantomNimbi)

---

### Requirements

* [Windows 11 File Explorer Styler](https://windhawk.net/mods/windows-11-file-explorer-styler)
* [Translucent Windows](https://windhawk.net/mods/translucent-windows)

---

![Screenshot](screenshot.png)

---

## Translucent Windows

> [!NOTE]
> Make sure to change the "AccentBlurBehind color blend" setting to "cccccccc" if you are using this with Light themes.

To import the mod settings, follow these steps:

* Open the "Translucent Windows" mod in Windhawk.
* Go to the "Settings" tab and select "Textual mode".
* Copy the content below to the text box and click "Save settings".

<details>
<summary>Content to import (click to expand)</summary>

```yaml
RenderingMod:
  ThemeBackground: 1
  SysColors: 1
  AccentColorControls: 1
type: acrylicblur
AccentBlurBehind: 3A232323
FlyoutsEffects: 1
ImmersiveDarkTitle: 1
ExtendFrame: 1
CornerOption: smallround
RainbowSpeed: 1
TitlebarColor:
  ColorTitlebar: 0
  RainbowTitlebar: 0
  titlerbarstyles_active: FF0000
  titlerbarstyles_inactive: 00FFFF
TitlebarTextColor:
  ColorTitlebarText: 0
  RainbowTextColor: 0
  titlerbarcolorstyles_active: ''
  titlerbarcolorstyles_inactive: ''
BorderColor:
  ColorBorder: 0
  RainbowBorder: 0
  borderstyles_active: ''
  borderstyles_inactive: ''
RuledPrograms:
  - target: mspaint.exe
    RenderingMod:
      ThemeBackground: 0
      AccentColorControls: 0
    type: none
    AccentBlurBehind: 3A232323
    ImmersiveDarkTitle: 0
    ExtendFrame: 0
    CornerOption: default
    RainbowSpeed: 1
    TitlebarColor:
      ColorTitlebar: 0
      RainbowTitlebar: 0
      titlerbarstyles_active: FF0000
      titlerbarstyles_inactive: 00FFFF
    TitlebarTextColor:
      ColorTitlebarText: 0
      RainbowTextColor: 0
      titlerbarcolorstyles_active: FF0000
      titlerbarcolorstyles_inactive: 00FFFF
    BorderColor:
      ColorBorder: 0
      RainbowBorder: 0
      borderstyles_active: FF0000
      borderstyles_inactive: 00FFFF
```
</details>

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
styleConstants:
  - ContentBG=<SolidColorBrush Color="{ThemeResource SystemChromeAltHighColor}" Opacity="1" />
  - Background=<WindhawkBlur BlurAmount="15" TintColor="{ThemeResource SystemAltLowColor}" TintOpacity="0.2" />
  - ElementBackground=<WindhawkBlur BlurAmount="20" TintColor="{ThemeResource SystemAltLowColor}" TintOpacity="0.4" />
  - ElementBackground2=<WindhawkBlur BlurAmount="20" TintColor="{ThemeResource SystemAltLowColor}" TintOpacity="0.2" />
  - AccentBackground=<WindhawkBlur BlurAmount="15" TintColor="{ThemeResource SystemAccentColorLight1}" TintOpacity="0.2" />
  - BorderBrush=<LinearGradientBrush StartPoint="0,0" EndPoint="0,1"><GradientStop Color="#50808080" Offset="0.0" /><GradientStop Color="#50404040" Offset="0.25" /><GradientStop Color="#50808080" Offset="1" /></LinearGradientBrush>
  - ElementBorderBrush=<LinearGradientBrush StartPoint="0,0" EndPoint="0,1"><GradientStop Color="#50808080" Offset="1" /><GradientStop Color="#50606060" Offset="0.15" /></LinearGradientBrush>
  - BorderThickness=0.3,1,0.3,0.3
  - ElementBorderThickness=0.3,0.3,0.3,1
  - CornerRadius=12
  - ElementCornerRadius=8
controlStyles:
  - target: Microsoft.UI.Xaml.Controls.Grid#PART_LayoutRoot
    styles:
      - Background=Transparent
      - HorizontalAlignment=Stretch
  - target: FileExplorerExtensions.FirstCrumbStackPanelControl#FirstCrumbStackPanel
    styles:
      - Visibility=1
  - target: Windows.UI.Xaml.Controls.Grid#RootCommandSearchGrid > Windows.UI.Xaml.Controls.Border#BorderElement
    styles:
      - Visibility=1
  - target: Microsoft.UI.Xaml.Controls.Primitives.NavigationViewItemPresenter#NavigationViewItemPresenter > Microsoft.UI.Xaml.Controls.Grid#LayoutRoot
    styles:
      - BorderThickness=$ElementBorderThickness
      - Background:=$ElementBackground
      - BorderBrush:=$ElementBorder
      - CornerRadius=$ElementCornerRadius
  - target: Microsoft.UI.Xaml.Controls.Grid#NavigationBarControlGrid
    styles:
      - Background:=Transparent
      - BorderBrush:=Transparent
  - target: Microsoft.UI.Xaml.Controls.Grid#HomeViewRootGrid
    styles:
      - BorderBrush:=$ElementBorderBrush
      - CornerRadius=$ElementCornerRadius
      - BorderThickness=$ElementBorderThickness
      - Margin=4,0
  - target: 'FileExplorerExtensions.GalleryViewControl#GalleryViewControl > Grid  '
    styles:
      - BorderBrush:=$ElementBorderBrush
      - CornerRadius=$ElementCornerRadius
      - BorderThickness=$ElementBorderThickness
      - Margin=4,0
  - target: FileExplorerExtensions.GalleryViewControl#GalleryViewControl > Grid > Grid#GalleryRootGrid
    styles:
      - Background:=Transparent
  - target: ToolTip
    styles:
      - BorderBrush:=$ElementBorderBrush
      - BorderThickness=$ElementBorderThickness
      - CornerRadius=$ElementCornerRadius
  - target: Grid#TabContainerGrid > Border#LeftBottomBorderLine
    styles:
      - Visibility=1
  - target: Grid#TabContainerGrid > Border#RightBottomBorderLine
    styles:
      - Visibility=1
  - target: TabViewItem > Grid#LayoutRoot
    styles:
      - Margin=5
      - Height=35
      - BorderThickness=$ElementBorderThickness
      - CornerRadius=$ElementCornerRadius
      - BorderBrush:=$ElementBorderBrush
  - target: TabViewItem > Grid#LayoutRoot > Canvas
    styles:
      - Visibility=1
  - target: TabViewItem > Grid#LayoutRoot > Grid#TabContainer
    styles:
      - Background=Transparent
      - BorderBrush=Transparent
  - target: TabViewItem > Grid#LayoutRoot@CommonStates
    styles:
      - Background@Selected:=$ElementBackground
      - Background@PointerOverSelected:=$AccentBackground
      - Background@PointerOver:=$AccentBackground
      - Background@Normal:=$ElementBackground
      - Background@PressedSelected:=$ButtonBackground2
  - target: Grid#TabContainerGrid > Border#LeftBottomBorderLine
    styles:
      - Visibility=1
  - target: Grid#TabContainerGrid > Border#RightBottomBorderLine
    styles:
      - Visibility=1
  - target: Microsoft.UI.Xaml.Controls.Border#BottomBorderLine
    styles:
      - Visibility=1
  - target: Microsoft.UI.Xaml.Shapes.Path#LeftRadiusRenderArc
    styles:
      - Visibility=1
  - target: Microsoft.UI.Xaml.Shapes.Path#RightRadiusRenderArc
    styles:
      - Visibility=1
  - target: Microsoft.UI.Xaml.Controls.Grid#TabContainer
    styles:
      - Visibility=0
  - target: Microsoft.UI.Xaml.Controls.Viewbox#IconBox
    styles:
      - Visibility=1
  - target: CommandBarOverflowPresenter#SecondaryItemsControl > Grid#LayoutRoot
    styles:
      - Background:=$ElementBackground
      - BorderThickness=$ElementBorderThickness
      - BorderBrush:=$ElementBorderBrush
      - CornerRadius=$ElementCornerRadius
  - target: Microsoft.UI.Xaml.Controls.AutoSuggestBox#FileExplorerSearchBox > Microsoft.UI.Xaml.Controls.Grid#LayoutRoot > Microsoft.UI.Xaml.Controls.TextBox#TextBox
    styles:
      - CornerRadius=$ElementCornerRadius
      - Background:=$ElementBackground
      - BorderBrush:=$ElementBorderBrush
      - BorderThickness=$ElementBorderThickness
  - target: Microsoft.UI.Xaml.Controls.Grid#FileExplorerAddressBarGrid
    styles:
      - CornerRadius=$ElementCornerRadius
      - Background:=$ElementBackground
      - BorderBrush:=$ElementBorderBrush
      - BorderThickness=$ElementBorderThickness
  - target: Microsoft.UI.Xaml.Controls.AutoSuggestBox#PART_AutoSuggestBox > Microsoft.UI.Xaml.Controls.Grid#LayoutRoot > Microsoft.UI.Xaml.Controls.TextBox#TextBox
    styles:
      - CornerRadius=$ElementCornerRadius
  - target: Microsoft.UI.Xaml.Controls.Grid#RootContainer
    styles:
      - Background:=Transparent
  - target: Microsoft.UI.Xaml.Controls.Border > Microsoft.UI.Xaml.Controls.Button#AddButton
    styles:
      - RenderTransform:=<TranslateTransform Y="-8" />
  - target: Microsoft.UI.Xaml.Controls.TextBlock#TextLabel
    styles:
      - Visibility=1
  - target: Microsoft.UI.Xaml.Controls.Grid#SubItemChevronPanel > Microsoft.UI.Xaml.Controls.FontIcon#SubItemChevron
    styles:
      - RenderTransform:=<TranslateTransform X="-5" Y="12" />
  - target: TabViewItem > Grid#LayoutRoot
    styles:
      - Height = 28
  - target: TabViewItem > Grid#LayoutRoot > Canvas
    styles:
      - Visibility=1
  - target: FileExplorerExtensions.CommandBarControl
    styles:
      - Visibility=1
  - target: FileExplorerExtensions.NavigationBarControl
    styles:
      - Grid.RowSpan=2
      - Margin=0,0,0,1
  - target: Grid#DetailsViewControlRootGrid
    styles:
      - Background:=Transparent
  - target: StackPanel#DetailsViewThumbnail
    styles:
      - Background:=Transparent
explorerFrameContainerHeight: 87
```
</details>
