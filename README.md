# Burger Queen - Back-end

## Índice

* [1. Burger Queen-API](#1-burger-queen-api)
* [2. Resumo do projeto](#2-resumo-do-projeto)
* [3. Como utilizar](#3-como-utilizar)
* [4. Endpoints](#4-endpoints)
* [5. Tecnologias usadas](#5-tecnologias-usadas)

***

## 1. Burger Queen API

O objetivo principal deste projeto foi a criação de uma API rest para uma Hamburgueria usar em um app no seu dia a dia.

## 2. Resumo do projeto

Este consiste no desenvolvimento de uma aplicação de servidor com enstrutura MVC (Model View Controller) que serve JSON através de uma conexão HTTP. A base de dados e os endpoints correspondem ao serviço da Hambugeria, com os produtos, criação de pedidos e relação de mesas e pedidos

A API rest é compatível com as requisições vindas do front a ser construído, foi desenvolvida a partir do Docker e possui testes de integração.

## 3. Como utilizar

A aplicação pode ser usada localmente, após a instalação de suas dependências, através do comando ``` docker compose up <ambiente> ``` (dev, db ou test), dentro da pasta do projeto ou pode ser acessada através do [link](https://bq-api-jackelinemattar.herokuapp.com/api) da api hospedada no Heroku.

ATENÇÃO: caso o ``` docker compose up <ambiente> ``` não rode a aplicação, talvez seja necessário o uso de ``` sudo docker compose up <ambiente> ```

## 4. Endpoints

#### `/products`

* `GET /products`
* `GET /products/:productid`
* `POST /products`
* `PUT /products/:productid`
* `DELETE /products/:productid`

#### `/orders`

* `GET /orders`
* `GET /orders/:orderid`
* `POST /orders`
* `PUT /orders/:orderid`
* `DELETE /orders/:orderid`

#### `/order-items`

* `GET /order-items`
* `GET /order-items/:orderitemid`
* `POST /order-items`
* `PUT /order-items/:orderitemid`
* `DELETE /order-items/:orderitemid`

#### `/tables`

* `GET /tables`
* `GET /tables/:tablenumber`
* `POST /tables`
* `PUT /tables/:tablenumber`
* `DELETE /tables/:tablenumber`

## 5. Tecnologias usadas

* Node.js
* Express
* Babel
* PostgreSQL
* Sequelize
* Postman
* DBeaver
* Docker
* Heroku
* Mocha
* Chai
* ESLint