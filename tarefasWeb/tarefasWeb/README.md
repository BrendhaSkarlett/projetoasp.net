# Tarefas Web

Este projeto é uma aplicação web desenvolvida em ASP.NET Core 8.0 que permite gerenciar tarefas. A aplicação oferece funcionalidades para cadastrar, editar e excluir tarefas, utilizando um banco de dados para armazenar as informações.

## Estrutura do Projeto

- **Controllers**
  - `TarefasController.cs`: Controlador responsável pelas operações CRUD (Criar, Ler, Atualizar, Excluir) para as tarefas.

- **Models**
  - `Tarefa.cs`: Define a entidade de tarefa, com propriedades como Id, Titulo, Descricao e Concluida.

- **Data**
  - `AppDbContext.cs`: Configuração do contexto do banco de dados, incluindo a definição do DbSet para a tabela de tarefas.

- **Views**
  - **Tarefas**
    - `Index.cshtml`: Exibe a lista de tarefas e links para criar, editar e excluir.
    - `Create.cshtml`: Formulário para criar uma nova tarefa.
    - `Edit.cshtml`: Formulário para editar uma tarefa existente.
    - `Delete.cshtml`: Confirmação para a exclusão de uma tarefa.

- **wwwroot**
  - **css**
    - `site.css`: Estilos para as views da aplicação.

- **Configurações**
  - `appsettings.json`: Configurações da aplicação, incluindo a string de conexão com o banco de dados.
  - `Program.cs`: Ponto de entrada da aplicação, configurando serviços e pipeline de requisições.
  - `Startup.cs`: Configuração dos serviços e middleware da aplicação.

## Como Executar a Aplicação

1. Clone o repositório para sua máquina local.
2. Abra o terminal e navegue até o diretório do projeto.
3. Execute o comando `dotnet restore` para restaurar as dependências.
4. Configure a string de conexão no arquivo `appsettings.json` para apontar para seu banco de dados.
5. Execute o comando `dotnet run` para iniciar a aplicação.
6. Acesse a aplicação em `http://localhost:5000` no seu navegador.

## Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou pull requests.