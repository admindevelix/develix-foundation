# Principles

## Simplicidade acima de tudo

A solução mais simples que atende corretamente aos requisitos deve ser preferida.

## Arquitetura orientada à extensibilidade

Novas funcionalidades devem ser adicionadas por extensão, e não por modificação do código existente, sempre que possível.

## Dependency Injection como padrão

Dependências devem ser resolvidas pelo Container, evitando instanciação manual.

## Application controla o ciclo de vida

A classe Application é responsável por orquestrar toda a inicialização do framework.

## Providers são registrados por classe

Service Providers são registrados pelo nome da classe.

A responsabilidade pela instanciação pertence exclusivamente à Application.

## Register antes de Boot

Todos os providers devem executar `register()` antes que qualquer provider execute `boot()`.

## Testes primeiro

Toda funcionalidade nova deve nascer acompanhada de testes automatizados.

## YAGNI

"You Aren't Gonna Need It"

Nenhum componente deve ser implementado apenas porque poderá ser útil futuramente.

Cada nova abstração deve resolver um problema existente.