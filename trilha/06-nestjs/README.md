# Etapa 06 — NestJS

```text
Você está aqui:
[✓] 05 — HTTP e API REST
[→] 06 — NestJS
[ ] 07 — PostgreSQL
```

## 1. Objetivo da etapa

Migrar a API de produtos para NestJS, preservando comportamentos e separando entrada HTTP das regras de negócio.

## 2. O que será aprendido

Module, controller, service, DTO, injeção de dependência e separação de responsabilidades.

## 3. Conceitos mínimos

```text
Request → Controller → Service → dados
                    ← resultado ←
```

O module reúne partes da funcionalidade. O controller traduz HTTP para chamadas. O service concentra operações e regras. O DTO descreve os dados recebidos. A injeção de dependência fornece o service sem o controller precisar construí-lo.

## 4. O que pesquisar

- “NestJS modules controllers providers documentação”
- “dependency injection NestJS”
- “DTO NestJS TypeScript”
- “NestJS route params body status code”

## 5. Tarefas práticas

1. Gerar a aplicação mínima e confirmar a inicialização.
2. Criar `ProductsModule` e conectá-lo ao módulo principal.
3. Criar `ProductsService` e mover para ele o CRUD em memória.
4. Criar `ProductsController` com os cinco endpoints.
5. Criar DTOs de cadastro e atualização, sem ainda antecipar validações avançadas.
6. Comparar respostas com a coleção da etapa anterior e corrigir regressões.

### Critérios de aceite

- módulo, controller e service têm responsabilidades distintas;
- controller recebe dados e delega regras ao service;
- DTOs não contêm persistência nem acesso HTTP;
- endpoints mantêm contratos e status definidos na etapa 05;
- coleção anterior evidencia que não houve regressão.

### Pistas graduais

<details><summary>💡 Pista 1</summary>Comece pelo diagrama e localize uma classe para cada caixa.</details>

<details><summary>💡 Pista 2</summary>Se o controller manipula diretamente o array, a responsabilidade ainda não foi movida.</details>

## 6. Fluxo Git

Proponha uma sequência de PRs que deixe a aplicação executável ao fim de cada um. Use branches por responsabilidade, não um único PR para toda a migração.

## 7. Antes de abrir o PR

- [ ] A aplicação inicia sem erros
- [ ] Rodei todas as requisições de regressão
- [ ] Controller e service não duplicam regras
- [ ] Revisei imports, arquivos gerados e diff
- [ ] Consigo explicar como o service chega ao controller

## 8. Perguntas de revisão

- Qual responsabilidade pertence ao controller e qual ao service?
- Quem cria a instância do service?
- De onde o DTO recebe dados e quem o consome?
- Remova mentalmente o `ProductsModule`: o que deixa de funcionar e por quê?

## 9. Critério para avançar

- [ ] Crio e conecto módulo, controller e service
- [ ] Explico injeção de dependência com o código aberto
- [ ] Preservo o contrato HTTP durante uma reorganização
- [ ] Leio o fluxo request → controller → service → resposta

## 10. Retrospectiva

O que aprendi? O que ainda não faço sozinho? Onde precisei de ajuda? Qual erro mais me ensinou? O que consigo explicar hoje que não conseguia antes?

[Próxima etapa →](../07-postgresql/README.md)
