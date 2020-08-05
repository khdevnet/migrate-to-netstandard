#Migrate to netstandard

[portability-analyzer](https://docs.microsoft.com/en-us/dotnet/standard/analyzers/portability-analyzer)
[.NET Framework to .NET Core](https://docs.microsoft.com/en-us/dotnet/core/porting)
[try-convert](https://github.com/dotnet/try-convert)

### Steps
```CMD
dotnet tool install -g try-convert --version 0.2.105801
try-convert --project project_name.csproj
```
Install  Windows.Compatibility if Service.Model dependencies exist
```
Install-Package Microsoft.Windows.Compatibility -Version 3.1.0
```
