# Fullstack Job Test - Back-End: PHP/NodeJs, MySQL & ReactJS/Vue

## Desafio

O objetivo é  criar uma aplicação onde usuários possam cadastrar produtos novos em um banco de dados, listar os produtos cadastrados e também possam editar ou excluir produtos existentes.
 
### Obrigatório

- O projeto deve ter um repositório público no github
- A parte do frontend deve ser feito em React ou então em Vue
- A parte do backend pode ser feito em PHP ou então em Node
  - Caso seja feito em PHP deve ser utilizado o laravel com versão superior ao 5.6
  - Caso seja feito em Node deve ser utilizado o express ou então o Adonis
- Os produtos disponíveis no projeto Front-End React devem ser recuperados através da API Rest Back-End PHP;
- Fique atento a princípios SOLID, DDD e orientação a objetos;
 
## API / Back-End PHP/Node
 
 ### Banco de Dados
 
 - Utilize Migrations
 - Tabelas e colunas do banco em inglês e utilizar snake case
 
 ### Endpoints
 
- Criar uma API REST usando PHP/Node com os seguintes endpoints:
      
     `GET /`: Retornar um Status: 200 e uma Mensagem "REST WebAPI Challenge 20200908 Running"
     
     `POST /products`: O endpoint servirá para inserir novos dados na tabela de produtos que serão enviados pelo frontend, que serão: nome, categoria e preço
     
     `PUT /products/:productId`: Será responsável por receber atualizações de um produto especifico enviados pelo frontend
     
     `DELETE /products/:productId`: Remover o produto da base de dados
     
     `GET /products/:productId`: Obter a informação somente de um produto da base de dados
     
     `GET /products`: Listar todos os produtos da base de dados
 
 - Integrar a API com o banco de dados para persistir os dados
 - Até o momento, os Endpoints estão todos abertos para acesso. Isso não é legal a nível de segurança, dessa forma, queremos que você use um esquema para bloquear qualquer tipo de acesso não autorizado.
 
 > Dica: Talvez seja interessante utilizar uma chave api no header das requisições
 
### Extras

- **Diferencial 1 -** Utilizar typescript caso utilize o Node
- **Diferencial 2 -** Escrever Unit Test para o endpoint `POST /products`
- **Diferencial 3 -** Executar o projeto usando Docker
- **Diferencial 4 -** Escrever o esquema de segurança aplicado nos endpoints
- **Diferencial 5 -** Escrever uma documentação para a API
 
## Front-End React/Vue

Nessa parte da aplição foi criado um figma para servir de material de apoio:

- [Figma](https://www.figma.com/file/RvniDEVlsA0kBMV8eSf57M/Fullstack-Job-Test?node-id=0%3A1)

### Criação de produto
 
Seu objetivo é montar uma tela para a criação de produtos novos no banco de dados. 
Nesta tela devemos adicionar os seguintes campos:

        - Nome (obrigatório)
        - Categoria (obrigatório)
        - Preço (obrigatório)
    
É necessário que o frontend faça a validação dos campos antes de serem enviados a REST API. 

O Product Manager do projeto deixou uma sugestão abaixo.

> Recomendado adicionar alertas de validações, sucesso e erro.

 
#### Listar produtos
 
Criar uma tela com uma tabela para listar os produtos processados pela API. É importante ter os seguintes campos:
 
        - Nome
        - Categoria
        - Preço
        - Data de criação (Data do upload do produto)
        - Ações (Botões Editar e Excluir)
 
#### Editar produto
 
Ao clicar no botão de editar na tabela de produtos, o usuário deverá ir para uma tela de edição do produto com os campos dos produtos para que seja possível editá-los com os seguintes campos:

        - Nome
        - Categoria
        - Preço
        
É necessário que o frontend faça a validação dos campos antes de serem enviados a REST API. 

O Product Manager do projeto deixou uma sugestão abaixo.

> Recomendado adicionar alertas de validações, sucesso e erro.

#### Remover produto
 
Antes de completar a ação de remover produto, devemos perguntar ao usuário se ele realmente quer realizar a ação. Para evitar a remoção de produtos de maneira indesejada. 
Após remover com êxito, notificar o usuário com um alerta de sucesso. 

#### Unit Testing
 
- **Diferencial 1 - Foco em Front-End** utilizar Unit Test no front-end para a opção de `Remover produto`. 
- **Diferencial 2 - Foco em Front-End** utilizar Unit Test no front-end para a opção de `Editar produto`. 
 
## Readme do Repositório
 
- Deve conter o título do projeto
- Uma descrição do projeto
- Instruções de como executar o projeto de maneira detalhada e especifica de cada parte (frontend e backend)
- Se durante o processo de desenvolvimento não conseguiu fazer algo, explique qual o impedimento que encontrou e como tentou resolver em uma seção "Dificuldades"

## Finalização 

Ao finalizar o projeto, envie o link do repositório via e-mail para contato@dompixel.com.br

## Suporte

Caso tenha algum dúvida envie um e-mail para contato@dompixel.com.br 
