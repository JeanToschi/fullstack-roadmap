# Git e GitHub

Git registra versões no computador. GitHub hospeda o repositório e permite colaborar por Issues, Pull Requests e reviews.

```text
arquivo alterado → git add → commit local → push → Pull Request no GitHub
```

Fluxo básico:

```bash
git switch main
git pull
git switch -c feat/product-name
git status
git diff
git add caminho/do/arquivo
git diff --staged
git commit -m "feat: add product system name"
git push -u origin feat/product-name
```

`git add` escolhe o que entrará no próximo commit; `commit` cria um registro local; `push` envia commits ao GitHub. Uma branch isola a tarefa. Confira `git status` entre os passos e não use `git add .` enquanto ainda não souber exatamente quais arquivos mudou.

Depois do push, abra um PR. O merge incorpora a mudança aprovada à branch principal.
