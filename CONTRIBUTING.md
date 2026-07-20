# Contribuindo com o Develix Core

Obrigado por contribuir com o projeto.

Antes de implementar qualquer funcionalidade, leia:

- PHILOSOPHY.md
- ARCHITECTURE.md
- DECISIONS.md
- CODING_STANDARD.md
- TESTING.md

---

# Fluxo de desenvolvimento

Sempre seguir a sequência:

Planejamento

↓

Implementação

↓

Testes

↓

Refatoração

↓

Documentação

---

# Antes de programar

Pergunte:

Esta funcionalidade pode ser reutilizada por outro produto?

Se sim, ela pertence ao Core.

Caso contrário, pertence à aplicação.

---

# Testes

Toda classe pública deve possuir testes.

Novas funcionalidades não devem ser implementadas sem cobertura mínima adequada.

---

# Pull Requests

Um Pull Request deve possuir apenas um objetivo.

Evite misturar várias funcionalidades.

---

# Commits

Mensagens curtas e objetivas.

Exemplos:

feat: add query builder count

fix: migration transaction

refactor: simplify router

test: add query builder insert

docs: update roadmap

---

# Código

Sempre seguir:

- PSR-4
- Tipagem
- Métodos pequenos
- Classes coesas

Evitar:

- duplicação
- código morto
- comentários desnecessários

---

# Dependências

Evite adicionar bibliotecas externas.

Antes de adicionar uma dependência, responda:

Ela realmente resolve um problema que não vale a pena implementar?

Ela reduz manutenção?

Ela será utilizada por vários produtos?

Caso contrário, prefira uma implementação própria.

---

# Documentação

Toda mudança relevante deve atualizar:

- ROADMAP.md
- DECISIONS.md
- AI_CONTEXT.md

quando necessário.

---

# Filosofia

O objetivo deste projeto não é apenas funcionar.

O objetivo é construir uma plataforma capaz de acelerar todos os futuros produtos da Develix.

Toda contribuição deve respeitar esse princípio.