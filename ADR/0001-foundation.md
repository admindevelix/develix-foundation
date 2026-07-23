# ADR 0001 - Criação do Develix Foundation

## Status

Accepted

---

## Contexto

A Develix tem como objetivo construir soluções digitais para resolver problemas complexos de pequenas e médias empresas utilizando uma plataforma tecnológica própria.

À medida que novos produtos são desenvolvidos, aumenta o risco de decisões arquiteturais divergentes, perda de conhecimento técnico, duplicação de soluções e inconsistências entre projetos.

Era necessário estabelecer um repositório independente responsável por concentrar a visão da empresa, os princípios arquiteturais, os padrões de desenvolvimento e o histórico das decisões técnicas.

---

## Decisão

Foi criado o repositório **develix-foundation** como a fonte oficial de verdade para toda a plataforma Develix.

Este repositório passa a concentrar toda a documentação institucional e arquitetural da empresa, incluindo:

* Manifesto
* Filosofia
* Arquitetura
* Padrões
* Roadmap
* Convenções de código
* Estratégias de testes
* Processo de contribuição
* Contexto para IA
* Architecture Decision Records (ADR)

Todos os projetos da Develix deverão seguir as diretrizes definidas neste repositório antes da implementação de qualquer funcionalidade.

O **develix-foundation** não contém código-fonte de produtos.

Seu objetivo é definir princípios, regras e decisões que orientam o desenvolvimento de toda a plataforma.

---

## Consequências

### Positivas

* Centralização do conhecimento arquitetural.
* Padronização entre todos os produtos.
* Facilidade de onboarding de novos desenvolvedores.
* Preservação do histórico das decisões.
* Menor acoplamento entre documentação e implementação.
* Evolução consistente da plataforma.

### Negativas

* Exige disciplina para manter a documentação atualizada.
* Algumas decisões precisarão ser formalizadas antes da implementação.

---

## Alternativas Consideradas

### Documentação dentro do Core

Rejeitada.

Misturaria arquitetura da empresa com implementação de um único projeto.

---

### Documentação distribuída entre os projetos

Rejeitada.

Geraria divergências e perda de consistência ao longo do tempo.

---

## Impacto na Plataforma

Esta decisão:

* aumenta a reutilização de conhecimento;
* aumenta a modularidade organizacional;
* reduz inconsistências entre projetos;
* facilita a criação de novos produtos;
* estabelece uma única fonte de verdade para decisões arquiteturais;
* está alinhada ao Manifesto e à Filosofia da Develix.

---

## Observações

Sempre que uma decisão arquitetural permanente for tomada, deverá ser registrada por meio de uma nova ADR neste repositório.

O código implementa as decisões.

O Foundation preserva as decisões.
