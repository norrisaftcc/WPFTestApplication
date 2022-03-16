***WPFTestApplication***

Note that this totally leaks my Bing Maps key, and I would yell at a student who did that -- but I was in a hurry.

***Instructions***

This is a tutorial for how to set up a Bing Maps control within a WPF application.

3/16/2022

Installed fresh Visual Studio Community 2022

Created new WPF project

NuGet: added Bing Map Control:
Install-Package Microsoft.Maps.MapControl.WPF -Version 1.0.0.3
(just typed in the package name in nuget, installed)

Now following this tutorial:
https://docs.microsoft.com/en-us/previous-versions/bing/wpf-control/hh830433(v=msdn.10)

Detour to get Bing Maps Key using FTCC Visual Studio login
key name: BingMapsTest
Basic / Dev/Test

At this point, my WPF MainWindow.xaml reads:
----
<Window x:Class="WPFTestApplication.MainWindow"
        xmlns="http://schemas.microsoft.com/winfx/2006/xaml/presentation"
        xmlns:x="http://schemas.microsoft.com/winfx/2006/xaml"
        xmlns:d="http://schemas.microsoft.com/expression/blend/2008"
        xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006"
        xmlns:m="clr-namespace:Microsoft.Maps.MapControl.WPF;assembly=Microsoft.Maps.MapControl.WPF"
        xmlns:local="clr-namespace:WPFTestApplication"
        mc:Ignorable="d"
        Title="MainWindow" Height="450" Width="800">
    <Grid>
        <m:Map x:Name="myMap" CredentialsProvider="ArRifk6122ZB2RSEec6gQgmQte_NcFEvVXoj7Er8B-nzf9du4Xdd1mr1j9Sug378" Mode="Aerial"/>
    </Grid>
    
</Window>
----

***Further Work***
A lot, probably. 
