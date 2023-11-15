pi@pi-top:~ mkdir /home/pi/localNuget
```

Configure the Nuget soruces by having a ```Nuget.Config``` file in the folder ```~/.nuget/NuGet```
Configure the Nuget sources by having a ```Nuget.Config``` file in the folder ```~/.nuget/NuGet```

The file should contain the following sources
```xml
<?xml version="1.0" encoding="utf-8"?>
<configuration>
  <solution>
    <add key="disableSourceControlIntegration" value="true" />
  </solution>
  <packageSources>
    <clear />
    <add key="local" value="/home/pi/localNuget" />
    <add key="nuget.org" value="https://api.nuget.org/v3/index.json" />
    <add key="dotnet-eng" value="https://pkgs.dev.azure.com/dnceng/public/_packaging/dotnet-eng/nuget/v3/index.json" />
    <add key="dotnet-tools" value="https://pkgs.dev.azure.com/dnceng/public/_packaging/dotnet-tools/nuget/v3/index.json" />
    <add key="dotnet3-dev" value="https://pkgs.dev.azure.com/dnceng/public/_packaging/dotnet3.1/nuget/v3/index.json" />
    <add key="dotnet5" value="https://pkgs.dev.azure.com/dnceng/public/_packaging/dotnet5/nuget/v3/index.json" />
    <add key="MachineLearning" value="https://pkgs.dev.azure.com/dnceng/public/_packaging/MachineLearning/nuget/v3/index.json" />
    <add key="PSGallery" value="https://www.powershellgallery.com/api/v2/" />
  </packageSources>
</configuration>
```
0 comments on commit 113955d
