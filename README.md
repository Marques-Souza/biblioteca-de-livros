# EmprestimoLivroFrontend

Este projeto foi gerado com o Angular CLI versão 17.3.11. Ele é a parte frontend de um sistema de Empréstimo de Livros, que se comunica com uma API .NET para gerenciar dados de empréstimos, livros e clientes (usuários).

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.


## Configuração da API
Este projeto depende de uma API .NET para funcionar corretamente. Para garantir que o frontend se conecte corretamente com a API, siga os passos abaixo:

1. Configure a URL da API
No arquivo de ambiente src/environments/environment.ts (para desenvolvimento) ou src/environments/environment.prod.ts (para production), defina a URL base da API. Exemplo:

export const environment = {
  production: false,
  apiUrl: 'http://localhost:5000/api'};

2. Verifique a API Backend
Certifique-se de que a API .NET está rodando corretamente no servidor. Geralmente, a URL da API será algo como http://localhost:5000/, mas isso pode variar conforme a configuração da API.


3. Comunicação com a API
O frontend se comunica com a API utilizando o Angular HTTP Client. Exemplo de como buscar dados da API:
exemplo: private apiUrl = `${environment.apiUrl}/livros`;

4. Certifique-se de que a API está acessível
Se a API não estiver rodando ou não estiver acessível, o frontend não será capaz de fazer requisições para recuperar ou enviar dados. Verifique sempre se o backend está ativo e respondendo corretamente.

# Para rodar a API .NET localmente, use: dotnet run

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.
