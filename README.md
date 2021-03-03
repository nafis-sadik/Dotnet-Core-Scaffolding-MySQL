# Scaffolding-MYSQL Database in Dotnet Core

![Framework](https://img.shields.io/badge/framework-.net%20core%20v3.1-green)
![Database](https://img.shields.io/badge/Database-MySQL-brightgreen)

# About This
This is a project for Scaffolding DBContext in Entity Framework Core from existing MySql database.

# NuGet Packages
  
| NuGet Packages | Version |
| ------ | ------ |
| MySql.Data | 8.0.23 |
| MySql.Data.EntityFrameworkCore | 8.0.22 |
| Microsoft.EntityFrameworkCore.Tools | 3.1.1 |

# Dependencies
  - Visual Studio 2019 | [Download](https://visualstudio.microsoft.com/downloads/)
  - Dotnet Core 3.1 | [Download](https://dotnet.microsoft.com/download/dotnet-core/3.1) |

# How to use it?
It's very simple. It's a C# class library targeting ***.net core 3.1.*** So makesure you have ***.net core 3.1 selected as target framework***.

**Step # 1 :** 
    
    Clone the repository
**Step # 2 :** 
    
    Open the solution file with Visual Studio 2019
**Step # 3 :** 

    Go to ***Tools > NuGet package manger > Package Manager Console***
**Step # 4 :** 

```sh
Scaffold-DbContext "server=[Database Source];User Id=[Your User Id];Password=[Your Password];Database=[Database Name];Port=[Your Port];" MySql.EntityFrameworkCore -OutputDir Models
```


**For Xampp**
* Default Port is 3306
* Default user is root
* No password for root user, so remove the password section from connection string above at ***Step # 4***

***Example (Connection string for Xampp)***

```Scaffold-DbContext "server=localhost;User Id=root;Database=test;Port=3306;" MySql.EntityFrameworkCore -OutputDir Models```

License
----

MIT


**Free Software, Hell Yeah!**

***Tools I used to create this read me. Might also help you!***

* [Shields IO](https://shields.io)
* [JBT](https://jbt.github.io/markdown-editor/)
