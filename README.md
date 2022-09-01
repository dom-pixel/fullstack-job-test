# Fullstack Job Test - DomPixel

## 💭 Sobre o desafio

O objetivo é  criar uma aplicação onde usuários possam cadastrar produtos novos em um banco de dados, listar os produtos cadastrados e também possam editar ou excluir produtos existentes.
 
### ❗❗ Obrigatório

- O projeto deve ter um repositório público com readme no github;
- A parte do frontend deve ser feito em Vue;
- A parte do backend tem que ser feito em PHP utilizando o framework LARAVEL com versão superior ao 8;
- Os produtos disponíveis no projeto Front-End React devem ser recuperados através da API Rest Back-End;
- Fique atento a princípios SOLID, DDD e orientação a objetos;
 
### 📝 Readme do Repositório
 
- Deve conter o título do projeto
- Uma descrição do projeto
- Instruções de como executar o projeto de maneira detalhada e especifica de cada parte (frontend e backend)
- Se durante o processo de desenvolvimento não conseguiu fazer algo, explique qual o impedimento que encontrou e como tentou resolver em uma seção "Dificuldades"

### 💯 Finalização

Ao finalizar o projeto, envie o link do repositório via e-mail para contato@dompixel.com.br

### 🤔 Suporte

Caso tenha algum dúvida envie um e-mail para contato@dompixel.com.br

## 👾 Back-End PHP LARAVEL

### 📚 Banco de Dados
 
 - Utilize Migrations
 - Tabelas e colunas do banco em inglês e utilizar snake case
 - Nesse teste temos apenas uma tabela de produtos que deve conter:
   - ID
   - Nome
   - Categoria
   - Preço
   - Data de criação

### ✅ Endpoints
 
- Criar uma API REST usando PHP (LARAVEL) com os seguintes endpoints:
      
     `GET /`: Retornar um Status: 200 e uma Mensagem "API Fullstack Job Test - DomPixel running"
     
     `POST /products`: O endpoint servirá para inserir novos dados na tabela de produtos que serão enviados pelo frontend, que serão: nome, categoria e preço
     
     `PUT /products/:productId`: Será responsável por receber atualizações de um produto especifico enviados pelo frontend
     
     `DELETE /products/:productId`: Remover o produto da base de dados
     
     `GET /products/:productId`: Obter a informação somente de um produto da base de dados
     
     `GET /products`: Listar todos os produtos da base de dados
 
 - Integrar a API com o banco de dados para persistir os dados
 - Até o momento, os Endpoints estão todos abertos para acesso. Isso não é legal a nível de segurança, dessa forma, queremos que você use um esquema para bloquear qualquer tipo de acesso não autorizado.
 
 > Dica: Talvez seja interessante utilizar uma chave api no header das requisições
 
### 🎯 Extras

- **Diferencial 1 -** Escrever Unit Test para o endpoint `POST /products`
- **Diferencial 2 -** Executar o projeto usando Docker
- **Diferencial 3 -** Escrever o esquema de segurança aplicado nos endpoints
- **Diferencial 4 -** Escrever uma documentação para a API
 
## 🌐 Front-End Vue

Nessa parte da aplição foi criado um figma para servir de material de apoio:

- [Figma](https://www.figma.com/file/RvniDEVlsA0kBMV8eSf57M/Fullstack-Job-Test?node-id=0%3A1)

> Obs: O Figma é apenas um exemplo de como devem ser as estruturas das telas, o frontend não precisa ser feito de maneira idêntica.

### 🆕 Criação de produto
 
Seu objetivo é montar uma tela para a criação de produtos novos no banco de dados. 
Nesta tela devemos adicionar os seguintes campos:

        - Nome (obrigatório)
        - Categoria (obrigatório)
        - Preço (obrigatório)
    
É necessário que o frontend faça a validação dos campos antes de serem enviados a REST API. 

O Product Manager do projeto deixou uma sugestão abaixo.

> Recomendado adicionar alertas de validações, sucesso e erro.

 
#### 📄 Listar produtos
 
Criar uma tela com uma tabela para listar os produtos processados pela API. É importante ter os seguintes campos:
 
        - Nome
        - Categoria
        - Preço
        - Data de criação (Data do upload do produto)
        - Ações (Botões Editar e Excluir)
 
#### 📝 Editar produto
 
Ao clicar no botão de editar na tabela de produtos, o usuário deverá ir para uma tela de edição do produto com os campos dos produtos para que seja possível editá-los com os seguintes campos:

        - Nome
        - Categoria
        - Preço
        
É necessário que o frontend faça a validação dos campos antes de serem enviados a REST API. 

O Product Manager do projeto deixou uma sugestão abaixo.

> Recomendado adicionar alertas de validações, sucesso e erro.

#### ❌ Remover produto
 
Antes de completar a ação de remover produto, devemos perguntar ao usuário se ele realmente quer realizar a ação. Para evitar a remoção de produtos de maneira indesejada. 
Após remover com êxito, notificar o usuário com um alerta de sucesso. 

### 🎯 Extras
 
- **Diferencial 1 - Foco em Front-End** utilizar Unit Test no front-end para a opção de `Remover produto`. 
- **Diferencial 2 - Foco em Front-End** utilizar Unit Test no front-end para a opção de `Editar produto`. 

---

<sup> Feito com 💙 pelos artesões da web da 👾<a href="https://dompixel.com.br/" target="_blank" rel="noopener">DomPixel</a> ® 2022.</sup>
