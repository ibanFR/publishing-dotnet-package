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

## Create a NuGet.org account

To publish packages to NuGet.org, you need to create an account on the NuGet website: [https://www.nuget.org/users/account/LogOn](https://www.nuget.org/users/account/LogOn).

See instructions in https://learn.microsoft.com/en-us/nuget/nuget-org/individual-accounts#add-a-new-individual-account.

To create a NuGet.org account, you need to have a personal Microsoft account (MSA). If you don't have one, you can 
create it in the following site https://signup.live.com/.

NuGet.org requires all accounts to have two-factor authentication (2FA) enabled on your MSA account. See instructions in
https://support.microsoft.com/account-billing/turning-two-step-verification-on-or-off-for-your-microsoft-account-b1a56fc2-caf3-a5a1-f7e3-4309e99987ca

## Run the packaging command

To create the NuGet package, run the dotnet pack command, which also builds the project automatically.

```shell
dotnet pack
```
  

[Create and publish a package with the dotnet CLI]: https://learn.microsoft.com/en-us/nuget/quickstart/create-and-publish-a-package-using-the-dotnet-cli