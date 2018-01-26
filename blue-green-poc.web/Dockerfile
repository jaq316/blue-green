FROM microsoft/aspnetcore:2.0
ARG source
WORKDIR /app
EXPOSE 80
ENV DEPLOYMENT_SLOT="red"
COPY ${source:-obj/Docker/publish} .
ENTRYPOINT ["dotnet", "blue-green-poc.web.dll"]
