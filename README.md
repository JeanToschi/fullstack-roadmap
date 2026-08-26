# Formação Full Stack: Sistema de Controle de Produtos

Uma trilha prática para quem está começando do zero e quer aprender a contribuir com segurança em aplicações reais. Você desenvolverá **um único sistema**, que começa no terminal e evolui até uma aplicação Full Stack executada com Docker.

Não é preciso conhecer programação, terminal ou Git. Comece por [Como usar esta trilha](docs/00-como-usar-esta-trilha.md), prepare o [ambiente](docs/01-configurando-o-ambiente.md) e siga as etapas em ordem.

## Como funciona

Cada atividade imita o fluxo de uma equipe:

```text
Problema → conceito mínimo → pesquisa → implementação → teste
        → Git → Pull Request → review → correção → merge
```

Git e GitHub fazem parte do treinamento desde a primeira mudança. Cada tarefa deve nascer em uma Issue, ser feita em uma branch pequena e terminar em um Pull Request revisado. Você avança quando consegue **fazer e explicar**, não apenas quando marca uma etapa como concluída.

## O projeto

O **Sistema de Controle de Produtos** amadurece junto com você: primeiro exibe mensagens, depois aplica regras de negócio, mantém um CRUD, vira uma API NestJS com PostgreSQL e ganha uma interface Angular. No fim, você entrega uma feature completa.

```text
Git/GitHub → Lógica → TypeScript → CRUD → API REST → NestJS
     → PostgreSQL → Angular → Full Stack → Validações
     → Testes → Docker → Feature real
```

Stack principal: TypeScript, Node.js, NestJS, PostgreSQL, Angular, Git, GitHub, Jest e Docker.

## Roadmap

| Etapa | Entrega no sistema | Autonomia |
|---|---|---|
| [01 — Primeiro Pull Request](trilha/01-primeiro-pull-request/README.md) | Nome, mensagem e versão no terminal | Muito guiada |
| [02 — Primeiros passos com programação](trilha/02-primeiros-passos-com-programacao/README.md) | Primeiras regras de produto | Muito guiada |
| [03 — Funções, arrays e objetos](trilha/03-funcoes-arrays-e-objetos/README.md) | Catálogo manipulável | Guiada |
| [04 — CRUD em memória](trilha/04-crud-em-memoria/README.md) | Cadastro completo em array | Intermediária |
| [05 — HTTP e API REST](trilha/05-http-e-api-rest/README.md) | CRUD exposto por endpoints | Intermediária |
| [06 — NestJS](trilha/06-nestjs/README.md) | API organizada em módulos | Intermediária |
| [07 — PostgreSQL](trilha/07-postgresql/README.md) | Persistência e categorias | Mais autônoma |
| [08 — Angular](trilha/08-angular/README.md) | Telas do catálogo | Mais autônoma |
| [09 — Integração Full Stack](trilha/09-integracao-fullstack/README.md) | Tela, API e banco conectados | Mais autônoma |
| [10 — Validações e erros](trilha/10-validacoes-e-erros/README.md) | Fluxos seguros e mensagens úteis | Profissional |
| [11 — Testes e Docker](trilha/11-testes-e-docker/README.md) | Testes e ambiente reproduzível | Profissional |
| [12 — Feature final](trilha/12-feature-final/README.md) | Gerenciamento de categorias | Profissional |

## Meu progresso

- [ ] 01 — Primeiro Pull Request
- [ ] 02 — Primeiros passos com programação
- [ ] 03 — Funções, arrays e objetos
- [ ] 04 — CRUD em memória
- [ ] 05 — HTTP e API REST
- [ ] 06 — NestJS
- [ ] 07 — PostgreSQL
- [ ] 08 — Angular
- [ ] 09 — Integração Full Stack
- [ ] 10 — Validações e erros
- [ ] 11 — Testes e Docker
- [ ] 12 — Feature final

Você pode copiar este checklist para uma Issue chamada `Meu progresso` e atualizá-la. Assim, o README continua igual para todos.

## Como saber quando avançar

Ao fim de cada etapa há um checkpoint. Avance somente se você consegue demonstrar os comportamentos pedidos, responder às perguntas de revisão e explicar as próprias decisões. Peça uma revisão ao mentor quando houver dúvida.

## Use IA para aprender, não para terceirizar

> IA pode ajudar a explicar, investigar erros e sugerir caminhos, mas você precisa conseguir explicar todo código que coloca em um Pull Request.

Peça pistas antes da solução, compare alternativas, use a IA para interpretar erros e revisar seu raciocínio. Leia e teste tudo. Nunca aceite código sem entender nem abra um PR que não consiga explicar.

Ruim: `Faça essa tarefa para mim.`

Melhor: `Estou tentando validar o estoque de um produto. Explique os conceitos necessários e dê uma pista, sem escrever a solução completa.`

Veja exemplos e limites em [Como usar IA para aprender](docs/08-como-usar-ia-para-aprender.md).

## Guias de apoio

- [Terminal básico](docs/02-terminal-basico.md)
- [Git e GitHub](docs/03-git-e-github.md)
- [Como trabalhar com Issues](docs/04-como-trabalhar-com-issues.md)
- [Como abrir um Pull Request](docs/05-como-abrir-um-pull-request.md)
- [Como receber code review](docs/06-como-receber-code-review.md)
- [Como pedir ajuda](docs/07-como-pedir-ajuda.md)
- [Como contribuir](CONTRIBUTING.md)

Não pule etapas e não copie soluções sem entendê-las. O objetivo é aprender a investigar e entregar mudanças pequenas com segurança.
