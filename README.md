# Docker .NET7 - Scaffold
Um script de criação de projeto AspNet Core 7 e Docker, sem uso de Dockerfile ou docker-compose.

# API-NET7-Docker

```CSharp
// Criar o projeto:
dotnet new mvc -n "App"

// Instalar o pacote Build Containers: 
dotnet add package Microsoft.NET.Build.Containers

// Criar a imagem:
dotnet publish --os linux --arch x64 -p:PublishProfile=DefaultContainer

// Rodar o contaienr:
docker run -it --rm -p 9750:80 appdocker:1.0.0
```

