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

## Application Lifecycle

A classe `Application` é responsável por orquestrar o ciclo de vida da aplicação.

O ciclo ocorre em duas fases:

1. Register
2. Boot

Durante a fase de register todos os Service Providers registram seus serviços no Container.

Somente após todos os providers terem sido registrados é iniciada a fase de boot.

Isso garante que qualquer provider possa depender de serviços registrados por outro provider.

Após a aplicação ser inicializada (`boot()`), qualquer provider registrado posteriormente será automaticamente inicializado.

## Sistema de Views

O Develix Core fornece uma camada simples de renderização baseada em arquivos PHP.

As views, layouts e componentes pertencem à aplicação consumidora, e não ao Core.

Estrutura esperada na aplicação:

```text
app/
├── Components/
├── Layouts/
└── Views/
```