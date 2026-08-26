# Etapa 12 — Feature final: gerenciamento de categorias

```text
Você está aqui:
[✓] 11 — Testes e Docker
[→] 12 — Feature final
[✓ ao concluir] Formação prática
```

## 1. Objetivo da etapa

Entregar, com supervisão e autonomia, uma feature Full Stack a partir de requisitos próximos aos de uma equipe real.

## 2. O que será aprendido

Refinamento, planejamento vertical, mudanças de banco, backend e frontend, gestão de risco, testes, comunicação de decisões e resposta a review.

## 3. Conceitos mínimos

Você já possui os conceitos necessários. Sua primeira responsabilidade é ler o sistema existente, localizar os pontos de mudança e transformar requisitos em um plano. Não comece alterando código antes de entender dependências e riscos.

## 4. O que pesquisar

Defina sua própria lista após a leitura do repositório. Registre na Issue:

- dúvidas de domínio;
- documentação oficial necessária;
- padrões existentes que podem ser reutilizados;
- riscos de banco, API e interface.

## 5. Demanda

### História

Como responsável pelo catálogo, quero gerenciar categorias e associá-las aos produtos para organizar a consulta do estoque.

### Requisitos

- listar, visualizar, criar, editar e excluir categorias;
- associar uma categoria válida a cada produto;
- persistir alterações no PostgreSQL por migração reproduzível;
- expor endpoints coerentes com a API existente;
- integrar telas e formulários Angular;
- validar dados e tratar ausência, conflito e falhas;
- manter estados de loading, vazio, sucesso e erro;
- criar testes mínimos dos comportamentos críticos;
- executar no ambiente Docker existente.

### Regras a esclarecer no refinamento

- uma categoria pode ser excluída se tiver produtos?
- nome de categoria precisa ser único? A comparação diferencia maiúsculas?
- como produtos sem categoria existentes serão migrados?
- quais endpoints e respostas preservam consistência com a API?

Não suponha essas respostas. Registre propostas e confirme com o mentor, que representa produto e equipe.

### Critérios de aceite

- fluxo completo funciona pela interface e por chamadas diretas à API;
- integridade do relacionamento é garantida no banco e no backend;
- migração funciona em banco vazio e em banco com produtos existentes;
- regras confirmadas no refinamento têm testes de sucesso e falha;
- erros são úteis ao usuário e não expõem detalhes internos;
- documentação permite executar e validar a feature;
- PRs são pequenos, relacionados às Issues e não contêm mudanças alheias.

## 6. Fluxo Git

Apresente antes do código:

1. mapa dos arquivos e fluxo atual;
2. decisões que dependem de refinamento;
3. divisão em Issues e PRs entregáveis;
4. estratégia de migração, testes e rollback;
5. ordem que evita deixar a aplicação quebrada.

Escolha branches e commits coerentes com [Como contribuir](../../CONTRIBUTING.md). Responda ao review com evidência, faça correções na mesma branch e não faça merge automaticamente.

## 7. Antes de abrir o PR

- [ ] Atendi somente o escopo da Issue
- [ ] Testei sucesso, limites, ausência e conflito
- [ ] Revisei banco, backend, frontend e documentação afetados
- [ ] Rodei a suíte e o ambiente Docker
- [ ] Revisei o diff e procurei secrets e código temporário
- [ ] Consigo explicar toda alteração e decisão
- [ ] Documentei como testar e riscos conhecidos

## 8. Perguntas de revisão

- Siga o dado do formulário de categoria até o banco e de volta à tela.
- Onde a integridade é protegida? O que ocorre em chamadas fora da interface?
- Qual foi o maior risco da migração e como foi reduzido?
- Que teste impediria a regressão mais provável?
- Que mudança você faria diferente depois do review e por quê?

## 9. Critério de conclusão da formação

Demonstre ao mentor, sem roteiro pronto:

- [ ] uso de terminal, branch, commits, push, PR e correções de review;
- [ ] leitura e explicação de funções, objetos, arrays e fluxo de dados;
- [ ] implementação de CRUD e endpoints NestJS;
- [ ] consultas e alterações PostgreSQL seguras;
- [ ] componentes, formulários e consumo de API Angular;
- [ ] investigação de bug com reprodução, hipótese, breakpoint/log e confirmação;
- [ ] testes que protegem comportamento relevante;
- [ ] execução e diagnóstico básico com Docker Compose;
- [ ] entrega de uma pequena feature Full Stack com supervisão.

Concluir arquivos não basta. O checkpoint termina quando você demonstra essas competências e consegue explicar escolhas e limitações.

## 10. Retrospectiva final

O que aprendi? O que já consigo fazer sozinho? Onde ainda preciso de supervisão? Qual erro mais me ensinou? Como minha forma de investigar mudou? Qual será minha próxima competência prática?

[← Voltar ao roadmap](../../README.md)
