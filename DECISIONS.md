# Decisões Técnicas

## ORM

Modelo híbrido.

Possui:

- Query Builder
- Active Record

Não utiliza:

- Doctrine
- Eloquent

---

## Testes

Toda classe pública deve possuir testes automatizados antes de receber novas funcionalidades.

---

## Banco

PDO.

Sem abstrações externas.

---

## Framework

Framework próprio.

---

## Arquitetura

MVC.

---

## Front-end

Bootstrap.

---

## Linguagem

PHP.

---

## Namespace

PSR-4.

---

## Versionamento

Git + GitHub.

## Provider Registration

Status: Accepted

Application registra providers utilizando o nome da classe.

Motivação:

- bootstrap mais limpo
- Application controla o ciclo de vida
- facilita descoberta automática
- evita instanciação manual
- reduz acoplamento

Consequências:

- providers devem possuir construtor padronizado
- Application passa a ser responsável pela criação dos providers


## ADR-0002

Título:
Core development is product-driven

Status:
Accepted

Context:
Inicialmente pretendíamos desenvolver um framework completo antes dos produtos.

Decision:
O Core passa a ser desenvolvido somente até o MVP necessário para iniciar um produto.

Consequences:
- menor tempo até o primeiro produto
- menos código morto
- menos abstrações desnecessárias
- arquitetura guiada por uso real

## Console

A composição dos comandos pertence ao bootstrap da aplicação.

O Core não instancia comandos automaticamente.

Cada aplicação (ex.: Develix Market) é responsável por registrar apenas os comandos que desejar disponibilizar.