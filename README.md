# Rotativa.AspNetCore 3.x

Rotativa for Asp.Net Core 3.x.

Docs are in the making. Should work almost exactly as Rotativa https://github.com/webgio/Rotativa
This repository is a fork to update to support Asp.Net Core 3.x

## Development version
Clone this repo and copy Rotativa.AspNetCore folder to your application project.
You may find wkhtmltopdf.exe in wwwroot folder of the demo project.

```
git clone https://github.com/utarn/Rotativa.AspNetCore
```

Please give feedback!

## Needs configuration
Basic configuration done in Startup.cs:

```csharp
RotativaConfiguration.Setup(env);
```
or, 

```csharp
RotativaConfiguration.Setup(env, "path/relative/to/root");
```

Make sure you have a folder with the wkhtmltopdf.exe file accessible by the process running the web app. By default it searches in a folder named "Rotativa" in the root of the web app. If you need to change that use the optional parameter to the Setup call `RotativaConfiguration.Setup(env, "path/relative/to/root")`

## Issues and Pull Request
Contribution is welcomed. If you would like to provide a PR please add some testing.