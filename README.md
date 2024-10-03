# História: Sistema de Cadastro de Produtos

## 💭 Sobre o desafio

A DompixelShop deseja criar uma aplicação web para gerenciar seu estoque de produtos e suas respectivas categorias. Como parte do processo de recrutamento, estamos avaliando desenvolvedores para integrar nossa equipe. Este desafio tem como objetivo avaliar suas habilidades de desenvolvimento.

### 🖥 Tecnologias

- Node.js (versão 18 ou superior)
- NestJS ou AdonisJS
- Banco de Dados (PostgreSQL ou MySQL)
- Docker

### ❗❗ Obrigatório

#### Requisitos Funcionais:

1. API de Produtos:
   - Deve permitir o cadastro de novos produtos com os seguintes campos:
      - Nome do produto (campo obrigatório)
      - Descrição do produto
      - Preço do produto (campo obrigatório)
      - Quantidade em estoque (campo obrigatório)
      - O produto deve estar vinculado a uma categoria.

2. CRUD de Produtos:
   - Criar: Adicionar novos produtos ao sistema.
   - Listar: Listar todos os produtos cadastrados, exibindo seus nomes, preços, quantidades em estoque e categoria associada.
     - Fazer a paginação de 10 produtos por página.
     - Implementar filtro pelo nome do produto.
   - Atualizar: Atualizar os dados de um produto já cadastrado.
   - Excluir: Remover produtos do sistema.
     - Implementar soft delete.

3. API de Categorias:
   - Deve permitir o cadastro de categorias de produtos com os seguintes campos:
     - Nome da categoria (campo obrigatório)

4. CRUD de Categorias:
   - Criar: Adicionar novas categorias ao sistema.
   - Listar: Listar todas as categorias cadastradas.
     - Fazer a paginação de 10 categorias por página.
     - Implementar filtro pelo nome da categoria.
   - Atualizar: Atualizar as informações de uma categoria.
   - Excluir: Remover categorias do sistema.
     - Implementar soft delete.

5. Versionamento do Banco de Dados:
   - O candidato deve utilizar migrations para criar a estrutura do banco de dados (tabelas de produtos e categorias, com as devidas relações).
   - Cada produto deve pertencer a uma única categoria.

6. Boas Práticas:
   - Código limpo e organizado.
   - Estrutura MVC, separando a lógica de negócios, controle e apresentação.
   - O código desenvolvido deve ser de fácil manutenção.

O candidato terá um prazo de 48 horas para entregar a solução desenvolvida, que será avaliada pela equipe técnica em relação à qualidade do código, cumprimento dos requisitos funcionais e organização da estrutura da aplicação.

### 📝 Readme do Repositório

- Deve conter o título do projeto
- Uma descrição do projeto
- Instruções de como executar o projeto de maneira detalhada e especifica
- Se durante o processo de desenvolvimento não conseguiu fazer algo, explique qual o impedimento que encontrou e como tentou resolver em uma seção "Dificuldades"
- Se possível deixar a collection do postman ou insomnia para testar as apis.

### 💯 Finalização

Ao finalizar o projeto, envie o link do repositório via e-mail para contato@dompixel.com.br

### 📞 Suporte
Caso tenha algum dúvida envie um e-mail para contato@dompixel.com.br