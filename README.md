# Creating Stacked Waterfall Chart using Blazor BarChart

## Overview

This sample demonstrates how to create a waterfall-style chart using the Syncfusion [Blazor Chart](https://www.syncfusion.com/blazor-components/blazor-charts) component and stacked bar series. Instead of using a dedicated waterfall series, the implementation creates the visual effect by combining multiple `StackingBar` series and an additional baseline series that offsets the visible values. This approach is useful when developers need greater control over segment positioning while presenting cumulative business metrics, financial results, or category-based comparisons.

## Key Features

- Uses the `SfChart` component to render a waterfall-style visualization.
- Configures `ChartPrimaryXAxis` with `ValueType.Category` to display category labels.
- Uses multiple `ChartSeries` elements with `Type="ChartSeriesType.StackingBar"` to build the stacked waterfall layout.
- Implements an invisible baseline series using the `baseline` data field to offset visible bars.
- Maps category values through the `XName` property.
- Maps stacked values through the `YName` property using `baseline`, `y1`, and `y2` data fields.
- Customizes series appearance through the `Fill` property.
- Removes unnecessary axis visuals by configuring `ChartAxisMajorGridLines` and `ChartAxisMajorTickLines` with a width of `0`.
- Demonstrates custom chart data modeling using category names and stacked numeric values.
- Provides a practical technique for creating waterfall-style charts using stacked bar chart functionality.

## Prerequisites

- Visual Studio 2022 or Visual Studio Code
- .NET SDK compatible with the project's target framework

## How to Run the Project

**Visual Studio 2022**

1. Clone or download this repository.
2. Open the solution file:

   `WaterfallChart.sln`

3. Restore all NuGet packages.
4. Set the startup project to `WaterfallChart` if required.
5. Build the solution.
6. Run the application using **Ctrl+F5**.

**Visual Studio Code**

1. Open the repository folder in Visual Studio Code.
2. Open the integrated terminal.
3. Navigate to the project directory.

```bash
dotnet restore
dotnet run
```

4. Open the local application URL displayed in the application output.

## Project Structure

- `Pages/Index.razor` — contains the `SfChart`, stacked bar series configuration, axis definitions, and waterfall-style implementation.

## Support and Feedback

- For general product questions, visit the [Syncfusion Community Forum](https://www.syncfusion.com/forums) or [Syncfusion Support](https://www.syncfusion.com/support).
- To report an issue specific to this sample, open a GitHub issue in this repository.
- For detailed documentation about creating chart visualizations with Syncfusion Blazor Charts, see: https://help.syncfusion.com/chart-sdk/blazor/charts/chart-types/waterfall

## License

This is a Syncfusion sample project provided to demonstrate product usage. Review the [Syncfusion license terms](https://www.syncfusion.com/sales/pricing?category=ui-components) before using Syncfusion components in your own applications.