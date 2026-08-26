# Etapa 05 — HTTP e API REST

```text
Você está aqui:
[✓] 04 — CRUD em memória
[→] 05 — HTTP e API REST
[ ] 06 — NestJS
```

## 1. Objetivo da etapa

Disponibilizar o CRUD conhecido por uma API REST e observar requisições e respostas.

## 2. O que será aprendido

Cliente, servidor, request, response, HTTP, JSON, rota, body, params, query e status codes `200`, `201`, `400`, `404` e `500`.

## 3. Conceitos mínimos

O cliente envia uma requisição; o servidor escolhe uma rota, executa uma operação e devolve uma resposta. O método HTTP expressa a intenção. Params identificam recursos na URL, query modifica uma consulta e body transporta dados. JSON é um formato de troca de dados, não a entidade em si.

| Método e rota | Operação | Resposta esperada |
|---|---|---|
| `GET /products` | listar | `200` |
| `GET /products/:id` | buscar | `200` ou `404` |
| `POST /products` | criar | `201` ou `400` |
| `PATCH /products/:id` | atualizar | `200`, `400` ou `404` |
| `DELETE /products/:id` | excluir | `200` ou `404` |

`500` representa uma falha inesperada do servidor; não deve substituir erros previsíveis do usuário.

## 4. O que pesquisar

- “requisição e resposta HTTP”
- “API REST métodos HTTP”
- “path params query params body diferença”
- “HTTP status 200 201 400 404 500”

## 5. Tarefas práticas

1. Criar um servidor HTTP mínimo e uma rota de verificação.
2. Expor listagem e busca por ID reutilizando o CRUD.
3. Expor cadastro e atualização por JSON.
4. Expor exclusão.
5. Criar uma coleção de requisições ou arquivo `.http` que demonstre sucesso e falha de cada endpoint.

### Critérios de aceite

- todos os endpoints da tabela respondem em JSON quando há corpo;
- IDs de params são convertidos e validados antes da regra de negócio;
- criação retorna `201`; recurso ausente retorna `404`; entrada inválida retorna `400`;
- a regra do CRUD não fica duplicada nas rotas;
- o PR explica como iniciar o servidor e testar cada cenário.

### Investigação

Envie propositalmente JSON inválido, ID inexistente e parâmetro com tipo errado. Registre status, corpo e hipótese para cada resposta. Use logs apenas para seguir a requisição e remova-os ao terminar.

## 6. Fluxo Git

Separe infraestrutura inicial e endpoints em PRs revisáveis. Sugestões: `feat/products-http-server` e `feat/product-create-endpoint`. Decida os commits e explique a divisão no PR.

## 7. Antes de abrir o PR

- [ ] Testei cada endpoint em sucesso e falha
- [ ] Status e corpo correspondem ao cenário
- [ ] Não dupliquei as regras do CRUD
- [ ] Documentei comandos e requisições reproduzíveis
- [ ] Revisei o diff e sei seguir uma requisição

## 8. Perguntas de revisão

- Quem é cliente e quem é servidor no seu teste?
- Onde o ID da URL vira um valor usado pelo CRUD?
- Qual diferença entre `400`, `404` e `500`?
- Siga uma requisição de cadastro até o array e de volta à resposta.

## 9. Critério para avançar

- [ ] Explico request, response, rota e JSON
- [ ] Relaciono os métodos HTTP às operações CRUD
- [ ] Testo e interpreto status de sucesso e erro
- [ ] Localizo o caminho completo de uma requisição

## 10. Retrospectiva

O que aprendi? O que ainda não faço sozinho? Onde precisei de ajuda? Qual erro mais me ensinou? O que consigo explicar hoje que não conseguia antes?

[Próxima etapa →](../06-nestjs/README.md)
