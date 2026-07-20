# Arquitetura

## Princípio Principal

Se pode ser reutilizado por outro produto, pertence ao Core.

Se atende apenas um produto, pertence à aplicação.

---

## Core

Responsável por:

- Router
- Controller Base
- Model Base
- Database
- Query Builder
- ORM
- Validation
- Authentication
- Authorization
- Sessions
- Upload
- Helpers
- Logs
- CLI
- Migrations
- Components
- Layouts

---

## Nunca colocar no Core

- Cadastro de Clientes
- Produtos
- Pedidos
- Financeiro
- Estoque
- Agenda
- Qualquer regra de negócio específica

---

## Dependências

Evitar dependências externas sempre que possível.

Criar soluções próprias quando o custo de manutenção justificar.

Bibliotecas externas somente quando realmente agregarem valor.