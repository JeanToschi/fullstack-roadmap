# Etapa 11 — Testes e Docker

```text
Você está aqui:
[✓] 10 — Validações e erros
[→] 11 — Testes e Docker
[ ] 12 — Feature final
```

## 1. Objetivo da etapa

Proteger comportamentos essenciais com testes e executar aplicação e banco em um ambiente reproduzível com Docker Compose.

## 2. O que será aprendido

Arrange, Act, Assert; testes unitários e básicos de integração; mocks; image, container, Dockerfile, Compose, porta, volume e variável de ambiente.

## 3. Conceitos mínimos

Um teste descreve um comportamento: prepara dados (**Arrange**), executa uma ação (**Act**) e verifica o efeito observável (**Assert**). Mock substitui uma dependência quando o foco não é testá-la. Uma image é o pacote; um container é sua execução. Volume preserva dados e porta conecta host e container.

## 4. O que pesquisar

- documentação Jest: matchers, setup e mocks
- documentação NestJS: testing
- documentação Docker: Dockerfile e Compose
- “Docker volume PostgreSQL persistência”
- “healthcheck depends_on Docker Compose”

## 5. Tarefas práticas

### Testes

- `given` produto válido, `when` cadastrar, `then` persistir e retornar resultado;
- `given` produto inexistente, `when` buscar, `then` retornar `404`;
- validar preço, estoque, nome e categoria;
- testar ao menos um endpoint integrado com dependências controladas;
- demonstrar que um teste falha antes da correção de um bug e passa depois.

### Docker

- criar Dockerfile adequado à aplicação;
- configurar API e PostgreSQL no Compose;
- configurar portas, variáveis e volume sem segredos commitados;
- documentar inicialização, migração, parada e diagnóstico;
- executar o sistema com `docker compose up` e comprovar persistência após recriar a API.

### Critérios de aceite

- testes são determinísticos, legíveis e verificam comportamento, não detalhes triviais;
- falha informa qual regra quebrou;
- aplicação não depende de banco instalado diretamente na máquina;
- serviço espera o banco ficar utilizável de forma confiável;
- volume preserva dados e `.env.example` documenta variáveis sem valores secretos;
- uma pessoa consegue executar seguindo apenas o README.

## 6. Fluxo Git

Separe proteção de comportamentos e ambiente Docker em entregas revisáveis. Explique no PR o que o teste garante e quais comandos foram executados. Não misture refatorações amplas sem Issue.

## 7. Antes de abrir o PR

- [ ] Vi pelo menos um teste relevante falhar e depois passar
- [ ] Executei toda a suíte sem dependência de ordem
- [ ] Subi o ambiente a partir de estado limpo
- [ ] Testei persistência e instruções de outra pessoa
- [ ] Não incluí secrets nem arquivos gerados

## 8. Perguntas de revisão

- Identifique Arrange, Act e Assert em um teste.
- O mock substitui o quê e por que isso é adequado?
- Qual diferença entre image e container? Onde os dados persistem?
- Siga a variável de conexão do Compose até o backend.

## 9. Critério para avançar

- [ ] Escrevo testes unitários e um teste básico de integração
- [ ] Uso mocks com propósito explícito
- [ ] Diagnostico uma falha pelo nome e saída do teste
- [ ] Executo e explico o ambiente com Docker Compose

## 10. Retrospectiva

O que aprendi? O que ainda não faço sozinho? Onde precisei de ajuda? Qual erro mais me ensinou? O que consigo explicar hoje que não conseguia antes?

[Próxima etapa →](../12-feature-final/README.md)
