#AWS Lambda com CLI do .NET Core

### download dos templates lambda
dotnet new --install Amazon.Lambda.Templates

### cria uma nova função lambda para desenvolver
dotnet new lambda.EmptyFunction --name ExemploFuncaoLambda

### Instala tool lambda para dotnet
dotnet tool install -g Amazon.Lambda.Tools

### Deploy função lambda vida dot net
dotnet lambda deploy-function FuncaoExemplo --function-role lambda-role

### Invoka função para teste via dot net
dotnet lambda invoke-function FuncaoExemplo --payload "01001000"

### Deleta a função via dot net
dotnet lambda delete-function FuncaoExemplo
