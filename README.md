#Migrate to netstandard

[.NET Framework to .NET Core](https://docs.microsoft.com/en-us/dotnet/core/porting)
[try-convert](https://github.com/dotnet/try-convert)

### Steps
```CMD
dotnet tool install -g try-convert --version 0.2.105801
try-convert --project project_name.csproj
```
