# Geobase Parser

# Start application:

- Go to source folder (`cd .\src\`)
- Navigate to Web project (` cd .\GeobaseParser.Web\`)
- Install NuGet packages (`dotnet restore`)
- Build source (`dotnet build`)
- Run source (`dotnet run`)
- Open this `http://localhost:5000` link
- Navigate `/swagger` part (`http://localhost:5000/swagger`)
- Go to root folder (`cd .\wwwroot\`)
- Navigate on client app (`cd .\ClientApp\`)
- Install npm packages (`npm install`)
- Build client app (`npm run-script build:dev`)
- Run client app (`npm run-script start`)
- Open in this portal `http://localhost:5001`

# Build application:

- Go to source folder (`cd .\src\`)
- Navigate to Web project (` cd .\GeobaseParser.Web\`)
- Publish API source (`dotnet publish`)
- Go to root folder (`cd .\wwwroot\`)
- Navigate to client app (`cd .\ClientApp\`)
- Production build app (`npm run-script build`)
- Copy the `dist` folder
- Back on publish directory (`cd ..\..\bin\Debug\net5.0\publish\`)
- Go to root folder (`cd .\wwwroot\`)
- Create `ClientApp` folder
- That created above the folder must be put in `dist` folder
- Back to publish directory (`cd ..\..\`)
- Run application (`dotnet GeobaseParser.Web.dll --urls "http://localhost:5000"`)
- Open in this portal `http://localhost:5000`
