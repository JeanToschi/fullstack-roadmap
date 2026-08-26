# Etapa 04 — CRUD em memória

```text
Você está aqui:
[✓] 03 — Funções, arrays e objetos
[→] 04 — CRUD em memória
[ ] 05 — HTTP e API REST
```

## 1. Objetivo da etapa

Implementar o ciclo completo de cadastro de produtos em memória, separando operações e regras de negócio.

## 2. O que será aprendido

CRUD (Create, Read, Update, Delete), identificadores, estado em memória, validações iniciais e composição de funções.

## 3. Conceitos mínimos

CRUD nomeia quatro operações comuns: criar, ler, atualizar e excluir. “Em memória” significa que os dados somem ao encerrar o programa. Cada função deve ter uma responsabilidade clara e lidar conscientemente com IDs inexistentes.

## 4. O que pesquisar

- “CRUD significado”
- “imutabilidade array TypeScript”
- “Partial TypeScript”
- “gerar identificador simples aplicação em memória”

## 5. Tarefas práticas

- implementar `createProduct` com ID único;
- implementar `getProducts` e `getProductById`;
- implementar `updateProduct` sem apagar campos não enviados;
- implementar `deleteProduct` com resultado que indique sucesso ou ausência;
- criar um roteiro executável que combine todas as operações;
- corrigir um bug no qual atualizar um ID inexistente altera outro item.

### Critérios de aceite

- criar aumenta a lista e não reutiliza ID;
- listar e buscar retornam resultados coerentes;
- atualizar preserva ID e campos não informados;
- excluir somente remove o item escolhido;
- operações inexistentes têm comportamento definido;
- o roteiro demonstra Create → Read → Update → Delete.

## 6. Fluxo Git

Planeje uma Issue por operação e uma integração final. Escolha branches descritivas; os comandos não serão fornecidos. Mantenha as regras fora do roteiro de demonstração.

## 7. Antes de abrir o PR

- [ ] Testei sucesso, lista vazia e ID inexistente
- [ ] Uma função não mistura várias operações
- [ ] Revisei alterações não relacionadas e logs temporários
- [ ] Consigo mostrar onde os dados ficam enquanto o programa roda

## 8. Perguntas de revisão

- O que se perde quando o processo termina e por quê?
- Onde cada item do CRUD está implementado?
- Como o ID percorre a chamada até a busca?
- O que ocorreria se duas criações recebessem o mesmo ID?

## 9. Critério para avançar

- [ ] Implemento e demonstro as quatro operações
- [ ] Trato IDs inexistentes de forma consistente
- [ ] Divido uma demanda em PRs pequenos
- [ ] Explico o estado da lista após cada chamada

## 10. Retrospectiva

O que aprendi? O que ainda não faço sozinho? Onde precisei de ajuda? Qual erro mais me ensinou? O que consigo explicar hoje que não conseguia antes?

[Próxima etapa →](../05-http-e-api-rest/README.md)
