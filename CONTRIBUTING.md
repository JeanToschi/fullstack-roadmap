# Como contribuir

Este repositório usa o mesmo fluxo de uma equipe de desenvolvimento. Antes de começar, crie ou escolha uma Issue e mantenha cada alteração pequena e focada.

## Branches

Atualize a branch principal e crie uma branch descritiva:

```bash
git switch main
git pull
git switch -c feat/product-list
```

Use `feat/nome-da-feature`, `fix/nome-do-bug`, `refactor/nome` ou `docs/nome`. Use letras minúsculas, palavras em inglês quando fizer sentido e hífens.

## Commits

Use Conventional Commits de forma simples:

- `feat:` nova capacidade;
- `fix:` correção;
- `docs:` documentação;
- `refactor:` reorganização sem mudar comportamento;
- `test:` testes;
- `chore:` manutenção.

Exemplos: `feat: add product creation`, `fix: handle product not found` e `docs: update git instructions`.

Faça commits pequenos, com uma intenção clara. Antes de cada commit, execute `git status` e `git diff --staged`.

## Pull Requests

Um PR deve tratar de uma mudança pequena, sem alterações não relacionadas. Teste, revise o diff e preencha o template. Relacione a Issue usando `Closes #número` quando o PR resolver toda a tarefa.

Durante o review: leia o comentário inteiro; confirme que entendeu ou pergunte; altere e teste; responda explicando o que mudou; só resolva a conversa depois do entendimento comum.

Não resolva comentários sem entender e não faça merge do próprio PR sem a aprovação combinada com o mentor.
