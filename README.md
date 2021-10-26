# myWebApp
An test ASP.NET app

## Cheatsheet

```
dotnet watch run --urls="http://localhost:8080"
dotnet build
dotnet publish --configuration Release
```

## Troubleshooting

### IIS Permission
```jsx
HTTP Error 500.19 - Internal Server Error
The requested page cannot be accessed because the related configuration data for the page is invalid.

Detailed Error Information:
Module	   IIS Web Core
Notification	   Unknown
Handler	   Not yet determined
Error Code	   0x80070005
Config Error	   Cannot read configuration file due to insufficient permissions
Config File	   \\?\C:\Users\cwang\myWebApp\bin\Release\net5.0\publish\web.config

```

Solution:  Add `IIS_IUSR`  to the `publish` folder

## References
* [Configure an ASP.NET Website on IIS](https://docs.microsoft.com/en-us/iis/application-frameworks/scenario-build-an-aspnet-website-on-iis/configure-an-asp-net-website-on-iis)
* [ASP.NET Tutorial | Hello World in 5 minutes | .NET](https://dotnet.microsoft.com/learn/aspnet/hello-world-tutorial/intro)
* [Publish an ASP.NET Core app to IIS](https://docs.microsoft.com/en-us/aspnet/core/tutorials/publish-to-iis?view=aspnetcore-5.0&tabs=visual-studio)
* [Application Pool Identities](https://docs.microsoft.com/en-us/iis/manage/configuring-security/application-pool-identities)
