# Mica Tabless Theme for File Explorer
a Theme that adds Mica Backdrop to Top Toolbars, and Visually Removes Tab Switcher at the Same Time!
Bonus : if you have MicaForEveryone or Translucent Backdrops Windhawk Mod, even the Details/Preview Panel has your Backdrop of Choice :D

Preview is Full-Size to also show the Details/Preview Pane

Also Check Out : Translucent Windows Mod

<img width="1720" height="880" alt="image" src="https://github.com/user-attachments/assets/1504d478-6cd3-42e6-8b00-093d8f540787" />

# Manual Installation :
The theme styles can be imported manually. To do that, follow these steps:
- Open the Windows 11 Taskbar Styler mod in Windhawk.
- Go to the "Advanced" tab.
- Copy the content below to the text box under "Mod settings" and click "Save".

<details>
<summary>Content to import (click to expand)</summary>

```json
{
"controlStyles[0].target":"Microsoft.UI.Xaml.Controls.Grid#CommandBarControlRootGrid",
  "controlStyles[0].styles[0]":"Background=Transparent",
"controlStyles[1].target":"Microsoft.UI.Xaml.Controls.Grid#ContentRoot",
  "controlStyles[1].styles[0]":"Background=Transparent",
"controlStyles[2].target":"FileExplorerExtensions.NavigationBarControl",
  "controlStyles[2].styles[0]":"Grid.Row=$NavigationBarGrid",
"controlStyles[3].target":"FileExplorerExtensions.CommandBarControl",
  "controlStyles[3].styles[0]":"Grid.Row=$CommandBarGrid",
"controlStyles[4].target":"Microsoft.UI.Xaml.Controls.Grid#TabContainerGrid > Border",
  "controlStyles[4].styles[0]":"Visibility=Collapsed",
"controlStyles[5].target":"Microsoft.UI.Xaml.Controls.Grid#TabContainer > Microsoft.UI.Xaml.Controls.Button#CloseButton",
  "controlStyles[5].styles[0]":"Visibility=Collapsed",
"controlStyles[6].target":"Microsoft.UI.Xaml.Controls.TabViewItem > Microsoft.UI.Xaml.Controls.Grid#LayoutRoot > Microsoft.UI.Xaml.Controls.Canvas",
  "controlStyles[6].styles[0]":"Opacity=0",
"controlStyles[7].target":"Grid#NavigationBarControlGrid",
  "controlStyles[7].styles[0]":"Background:=<SolidColorBrush Color=\"{ThemeResource SystemChromeLowColor}\" />",
"controlStyles[8].target":"Microsoft.UI.Xaml.Controls.Grid#TabContainer",
  "controlStyles[8].styles[0]":"BorderThickness=0",
"controlStyles[9].target":"Microsoft.UI.Xaml.Controls.ContentPresenter > Microsoft.UI.Xaml.Controls.StackPanel > Microsoft.UI.Xaml.Controls.TextBlock",
  "controlStyles[9].styles[0]":"FontFamily=Segoe UI, Segoe Fluent Icons",
  "controlStyles[9].styles[1]":"FontWeight=Normal",
"controlStyles[10].target":"Microsoft.UI.Xaml.Controls.Grid#CommandBarControlRootGrid",
  "controlStyles[10].styles[0]":"BorderThickness=0,0,0,1",
"controlStyles[11].target":"FileExplorerExtensions.FileExplorerTabControl",
  "controlStyles[11].styles[0]":"Height=36",
"controlStyles[12].target":"Microsoft.UI.Xaml.Controls.Grid#TabContainer",
  "controlStyles[12].styles[0]":"Padding=1,0,0,1",
"controlStyles[13].target":"Microsoft.UI.Xaml.Controls.Viewbox#IconBox",
  "controlStyles[13].styles[0]":"Margin=0,0,4,0",
"controlStyles[14].target":"Microsoft.UI.Xaml.Controls.TabViewItem",
  "controlStyles[14].styles[0]":"Margin=0,-8,0,0",
"explorerFrameContainerHeight":0,
"controlStyles[15].target":"Microsoft.UI.Xaml.Controls.Grid#NavigationBarControlGrid",
  "controlStyles[15].styles[0]":"Background=Transparent",
"controlStyles[16].target":" Microsoft.UI.Xaml.Controls.Grid#DetailsViewControlRootGrid",
  "controlStyles[16].styles[0]":"Background=Transparent",
"controlStyles[17].target":"Microsoft.UI.Xaml.Controls.AppBarSeparator",
  "controlStyles[17].styles[0]":"Opcaity=0"
"styleConstants[0]":"NavigationBarGrid=1",
"styleConstants[1]":"CommandBarGrid=2",
}
```
</details>
