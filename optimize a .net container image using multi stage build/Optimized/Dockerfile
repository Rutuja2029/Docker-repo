FROM mcr.microsoft.com/dotnet/sdk:6.0 AS build
WORKDIR /src
COPY BrezyWeather.csproj .
RUN dotnet restore BrezyWeather.csproj
COPY . .
RUN dotnet publish BrezyWeather.csproj -c Release -o /app

FROM mcr.microsoft.com/dotnet/sdk:6.0 AS final
WORKDIR /app
ENV ASPNETCORE_URLS=http://+:80/
EXPOSE 80
COPY --from=build /app .
ENTRYPOINT ["dotnet", "BrezyWeather.dll"]

