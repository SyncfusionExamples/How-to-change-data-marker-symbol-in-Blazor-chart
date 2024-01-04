# How-to-change-data-marker-symbol-in-Blazor-chart.

This article explains how to change data marker symbol in Blazor Chart Component.

**Changing marker symbol in Blazor chart**

[Blazor Chart](https://www.syncfusion.com/blazor-components/blazor-charts) provides data markers to adorn the data points with different shapes and labels. It is enabled by setting [Visible](https://help.syncfusion.com/cr/blazor/Syncfusion.Blazor.Charts.ChartCommonMarker.html#Syncfusion_Blazor_Charts_ChartCommonMarker_Visible) Property of [ChartMarker](https://help.syncfusion.com/cr/blazor/Syncfusion.Blazor.Charts.ChartMarker.html) to **true**. 

The default shape of data marker in [Blazor Chart](https://www.syncfusion.com/blazor-components/blazor-charts) is **Circle**. It can be assigned different shapes such as Rectangle, Circle, Diamond etc., by using the [Shape](https://help.syncfusion.com/cr/blazor/Syncfusion.Blazor.Charts.ChartCommonMarker.html#Syncfusion_Blazor_Charts_ChartCommonMarker_Shape) property. 

The following code illustrates how to use the [Shape](https://help.syncfusion.com/cr/blazor/Syncfusion.Blazor.Charts.ChartCommonMarker.html#Syncfusion_Blazor_Charts_ChartCommonMarker_Shape) property to change the data marker symbol.

**Index.razor**

```cshtml

@using Syncfusion.Blazor.Charts

<SfChart>
    <ChartSeriesCollection>
        <ChartSeries DataSource="@ConsumerReports" XName="X" YName="Y" Type="ChartSeriesType.Line">
            <ChartMarker Visible="true" Height="10" Width="10" Shape="ChartShape.Diamond"/>
        </ChartSeries>
    </ChartSeriesCollection>
</SfChart>

@code {
    public class ChartData
    {
        public double X { get; set; }
        public double Y { get; set; }
    }

    public List<ChartData> ConsumerReports = new List<ChartData>
    {
        new ChartData{ X= 20, Y= 28 },
        new ChartData{ X= 25, Y= 20 },
        new ChartData{ X= 30, Y= 30 },
        new ChartData{ X= 35, Y= 27 },
        new ChartData{ X= 40, Y= 15 },
        new ChartData{ X= 45, Y= 35 },
        new ChartData{ X= 50, Y= 30 }
    };
}

```

The following screenshot illustrates the output of the above code snippet.

**Output:**

![](/marker.png)

**Conclusion**

I hope you enjoyed learning how to change data marker symbol in Blazor Chart Component.

You can refer to our [Blazor Chart feature tour](https://www.syncfusion.com/blazor-components/blazor-charts) page to know about its other groundbreaking feature representations and [documentation](https://blazor.syncfusion.com/documentation/chart/getting-started), and how to quickly get started for configuration specifications. You can also explore our [Blazor Chart example](https://blazor.syncfusion.com/demos/chart/line?theme=bootstrap5) to understand how to create and manipulate data.

For current customers, you can check out our components from the [License and Downloads](https://www.syncfusion.com/sales/teamlicense) page. If you are new to Syncfusion, you can try our 30-day [free trial](https://www.syncfusion.com/downloads/blazor) to check out our other controls.

If you have any queries or require clarifications, please let us know in the comments section below. You can also contact us through our [support forums](https://www.syncfusion.com/forums), [support portal](https://support.syncfusion.com/create), or [feedback portal](https://www.syncfusion.com/feedback/blazor-components?control=charts). We are always happy to assist you!