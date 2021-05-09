# VitrineMvc
Aplicação MVC para o back-office de cadastro de produtos e fornecedores

Desenvolvida em .NET Core 3.1 e utiliza EF Core para acesso a dados.

Funcionalidades:
* Tem extensões para exibir nossa moeda localizada
* Formatação automática de CPF / CNPJ
* Form modal para editar dados, que atualiza partial view
* Função JS para buscar dados do logradouro ao se digitar o CEP
* Tradução da maioria das mensagens de erro
* Uso do container próprio de injeção de dependências

Para executar o projeto faça as migrações antes:

1. No Visual Studio (Package Manager Console)
```
    Add-Migration InitialCreate
    Update-Database
```
    
2. No VS Code (CMD, Powershell, Terminal)
* Instale o Entity Framework Core tools reference - .NET Core CLI (caso não tenha):
```
    dotnet tool install --global dotnet-ef
```
```
    dotnet-ef migrations add InitialCreate
    dotnet ef database update
```
