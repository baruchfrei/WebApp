FROM microsoft/dotnet:latest
COPY . /app
WORKDIR /app

RUN ["dotnet", "restore"]
RUN ["dotnet", "build"]
 
EXPOSE 90/tcp
ENV ASPNETCORE_URLS http://*:90
 
ENTRYPOINT ["dotnet", "run"]






#FROM microsoft/dotnet:1.0.0-core


# Set the Working Directory
# WORKDIR /app

# Configure the listening port to 80
# ENV ASPNETCORE_URLS http://*:80
# EXPOSE 80

# Copy the app
# COPY . /app

# Start the app
# ENTRYPOINT dotnet WebApp.dll

# ARG CONTAINER_PORT=80
# ARG SERVER_URLS=http://*:$CONTAINER_PORT
# ENV SERVER.URLS $SERVER_URLS
# EXPOSE $CONTAINER_PORT

# ENTRYPOINT ["dnx", "-p", "project.json", "web"]

