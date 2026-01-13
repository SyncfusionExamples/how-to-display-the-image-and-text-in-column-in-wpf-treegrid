# How to Display the Image and Text in WPF TreeGrid Column?

This example illustrates how to display the image and text in column in [WPF TreeGrid](https://www.syncfusion.com/wpf-controls/treegrid) (SfTreeGrid).

`TreeGrid` allows you to display image and text in the columns by using [TreeGridTemplateColumn](https://help.syncfusion.com/cr/wpf/Syncfusion.UI.Xaml.TreeGrid.TreeGridTemplateColumn.html).

#### XAML
``` xml
<syncfusion:TreeGridTemplateColumn MappingName="FirstName">
    <syncfusion:TreeGridTemplateColumn.CellTemplate>
        <DataTemplate>
            <StackPanel Orientation="Horizontal">
                <Image Source="Employee.png" HorizontalAlignment="Left"  Margin="5" VerticalAlignment="Center"/>
                <TextBlock Text="{Binding FirstName}"/>
            </StackPanel>
        </DataTemplate>
    </syncfusion:TreeGridTemplateColumn.CellTemplate>
    <syncfusion:TreeGridTemplateColumn.EditTemplate>
        <DataTemplate>
            <StackPanel Orientation="Horizontal">
                <Image Source="Employee.png" HorizontalAlignment="Left"  Margin="5" VerticalAlignment="Center"/>
                <TextBox Text="{Binding FirstName, Mode=TwoWay}"/>
            </StackPanel>
        </DataTemplate>
    </syncfusion:TreeGridTemplateColumn.EditTemplate>
</syncfusion:TreeGridTemplateColumn> 
```

![DataGrid column to show image and text in a column](ImageAndTextColumn.png)

## Requirements to run the demo 
Visual Studio 2015 and above versions.