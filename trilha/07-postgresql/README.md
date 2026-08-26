# Etapa 07 — PostgreSQL

```text
Você está aqui:
[✓] 06 — NestJS
[→] 07 — PostgreSQL
[ ] 08 — Angular
```

## 1. Objetivo da etapa

Substituir o array por persistência PostgreSQL e relacionar produtos a categorias sem alterar o contrato da API.

## 2. O que será aprendido

Banco, tabela, linha, coluna, chave primária e estrangeira; `SELECT`, `INSERT`, `UPDATE`, `DELETE`, `WHERE`, `ORDER BY` e `JOIN`; migrações e configuração por ambiente.

## 3. Conceitos mínimos

Uma tabela define colunas; cada linha representa um registro. A chave primária identifica a linha e a estrangeira referencia outra tabela. SQL consulta e altera os dados. Uma migração registra mudanças de estrutura para que a equipe possa reproduzi-las.

```text
categories (id) ← products (category_id)
```

## 4. O que pesquisar

- documentação PostgreSQL: tipos, constraints e CRUD
- “primary key foreign key PostgreSQL”
- “SQL join products categories”
- documentação da ferramenta de acesso a dados escolhida pelo mentor
- “variáveis de ambiente Node.js banco de dados”

## 5. Tarefas práticas

1. Desenhar as tabelas `products` e `categories`, tipos e restrições; revisar antes de implementar.
2. Criar migrações e inserir dados locais de teste.
3. Executar manualmente consultas com `WHERE`, `ORDER BY` e `JOIN` e explicar resultados.
4. Integrar leitura e cadastro de produtos ao service.
5. Integrar atualização e exclusão, incluindo categoria inexistente.
6. Reiniciar a API e demonstrar que os dados permanecem.

### Critérios de aceite

- schema é reproduzível por migrações, sem edição manual obrigatória;
- preço e estoque têm tipos e restrições coerentes;
- produto referencia uma categoria existente;
- credenciais ficam em variáveis de ambiente e não são commitadas;
- endpoints preservam contratos e dados sobrevivem ao reinício;
- `JOIN` retorna produto com sua categoria.

### Investigação

Reproduza uma violação de chave estrangeira em ambiente local. Leia nome da constraint, tabela e valor envolvidos; formule uma hipótese antes de mudar código ou dados.

## 6. Fluxo Git

Crie Issues para schema, consultas e integração. Proponha nomes de branches e estratégia de commits no comentário inicial da primeira Issue. Inclua migração e código dependente em uma ordem revisável.

## 7. Antes de abrir o PR

- [ ] Recriei o banco do zero usando as instruções
- [ ] Testei persistência após reinício e relações inválidas
- [ ] Não incluí senha, `.env` ou dado sensível
- [ ] Revisei migrações e consultas destrutivas
- [ ] Sei seguir o endpoint até a consulta executada

## 8. Perguntas de revisão

- Por que `category_id` é uma chave estrangeira?
- Qual consulta localiza produtos ativos ordenados por nome?
- Onde um registro é convertido em resposta da API?
- O que falha se uma categoria referenciada for excluída? Qual comportamento foi escolhido?

## 9. Critério para avançar

- [ ] Crio, consulto, atualizo e excluo registros com SQL básico
- [ ] Explico chaves e relacionamento com dados reais
- [ ] Executo migrações em um banco vazio
- [ ] Investigo erros do banco sem expor credenciais

## 10. Retrospectiva

O que aprendi? O que ainda não faço sozinho? Onde precisei de ajuda? Qual erro mais me ensinou? O que consigo explicar hoje que não conseguia antes?

[Próxima etapa →](../08-angular/README.md)
