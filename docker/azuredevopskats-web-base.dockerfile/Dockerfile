# Build Stage
FROM mcr.microsoft.com/dotnet/sdk:5.0.403

RUN apt-get update && apt-get install -y \
    tree \
    && rm -rf /var/lib/apt/lists/*

COPY .  /app
WORKDIR /app

RUN dotnet restore
