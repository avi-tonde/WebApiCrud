.NET API Crud:

Commands Used:

**Create SLN File with new folder:**
$ dotnet new sln -n WebApiCrud -o WebApiCrud

**Create NewClass Library: Domain Layer**
$ dotnet new classlib -n WebApiCrud.Domain

**Create NewClass Library: Database Layer**
$ dotnet new classlib -n WebApiCrud.Data

**Create New WebApi Project: APIEndpoint**
$ dotnet new webapi -n WebApiCrud.ApiEndpoint


**************************************************************
                    Add Projects to SLN
**************************************************************

$ dotnet sln WebApiCrud.sln add WebApiCrud.ApiEndpoint/WebApiCrud.ApiEndpoint.csproj

$ dotnet sln WebApiCrud.sln add WebApiCrud.Domain/WebApiCrud.Domain.csproj

$ dotnet sln WebApiCrud.sln add WebApiCrud.Data/WebApiCrud.Data.csproj


**************************************************************
            Add NUGET Packages in WebApiCrud.Data
**************************************************************

$ dotnet add package Microsoft.EntityFrameworkCore

$ dotnet add package Microsoft.EntityFrameworkCore.Relational

$ dotnet add package Microsoft.EntityFrameworkCore.Design

$ dotnet add package Microsoft.EntityFrameworkCore.Tools

$ dotnet add package Microsoft.EntityFrameworkCore.Sqlite

