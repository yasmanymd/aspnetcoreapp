FROM mcr.microsoft.com/dotnet/sdk:7.0 AS development
WORKDIR /app

# Copy the project file and restore any dependencies (use .csproj for the project name)
COPY *.csproj ./
RUN dotnet restore

#Important: --no-launch-profile because it is avoiding read the launchSettings.json
CMD dotnet watch run --no-launch-profile