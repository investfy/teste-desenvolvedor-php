# Teste para candidatos à vaga de Desenvolvedor PHP

Olá caro desenvolvedor, nesse teste analisaremos seu conhecimento geral e inclusive velocidade de desenvolvimento. Abaixo explicaremos tudo o que será necessário.

## Instruções

O desafio consiste em implementar uma aplicação web utilizando o framework PHP Laravel, e um banco de dados relacional SQLite, MySQL/MariaDB ou Postgres, a partir de uma modelagem de dados inicial desnormalizada, que deve ser normalizada para a implementação da solução.

Você vai criar uma aplicação de cadastro de pedidos de compra, a partir de uma modelagem inicial, com as seguintes funcionalidades:

1. CRUD de clientes.
1. CRUD de produtos.
1. CRUD de pedidos de compra, com status (Em Aberto, Pago ou Cancelado).
1. Cada CRUD:
    - deve ser filtrável e ordenável por qualquer campo, e possuir paginação de 20 itens.
    - deve possuir formulários para criação e atualização de seus itens.
    - deve permitir a remoção de qualquer item de sua lista.
1. Barra de navegação entre os CRUDs.
1. Links para os outros CRUDs nas listagens (Ex: link para o detalhe do cliente da compra na lista de pedidos de compra)

## Modelo de dados

A modelagem inicial para a implementar a solução é a seguinte:

**Pedido**
- Número do pedido
- Nome do cliente
- CPF
- E-mail
- Data do pedido
- Código de barras
- Nome do produto
- Valor unitário
- Quantidade

Você deve alterar esta modelagem para que a mesma cumpra com os três primeiros requisitos.

Além disso, a implementação deste modelo em um banco de dados relacional deve ser realizada levando em consideração os seguintes requisitos:

- O banco de dados deve ser criado utilizando [migrations](https://laravel.com/docs/migrations) do framework Laravel, e também utilizar [Seeds e Factories](https://laravel.com/docs/seeding) para popular as informações no banco de dados.
- Implementação das validações necessárias na camada que julgar melhor.

## Tecnologias a serem utilizadas

Devem ser utilizadas as seguintes tecnologias:

- Frameworks Laravel (PHP)
- Docker (construção do ambiente de desenvolvimento)
- Front-end básico com templates [Blade](https://laravel.com/docs/blade) *ou* PWA e comunicação via API REST.

## Entrega

- Para iniciar o teste, faça um fork deste repositório;
- Crie uma branch com o seu nome completo;
- Altere o arquivo teste.md com as informações necessárias para executar o seu teste (comandos, migrations, seeds, etc);
- Depois de finalizado, envie-nos o pull request.

## O que vamos avaliar

- Organização do código;
- Aplicação de design patterns;
- Testes;
- Separação de módulos e componentes;
- Legibilidade;
- Criação do ambiente com Docker;
- Documentação.

## Bônus

> Não são obrigatórios mas acrescentam muitos pontos ao seu teste:

- Implementar autenticação de usuário na aplicação.
- Permitir que o usuário mude o número de itens por página na paginação.
- Permitir remoção em massa de itens nos CRUDs.
- Implementar aplicação de desconto em alguns pedidos de compra.
- Implementar front-end responsivo para desktop, tablet e celular.
- Implementar a camada de front-end utilizando PWA com comunicação API REST.

**_Boa sorte!_**
