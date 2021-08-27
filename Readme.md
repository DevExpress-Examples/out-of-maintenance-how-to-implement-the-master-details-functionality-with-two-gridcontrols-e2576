<!-- default badges list -->
![](https://img.shields.io/endpoint?url=https://codecentral.devexpress.com/api/v1/VersionRange/128651632/10.1.6%2B)
[![](https://img.shields.io/badge/Open_in_DevExpress_Support_Center-FF7200?style=flat-square&logo=DevExpress&logoColor=white)](https://supportcenter.devexpress.com/ticket/details/E2576)
[![](https://img.shields.io/badge/📖_How_to_use_DevExpress_Examples-e9f6fc?style=flat-square)](https://docs.devexpress.com/GeneralInformation/403183)
<!-- default badges end -->
<!-- default file list -->
*Files to look at*:

* [MainWindow.xaml](./CS/WpfApplication15/MainWindow.xaml) (VB: [MainWindow.xaml](./VB/WpfApplication15/MainWindow.xaml))
* [MainWindow.xaml.cs](./CS/WpfApplication15/MainWindow.xaml.cs) (VB: [MainWindow.xaml.vb](./VB/WpfApplication15/MainWindow.xaml.vb))
<!-- default file list end -->
# How to implement the Master-Details functionality with two GridControls


<p>In this example, we demonstrated two general approaches to achieve this goal:<br /><br />1. If the data source object does not have a property that includes all child rows, you can handle changes of the master grid's selection and filter the detail grid's source based on the selected value. In the latest version of this example, we implemented this logic in the <strong>CurrentRow</strong> property setter; this property is bound to the GridControl's <a href="https://documentation.devexpress.com/#WPF/DevExpressXpfGridDataControlBase_CurrentItemtopic">CurrentItem</a> property.<br /><br />2. In the case when master row objects contain child items (in our example, <strong>GridControl</strong> contains <strong>DataRowView</strong> objects with a separate <strong>CompanyModels</strong> property), it's easier to bind the detail grid's <strong>ItemsSource</strong> property to the selected item directly.</p>

<br/>


