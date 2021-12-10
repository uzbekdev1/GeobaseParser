# Geobase Parser

## Start application:

- Go to source folder (`cd .\src\`)
- Navigate to Web API (` cd .\GeobaseParser.Api\`)
- Install NuGet packages (`dotnet restore`)
- Build source (`dotnet build`)
- Run source (`dotnet run`)
- Open this `http://localhost:5000` link

## Build application:

- Go to source folder (`cd .\src\`)
- Navigate to Web API (` cd .\GeobaseParser.Api\`)
- Publish API source (`dotnet publish`)
- Run application (`dotnet GeobaseParser.Api.dll --urls "http://localhost:5000"`)
- Open in this portal (`http://localhost:5000`)

## Test application:

- Go to source folder (`cd .\src\`)
- Navigate to Integration Test project (` cd .\GeobaseParser.IntegrationTest\`)
- run Test API layer (`dotnet test`)
- Navigate to Unit Test projet (` cd .\GeobaseParser.UnitTest\`)
- run Test Data acess layer (`dotnet test`)

## Containerize application:

- Build image (`docker -t demo-api build .`)
- Run image (`docker run demo-api`)
- Open in this portal (`http://localhost:5000`)

## Register image:

- Create new repo (`https://hub.docker.com/repositories`)
- Login hube (`docker login`)
- Tag image (`docker tag levdeo/demoapi levdeo/demoapi`)
- Push image (`docker push levdeo/demoapi`)
- Pull image (`docker pull levdeo/demoapi`)
- Run image (`docker run -it levdeo/demoapi`)
- Open in this portal (`http://localhost:5000`)

## Nginx balancer:

- Go to root (`cd .\nginx`)
- Build image (`docker-compose build`)
- Run image (`docker-compose up -d --scale api=10`)
- Open in this portal (`http://localhost:5000`) 