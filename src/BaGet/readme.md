# BaGet

This is the project that implements [NuGet service APIs](https://docs.microsoft.com/en-us/nuget/api/overview). Today, only SQLite is supported. SQL Server will be added later. Most of the core logic is contained within the `BaGet.Core` project.

## Migrations

Regenerate migrations with:

```
rm baget.db
dotnet ef migrations remove
dotnet ef migrations add Initial

dotnet ef database update
```