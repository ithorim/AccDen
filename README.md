# AccDen 

_**AccDen**_ project consists of 2 applications that together form a software solution designed to facilitate the planning and delegation of tasks across various projects.
Project uses Angular and ASPT.NET

## Required installations for running the applications in a development environment

### Angular
- Node.js `20.X.X`
- Angular CLI `17.X.X`

### ASP.NET
- .NET 8.0
- Visual Studio Code

### Db
- SQlite (can easily adjust to use any other db)

## Setting up the project to run in a development environment

- Clone or download the repository

### Running the applications

- **Angular**, In the /src/frontend/ directory, run the application using AngularCLI by typing `ng serve` in the terminal.
- **.NET**, In the /src/backend/ directory, run the application using DotNetCLI by typing `dotnet watch --no-hot-reload in the terminal`.

## Ports
- 5001 - Backend
- 4200 - Frontend

## Publishing the project
- Change the enviroment variables
- Run `ng build --configuration production` to build the angular files
- Enable the use of static files in Program.cs
- Move files from wwwroot/browser to wwwroot in backend folder
- Run `dotnet publish --output Your\Desired\Location`
- Copy files to the server (e.g. using scp via ssh)
- Run the app on the server using `nohup dotnet backend.dll --urls "http://your.desired.url" &`
