# Etapa 08 — Angular

```text
Você está aqui:
[✓] 07 — PostgreSQL
[→] 08 — Angular
[ ] 09 — Integração Full Stack
```

## 1. Objetivo da etapa

Construir as telas do catálogo em Angular com dados mockados, preparando contratos para a integração real.

## 2. O que será aprendido

HTML, CSS básico, component, template, property binding, event binding, service, routing e formulário.

## 3. Conceitos mínimos

Um component coordena estado e comportamento de uma parte da interface; o template descreve sua exibição. Property binding leva valores para a tela, event binding leva ações da tela ao código. Um service compartilha acesso a dados. Rotas relacionam URLs a telas.

## 4. O que pesquisar

- documentação Angular: components e templates
- “Angular property binding event binding”
- documentação Angular: routing
- documentação Angular: reactive forms
- “Angular service dependency injection”

## 5. Tarefas práticas

1. Criar layout simples e navegação principal.
2. Implementar `/products` com lista mockada e estado vazio.
3. Implementar `/products/:id` com detalhe e produto inexistente.
4. Implementar `/products/new` com formulário de cadastro.
5. Implementar `/products/:id/edit` reutilizando decisões do formulário.
6. Extrair acesso aos mocks para um service, sem chamar a API ainda.

### Critérios de aceite

- as quatro rotas abrem diretamente pela URL;
- lista identifica nome, preço, estoque, estado e categoria;
- formulário possui labels, navegação por teclado e ações claras;
- componentes não acessam diretamente o array mockado;
- layout funciona em largura estreita sem esconder ações essenciais;
- não há integração HTTP antecipada nesta etapa.

### Leitura e debug

Escolha o botão “Salvar” e siga: evento → método → service → atualização da tela. Depois reproduza uma rota com ID inexistente, use breakpoint no component e anote o valor recebido.

## 6. Fluxo Git

Organize as telas em Issues e PRs independentes. Defina o limite entre component e service e registre a decisão. Os critérios, não os nomes sugeridos, devem orientar sua branch.

## 7. Antes de abrir o PR

- [ ] Testei navegação, ações, estado vazio e ID inexistente
- [ ] Verifiquei a interface em duas larguras
- [ ] Componentes e service têm papéis claros
- [ ] Revisei o diff e arquivos gerados
- [ ] Sei explicar bindings e fluxo de um clique

## 8. Perguntas de revisão

- Qual diferença entre property binding e event binding?
- Onde a rota fornece o ID ao component?
- Por quais arquivos os dados mockados passam até a tela?
- O que aconteceria se o service fosse acessado diretamente pelo template?

## 9. Critério para avançar

- [ ] Crio component, rota, service e formulário básicos
- [ ] Explico a divisão entre template e classe
- [ ] Investigo eventos com breakpoint
- [ ] Demonstro as quatro telas com dados mockados

## 10. Retrospectiva

O que aprendi? O que ainda não faço sozinho? Onde precisei de ajuda? Qual erro mais me ensinou? O que consigo explicar hoje que não conseguia antes?

[Próxima etapa →](../09-integracao-fullstack/README.md)
