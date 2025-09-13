# MS Ecommerce Platform

This repository contains the MS Ecommerce platform built with .NET.

## Prerequisites

- .NET 8.0 SDK or later (currently using .NET 8.0.119)
- Visual Studio 2022 17.8+ or Visual Studio Code with C# extension

> **Note:** This solution is configured to target .NET 8.0 but is designed to be easily upgraded to .NET 9.0 when available. To upgrade:
> 1. Update `global.json` to specify .NET 9.0 SDK version
> 2. Update `Directory.Build.props` to change `<TargetFramework>` from `net8.0` to `net9.0`

## Solution Structure

The solution `ms-ecommerce.sln` is currently empty and ready for development.

## Development Setup

1. Clone the repository
2. Ensure you have .NET 9.0 SDK installed
3. Run `dotnet restore` to restore NuGet packages
4. Run `dotnet build` to build the solution

## Code Standards

This project uses EditorConfig for consistent code formatting and follows .NET best practices:

- Nullable reference types enabled
- Implicit usings enabled
- Latest C# language version
- Code analysis enabled with recommended rules
- Treat warnings as errors in builds

## Getting Started

To add new projects to the solution:

```bash
# Create a new project
dotnet new <template> -n <ProjectName>

# Add to solution
dotnet sln ms-ecommerce.sln add <ProjectName>/<ProjectName>.csproj
```