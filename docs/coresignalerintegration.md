# ASPNET Core SignalR Integration

For more information about ASPNET Core SignalR check out [SignalR ASPNET Core Integration](https://aspnetboilerplate.com/Pages/Documents/SignalR-AspNetCore-Integration).

## 1. Add SignalR to ABP

***If you are using the ABP starter template SignalR is already implemented and you can skip to step 2***

Follow the installation steps [here](https://aspnetboilerplate.com/Pages/Documents/SignalR-AspNetCore-Integration#installation)

## 2. Add Abp.AppFactory.Sync

* Add the [Abp.AppFactory.Sync Nuget Package]() to your Web.Core project

* Add Abp.AppFactory.Sync as a dependency to you WebCoreModule
```cs
[DependsOn( ...,
   typeof(Abp.AppFactory.Sync)]
public class ExampleWebCoreModule : AbpModule 
{ 
...
}
```

## 3. Add Abp.AppFactory.Interfaces

***If Abp.AppFactory.Interfaces is already included in your Application project then skip to step 4***

* Add the [Abp.AppFactory.Interfaces Nuget Package]() to your Application project

* Add Abp.AppFactory.Interfaces as a dependency to you ApplicationModule
```cs
[DependsOn( ...,
   typeof(Abp.AppFactory.Interfaces)]
public class ExampleApplicationModule : AbpModule 
{ 
...
}
```