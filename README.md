# How to Change Data Marker Symbols in a Blazor Chart

## Overview

This sample demonstrates how to customize data marker symbols in a Syncfusion [Blazor Charts](https://www.syncfusion.com/blazor-components/blazor-charts) component. The application displays a line chart bound to a collection of data points and enables chart markers for each point in the series. By configuring the marker shape, the sample replaces the default circular marker with a diamond marker, making it easier to visually distinguish charted values and improve chart readability.

The implementation focuses on marker customization that can be applied to chart series when highlighting data points is important for analysis, reporting, or presentation scenarios.

## Key Features

- Uses the `SfChart` component to render chart data.
- Configures a `ChartSeries` with `Type="ChartSeriesType.Line"`.
- Binds data through the `DataSource` property.
- Maps X and Y values using the `XName` and `YName` properties.
- Enables markers using `ChartMarker Visible="true"`.
- Customizes marker dimensions with the `Height` and `Width` properties.
- Changes the marker symbol using `Shape="ChartShape.Diamond"`.
- Demonstrates binding a collection of `ChartData` objects to the chart.

## Prerequisites

- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or [Visual Studio Code](https://code.visualstudio.com/)
- [.NET SDK](https://dotnet.microsoft.com/en-us/download/dotnet) compatible with the project's target framework

## How to Run the Project

**Visual Studio 2022**

1. Clone or download the repository.
2. Open the verified project file:

   `MarkerSymbol/MarkerSymbol.csproj`

3. Restore NuGet packages.
4. Build the project.
5. Run the application using `Ctrl+F5`.

**Visual Studio Code**

1. Clone or download the repository.
2. Open the repository folder in Visual Studio Code.
3. Open the integrated terminal.
4. Navigate to the project directory.

```bash
cd MarkerSymbol
```

5. Restore NuGet packages:

```bash
dotnet restore
```

6. Run the application:

```bash
dotnet run
```

7. Open the local URL displayed in the console output.

## Project Structure

`Pages/Index.razor` - Hosts the Syncfusion chart sample, binds data, enables chart markers, and sets `ChartMarker.Shape` to `ChartShape.Diamond`.

## Support and Feedback

- For general product questions, visit the [Syncfusion Community Forum](https://www.syncfusion.com/forums) or [Syncfusion Support](https://www.syncfusion.com/support).
- To report an issue specific to this sample, open a GitHub issue in this repository.
- Official documentation for chart markers and chart customization: https://help.syncfusion.com/chart-sdk/blazor/charts/getting-started

## License

This is a Syncfusion sample project provided to demonstrate product usage. Review the [Syncfusion license terms](https://www.syncfusion.com/sales/pricing?category=ui-components) before using Syncfusion components in your own applications.