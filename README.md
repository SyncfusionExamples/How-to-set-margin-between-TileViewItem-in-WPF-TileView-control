# Margin Between TileViewItem in WPF TileViewControl
This sample shows how to add consistent spacing between items in a Syncfusion WPF TileViewControl by styling the TileViewItem container. You’ll learn how to apply margins via ItemContainerStyle, tune layout spacing in both Normal and Maximized states, and theme the control.

## Features
- Set uniform outer spacing for each TileViewItem via ItemContainerStyle
- Different margins for Normal and Maximized states if desired
- Works with ItemsSource or direct child items
- Compatible with themes and custom templates
- Simple and MVVM-friendly approach

## Getting Started
1. Create a new WPF project in Visual Studio.
2. Install the NuGet package: Syncfusion.Tools.WPF.
3. Add the Syncfusion XML namespace in XAML:
   - xmlns:syncfusion="http://schemas.syncfusion.com/wpf"
4. Place a TileViewControl in your Window/Page.
5. Apply an ItemContainerStyle that sets the Margin on TileViewItem.
6. Optionally apply a theme using syncfusion:SkinStorage.VisualStyle.

## How It Works
TileViewControl generates TileViewItem containers for each item. By setting an ItemContainerStyle that targets TileViewItem and assigns the Margin property, you create visual gaps between tiles. This does not alter the inner content’s padding; use Padding inside your item template if you also want spacing within a tile.

## Usage Tips
- Use Margin on the TileViewItem for outer spacing; use Padding inside your item template for inner spacing.
- Keep margins modest (e.g., 6–12) to avoid excessive whitespace and preserve layout balance.
- If you need different spacing when a tile is maximized, use triggers on TileViewItem.State to adjust Margin conditionally.
- Combine with Grid or UniformGrid-like sizing inside the item template to create consistent inner layouts.
- Theme with syncfusion:SkinStorage.VisualStyle to match your application’s branding.

## About the Sample
This sample focuses on spacing between tiles in the Syncfusion WPF TileViewControl, providing a clean, readable layout with simple styling that works well in MVVM scenarios. Extend it by adding commands, richer item templates, and responsive sizing behavior.
