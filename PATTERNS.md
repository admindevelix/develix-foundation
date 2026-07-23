# Develix Design Patterns

## Objetivo

Este documento define os padrões oficiais utilizados nos projetos da Develix.

Um padrão somente passa a fazer parte deste documento após validação e adoção oficial. Isso garante consistência entre todos os produtos da plataforma.

---

# Arquitetura

## MVC

Responsável pela separação entre apresentação, domínio e acesso a dados.

Utilização obrigatória em aplicações web.

---

## Repository

Responsável exclusivamente pelo acesso aos dados.

Nunca deve conter regras de negócio.

---

## Service

Responsável por concentrar regras de negócio.

Controllers devem delegar processamento para Services.

---

## Dependency Injection

Dependências devem ser recebidas por construtor sempre que possível.

Evitar instanciações diretas dentro das classes.

---

# Objetos

## Entity

Representa um objeto persistente do domínio.

---

## DTO (Data Transfer Object)

Utilizado para transporte de dados entre camadas.

Não deve conter regras de negócio.

---

## Value Object

Representa valores imutáveis.

Dois Value Objects com o mesmo conteúdo são considerados iguais.

---

## Collection

Representa conjuntos tipados de objetos do domínio.

---

# Criação

## Factory

Responsável pela criação de objetos complexos.

---

## Builder

Responsável pela construção gradual de objetos.

---

# Comportamentais

## Command

Representa uma ação executável.

Cada Command deve possuir uma única responsabilidade.

---

## Strategy

Permite trocar algoritmos sem alterar o consumidor.

---

## Observer

Utilizado para comunicação desacoplada entre componentes.

---

## Event

Eventos representam fatos ocorridos no sistema.

Nunca devem conter regras de negócio.

---

# Infraestrutura

## Middleware

Executa processamento antes ou depois da requisição.

---

## Adapter

Responsável por integrar sistemas externos.

---

## Driver

Abstrai implementações específicas de infraestrutura.

---

## Cache

Responsável por armazenamento temporário de dados.

Nunca deve ser acessado diretamente pelo domínio.

---

# Evolução

Novos padrões devem ser documentados neste arquivo antes de serem adotados oficialmente nos projetos da Develix.
