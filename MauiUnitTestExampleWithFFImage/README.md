# Introduction 
This is a sample repro project to show the issue with FFImageLoadingCompat NuGet packages in a MAUI app that targets 'vanilla' net7.0 so it can be tested by an NUnit project

# To Repro the Issue 
1.) Add just the single FFImageLoadingCompat NuGet package to Maui app project. Package is successfully added 
2.) Attempt to add one ore more of the other 4 packages:
    - FFImageLoadingCompat.Maui
    - FFImageLoadingCompat.Transformation
    - FFImageLoadingCompat.Svg
    - FFImageLoadingCompat.Svg.Maui

Result:
In Package Console output:
Package FFImageLoadingCompat.Maui 0.1.1 is not compatible with net7.0 (.NETCoreApp,Version=v7.0). Package FFImageLoadingCompat.Maui 0.1.1 supports:
  - net7.0-android33.0 (.NETCoreApp,Version=v7.0)
  - net7.0-ios16.1 (.NETCoreApp,Version=v7.0)
  - net7.0-maccatalyst16.1 (.NETCoreApp,Version=v7.0)
  - net7.0-windows10.0.19041 (.NETCoreApp,Version=v7.0)
