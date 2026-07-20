# AI Context

## Projeto

Develix Core

## Objetivo

O Develix Core é o núcleo tecnológico utilizado por todos os produtos da Develix.

Seu objetivo é acelerar a criação de novos sistemas, concentrando toda funcionalidade reutilizável em uma única biblioteca.

O Core nunca deve conter regras de negócio específicas de um produto.

---

## Stack

- PHP 8.3+
- Composer
- PHPUnit
- PSR-4
- MVC
- MySQL (inicialmente)

---

## Arquitetura

- MVC
- Query Builder próprio
- Active Record simplificado
- Router próprio
- CLI própria
- Migration própria
- Autoload via Composer

---

## Estado Atual

Implementado:

- Router
- CLI
- Migration
- Query Builder
- Gerador de Models
- Gerador de Controllers

Em desenvolvimento:

- ORM
- Model Base

Pendentes:

- Validation
- Authentication
- Authorization
- Sessions
- Upload
- Events
- Cache
- Mail
- Queue

---

## Filosofia

Toda decisão deve tornar o próximo produto da Develix mais rápido de ser desenvolvido.

Nenhuma decisão deve favorecer apenas um sistema específico.

Sempre priorizar simplicidade, legibilidade e independência de bibliotecas externas.