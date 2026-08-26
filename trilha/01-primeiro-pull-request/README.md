# Etapa 01 — Primeiro Pull Request

```text
Você está aqui:
[→] 01 — Primeiro Pull Request
[ ] 02 — Primeiros passos com programação
```

## 1. Objetivo da etapa

Concluir mudanças simples no sistema usando Issue, branch, commit, push, Pull Request, review e merge, mesmo sem experiência anterior.

## 2. O que será aprendido

Repositório, clone, pastas e terminal; VS Code; arquivo TypeScript; branch, status, add, commit e push; Issue, PR e code review.

## 3. Conceitos mínimos

Um arquivo contém texto ou código. O terminal executa comandos na pasta atual. Git registra versões locais; GitHub permite compartilhar e revisar essas versões. Uma branch separa sua tarefa da versão principal.

O programa inicial deve exibir informações no terminal. Uma variável dá nome a um valor; `console.log` exibe um valor. Descubra a forma exata pela pesquisa e pelas pistas, sem copiar uma solução pronta.

## 4. O que pesquisar

- “como declarar const em TypeScript”
- “console.log JavaScript”
- “diferença entre commit e push Git”
- “como criar pull request GitHub”

## 5. Tarefas práticas

Faça uma Issue e um PR para **cada** tarefa:

1. `Adicionar o nome do sistema`: crie o arquivo inicial e exiba `Controle de Produtos`.
2. `Adicionar mensagem de boas-vindas`: exiba uma segunda mensagem clara.
3. `Exibir versão do sistema`: use uma variável separada para a versão `1.0.0`.
4. `Corrigir mensagem incorreta`: peça ao mentor para inserir ou indicar um pequeno erro de texto; reproduza e corrija.

### Critérios de aceite

- cada execução mostra exatamente as informações pedidas, sem `undefined` ou erros;
- cada tarefa possui branch e PR próprios, ligados à Issue;
- o PR explica a mudança e como conferir o resultado;
- nenhum arquivo sem relação entra no commit.

### Pistas

<details><summary>💡 Pista 1</summary>Uma string é um texto delimitado por aspas. Procure como atribuí-la a uma constante.</details>

<details><summary>💡 Pista 2</summary>Leia o exemplo da documentação de <code>console.log</code> e substitua o valor pelo nome da sua variável.</details>

## 6. Fluxo Git

Para a primeira tarefa:

```bash
git switch main
git pull
git switch -c feat/system-name
git status
# altere e teste o arquivo
git diff
git add caminho/do/arquivo
git diff --staged
git commit -m "feat: add product system name"
git push -u origin feat/system-name
```

Abra o PR no GitHub. Após aprovação e merge, volte à `main`, execute `git pull` e crie outra branch. Sugestões: `feat/welcome-message`, `feat/system-version` e `fix/welcome-message`.

## 7. Antes de abrir o PR

- [ ] Li minha alteração inteira
- [ ] Executei e vi o resultado esperado
- [ ] Revisei `git status`, `git diff` e o commit
- [ ] Preenchi o template e relacionei a Issue
- [ ] Sei explicar cada linha alterada

## 8. Perguntas de revisão

- Qual é a diferença entre Git e GitHub? Entre commit e push?
- Por que usamos uma branch? O que `git status` informa?
- De onde vem o valor mostrado no terminal?
- O que aconteceria se o nome da variável estivesse escrito de forma diferente no `console.log`?

## 9. Critério para avançar

- [ ] Consigo localizar o repositório e abrir o projeto pelo terminal
- [ ] Consigo repetir o fluxo Issue → branch → PR com consulta mínima
- [ ] Sei corrigir um comentário de review e enviar a correção
- [ ] Consigo explicar o arquivo inicial linha por linha

## 10. Retrospectiva

O que aprendi? O que ainda não faço sozinho? Onde precisei de ajuda? Qual erro mais me ensinou? O que consigo explicar hoje que não conseguia antes?

[Próxima etapa →](../02-primeiros-passos-com-programacao/README.md)
