# Configurando o ambiente

Peça ajuda ao mentor para instalar as ferramentas. Não avance enquanto os comandos de verificação não funcionarem.

## Ferramentas iniciais

- Git;
- Node.js na versão LTS adotada pela equipe (inclui `npm`);
- Visual Studio Code;
- uma conta no GitHub com acesso ao repositório.

No terminal, confira:

```bash
git --version
node --version
npm --version
code --version
```

Configure sua identidade no Git somente com os dados da sua conta:

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu-email-do-github@exemplo.com"
```

Depois, siga o método de autenticação recomendado pela equipe, clone a URL fornecida e entre na pasta:

```bash
git clone URL_DO_REPOSITORIO
cd fullstack-roadmap
code .
```

Execute `git status`. Se aparecer que você está na branch `main` e não há alterações, o ambiente inicial está pronto. Nunca publique senhas, tokens ou arquivos `.env`.

Próximo guia: [Terminal básico](02-terminal-basico.md).
