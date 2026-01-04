# Sample repository for testing packaging and publishing .NET projects

This repository contains sample .NET projects that demonstrate how to package and publish .NET applications and
libraries.

It follows instructions from the Quickstart guide: [Create and publish a package with the dotnet CLI].

## Add package metadata to the project file

To create a NuGet package, you need to add specific metadata to your project file (`.csproj`). Here is an example of the necessary properties:

```xml
<PropertyGroup>
  <PackageId>Unique.Package.Identifier</PackageId>
  <Version>1.0.0</Version>
  <Authors>Your Name</Authors>
  <Company>Your Company</Company>
  <Description>This is a sample package for demonstration purposes.</Description>
</PropertyGroup>
```

## Run the packaging command

To create the NuGet package, run the dotnet pack command, which also builds the project automatically.

```shell
dotnet pack
```
  

[Create and publish a package with the dotnet CLI]: https://learn.microsoft.com/en-us/nuget/quickstart/create-and-publish-a-package-using-the-dotnet-cli