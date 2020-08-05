# Migrate to netstandard

* [portability-analyzer](https://docs.microsoft.com/en-us/dotnet/standard/analyzers/portability-analyzer)
* [.NET Framework to .NET Core](https://docs.microsoft.com/en-us/dotnet/core/porting)
* [try-convert](https://github.com/dotnet/try-convert)

### Steps
1 Migrate project files
```CMD
dotnet tool install -g try-convert --version 0.2.105801
try-convert --project project_name.csproj
```
2 Migrate packages.config file (right click and migrate)

3 Install  Windows.Compatibility (if some assemblies depends on it)
```
Install-Package Microsoft.Windows.Compatibility -Version 3.1.0
```

4 Remove packages.config

