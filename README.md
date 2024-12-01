# Dalamud.NET.Sdk
.NET SDK for use with Dalamud plugins. [See SamplePlugin](https://github.com/goatcorp/SamplePlugin/blob/master/SamplePlugin/SamplePlugin.csproj) for usage.

## When updating this package
...you need to make sure to [tell Plogon to download the new version instead](https://github.com/goatcorp/Plogon/blob/master/Plogon/BuildProcessor.cs#L102).

## Testing locally
Create a `nuget.config` file with the following contents in the directory of the project you want to test with, pointing to the `bin/Release` directory.

```xml
<?xml version="1.0" encoding="utf-8"?>
<configuration>
  <packageSources>
    <add key="local-packages" value="C:\repos\Dalamud.NET.Sdk\Dalamud.NET.Sdk\bin\Release" />
  </packageSources>
</configuration>
```

### Acknowledgements
This project is a fork of Godot's .NET SDK, licensed under the MIT license, located [here](https://github.com/godotengine/godot/tree/master/modules/mono/editor/Godot.NET.Sdk/Godot.NET.Sdk).
