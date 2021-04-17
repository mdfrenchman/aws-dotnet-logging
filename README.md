# aws-dotnet-logging
 demo of Logging in a .NET Core WebApi as a Lamda Function 

## Dev Environment
 - OS: Windows 10
 - Editor: VSCode
 - Terminal: Powershell
 - Git management: Github Desktop
 
## Initial Setup Steps
1. Install Lambda Template Nuget package `dotnet new -i Amazon.Lambda.Templates`
2. Dry Run Adding a Lambda Asp.Net Core Web Api project `dotnet new serverless.AspNetCoreWebApi -n serverless-logging-example --dry-run`.
 - `--dry-run` allows us to make sure we're running in the right directory and we like the naming of what's going to be created.
 - `-n` is for the name of our project.
3. Install the dotnet Lambda Tools `dotnet tool install -g Amazon.Lambda.Tools`
4. Run Tests to make sure things initialized correctly (and really just for the satisfaction of a successful test)
 - `cd ".\serverless-logging-example\test\serverless-logging-example.Tests\"`
 - `dotnet test`