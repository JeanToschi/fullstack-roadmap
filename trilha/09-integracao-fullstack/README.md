# Etapa 09 — Integração Full Stack

```text
Você está aqui:
[✓] 08 — Angular
[→] 09 — Integração Full Stack
[ ] 10 — Validações e erros
```

## 1. Objetivo da etapa

Conectar Angular, NestJS e PostgreSQL para executar o CRUD completo pela interface.

## 2. O que será aprendido

Cliente HTTP, operações assíncronas, contratos entre frontend e backend, configuração de URL e atualização de estado após respostas.

## 3. Conceitos mínimos

```text
Angular → HTTP → NestJS → PostgreSQL
Angular ← JSON ← NestJS ← resultado
```

A interface não lê o banco diretamente. Ela envia uma requisição e reage à resposta. O contrato define campos, formatos e status que os dois lados precisam respeitar. Configuração de ambiente separa a URL da API do código de tela.

## 4. O que pesquisar

- documentação Angular: HttpClient
- “Observable subscribe Angular HTTP”
- “CORS NestJS Angular”
- “environment configuration Angular API URL”
- “Network tab browser developer tools”

## 5. Tarefas práticas

1. Substituir a listagem mockada por `GET /products`.
2. Integrar detalhe e cadastro.
3. Integrar edição preservando o contrato de `PATCH`.
4. Integrar exclusão com confirmação e atualização da lista.
5. Remover mocks que deixaram de ser usados.
6. Investigar um contrato quebrado propositalmente pelo mentor usando a aba Network.

### Critérios de aceite

- listar, visualizar, cadastrar, editar e excluir funcionam pela interface;
- atualização só aparece como concluída após resposta de sucesso;
- URL da API não está espalhada pelos components;
- recarregar a página preserva mudanças feitas no banco;
- requests exibidas na aba Network correspondem aos endpoints documentados;
- não há duplicação de modelos incompatíveis sem justificativa.

## Siga o dado

Para cadastro e edição, desenhe e explique:

- De onde o dado vem?
- Por quais arquivos ele passa?
- Onde é validado?
- Onde é salvo?
- Como volta para a tela?

Faça a explicação com os arquivos abertos, do clique até a linha persistida e de volta ao template.

## 6. Fluxo Git

Planeje a integração verticalmente: cada PR deve entregar um comportamento observável de ponta a ponta. Registre qualquer mudança de contrato e seus consumidores no mesmo plano de Issue.

## 7. Antes de abrir o PR

- [ ] Testei frontend, API e banco iniciando do zero
- [ ] Conferi request, status e response na aba Network
- [ ] Testei recarregamento após cada operação
- [ ] Removi mocks e logs que ficaram obsoletos
- [ ] Consigo seguir o dado sem pular camadas

## 8. Perguntas de revisão

- Qual arquivo inicia a requisição e qual endpoint a recebe?
- Onde o dado muda de formulário para JSON e de registro para resposta?
- Como a lista sabe que deve atualizar após uma exclusão?
- Uma falha foi causada por tela, contrato, backend ou banco? Que evidência comprova?

## 9. Critério para avançar

- [ ] Demonstro o CRUD completo pela interface
- [ ] Uso Network e logs para localizar a camada de uma falha
- [ ] Explico o fluxo frontend → backend → banco → frontend
- [ ] Alinho uma mudança de contrato nos dois lados

## 10. Retrospectiva

O que aprendi? O que ainda não faço sozinho? Onde precisei de ajuda? Qual erro mais me ensinou? O que consigo explicar hoje que não conseguia antes?

[Próxima etapa →](../10-validacoes-e-erros/README.md)
