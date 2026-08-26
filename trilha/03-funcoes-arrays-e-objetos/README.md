# Etapa 03 — Funções, arrays e objetos

```text
Você está aqui:
[✓] 02 — Primeiros passos com programação
[→] 03 — Funções, arrays e objetos
[ ] 04 — CRUD em memória
```

## 1. Objetivo da etapa

Organizar produtos em uma coleção e criar funções reutilizáveis para consultar e calcular dados do catálogo.

## 2. O que será aprendido

Funções, parâmetros, retorno, objetos, arrays, tipos próprios, `map`, `filter`, `find`, `some` e `every`.

## 3. Conceitos mínimos

Um objeto reúne propriedades de uma entidade; um array reúne vários valores. Uma função recebe dados por parâmetros e devolve um resultado com `return`. Métodos de array têm intenções diferentes: transformar, selecionar, localizar ou responder a uma pergunta.

## 4. O que pesquisar

- “type object TypeScript” e “array TypeScript”
- “parâmetros e retorno função TypeScript”
- “diferença map filter find JavaScript”
- “some every JavaScript”

## 5. Tarefas práticas

1. Criar o tipo de produto e uma lista com pelo menos quatro cenários variados.
2. Listar os nomes dos produtos sem alterar a lista original.
3. Buscar produto por ID e tratar a ausência.
4. Exibir apenas produtos ativos.
5. Calcular o valor total do estoque (`preço × quantidade`).
6. Verificar se existe produto sem estoque e se todos têm preço positivo.
7. Criar função que recebe preço e percentual e retorna o preço com desconto.

### Critérios de aceite

- funções recebem os dados necessários e retornam valores previsíveis;
- cada método de array é usado de acordo com sua intenção;
- busca inexistente não causa erro;
- cálculo total considera todos os itens e não altera os produtos;
- há demonstração de ao menos dois cenários por função.

### Leitura e debug

Escolha uma função e explique cada entrada, decisão e saída. Depois peça ao mentor um bug simples (ID com tipo incorreto ou `return` ausente): reproduza, leia a mensagem, formule uma hipótese, use um log temporário e confirme a correção.

## 6. Fluxo Git

Use uma Issue por comportamento e branches como `feat/product-search`. Consulte os comandos somente se travar. Antes do commit, confira se um arquivo não relacionado entrou por engano.

## 7. Antes de abrir o PR

- [ ] Testei lista preenchida, vazia e busca inexistente quando aplicável
- [ ] Minhas funções têm nomes, entradas e retornos claros
- [ ] Revisei o diff e removi logs temporários
- [ ] Sei justificar o método de array escolhido

## 8. Perguntas de revisão

- O que `filter` retorna? Como difere de `find`?
- Por que essa lógica está em uma função?
- De onde o parâmetro recebe seu valor? Onde o retorno é usado?
- A função modifica o array original? Como você verificou?

## 9. Critério para avançar

- [ ] Modelo objetos e arrays tipados
- [ ] Escrevo funções com parâmetros e retorno
- [ ] Escolho entre `map`, `filter`, `find`, `some` e `every`
- [ ] Investigo um bug com hipótese e evidência

## 10. Retrospectiva

O que aprendi? O que ainda não faço sozinho? Onde precisei de ajuda? Qual erro mais me ensinou? O que consigo explicar hoje que não conseguia antes?

[Próxima etapa →](../04-crud-em-memoria/README.md)
