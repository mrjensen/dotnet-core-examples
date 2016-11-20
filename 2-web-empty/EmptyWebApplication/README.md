# Empty Web Application
The project shows how a "Hello World" string is configured in the Startup.cs middleware.

# How to run
## Running on machine
```bash
dotnet restore
dotnet run

open http://localhost:5000
```

## Running in docker dotnet runtime container
```bash
dotnet restore
dotnet publish -c Production -o out
docker build -t 2-web-empty .
docker run -p 5000:5000 2-web-empty

open http://localhost:5000
```