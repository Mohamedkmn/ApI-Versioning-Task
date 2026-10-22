# Task 1 — Implement API Versioning

A simple ASP.NET Core Web API example demonstrating URL-based API versioning.

## Requirements

- .NET 8 SDK
- ASP.NET Core Web API project

## Install packages

Run these commands in the project directory:

```powershell
dotnet add package Asp.Versioning.Mvc
dotnet add package Asp.Versioning.Mvc.ApiExplorer
dotnet add package Swashbuckle.AspNetCore
```

## Add the files

1. Replace the contents of `Program.cs` with the `Program.cs` included here.
2. Add `Controllers/ProductsController.cs` to your project.
3. If your project uses a different namespace, update the namespace in `ProductsController.cs`.

## Test the endpoints

### Version 1

`GET /api/v1/products`

```json
{
  "id": 1,
  "name": "Laptop",
  "price": 25000
}
```

### Version 2

`GET /api/v2/products`

```json
{
  "id": 1,
  "name": "Laptop",
  "price": 25000,
  "categoryName": "Electronics"
}
```

Version 1 keeps its original response, while version 2 adds `categoryName`.

## Notes

This archive contains the two source files and instructions; it is not a complete `.csproj` project. Add the files to your existing ASP.NET Core Web API project.
