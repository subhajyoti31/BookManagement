# Bookmanagement


dotnet tool install --global dotnet-ef

dotnet new mvc -n "BookManagement" -lang "C#" -au none

dotnet build

dotnet add package Microsoft.EntityFrameworkCore

dotnet add package Microsoft.EntityFrameworkCore.SqlServer

dotnet add package Microsoft.EntityFrameworkCore.Design

dotnet build

dotnet run

docker build -t bookmanagement .

docker run -p 8080:80 bookmanagement  

dotnet build

dotnet ef migrations add "Initial migration"

docker-compose up --build
