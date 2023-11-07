FROM mcr.microsoft.com/dotnet/sdk:7.0
WORKDIR /app

COPY . .

RUN dotnet restore
RUN dotnet publish -c release --self-contained false --no-restore -o ./publish .

CMD ["dotnet", "publish/Worker.dll"]

LABEL maintainer="DUBAIL Séraphin seraphin.dubail@supinfo.com" #"MAINTAINER" est considéré comme obsolète depuis Docker 1.13