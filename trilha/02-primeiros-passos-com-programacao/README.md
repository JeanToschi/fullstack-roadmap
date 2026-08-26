# Etapa 02 — Primeiros passos com programação

```text
Você está aqui:
[✓] 01 — Primeiro Pull Request
[→] 02 — Primeiros passos com programação
[ ] 03 — Funções, arrays e objetos
```

## 1. Objetivo da etapa

Representar um produto e tomar decisões simples sobre disponibilidade, estoque, preço e situação.

## 2. O que será aprendido

`const`, `let`, `string`, `number`, `boolean`, operadores, comparação, `if` e `else`.

## 3. Conceitos mínimos

Variáveis guardam valores. Prefira `const` quando a referência não será reatribuída e use `let` somente quando precisar mudar. Condições executam caminhos diferentes conforme uma expressão verdadeira ou falsa. Compare com `===`, deixando clara a intenção.

## 4. O que pesquisar

- “tipos string number boolean TypeScript”
- “const vs let JavaScript”
- “if else TypeScript”
- “operadores comparação === maior que JavaScript”

## 5. Tarefas práticas

1. **Disponibilidade:** modele nome, preço, ativo e estoque; informe se pode ser vendido.
2. **Estoque zerado:** mostre um aviso específico quando o estoque for zero.
3. **Frete grátis:** informe frete grátis quando o preço atingir o limite definido na Issue.
4. **Produto inativo:** mostre mensagens diferentes para ativo e inativo.
5. **Bug orientado:** reproduza e corrija uma regra que considera estoque negativo disponível.

### Critérios de aceite

- as informações usam tipos adequados;
- cenários dos dois lados de cada condição são executados e anotados no PR;
- estoque zero ou negativo nunca aparece como disponível;
- não há números repetidos sem nome: o limite do frete tem uma constante clara;
- cada tarefa segue Issue, branch e PR.

### Pistas

<details><summary>💡 Pista 1</summary>Escreva em português a regra “pode vender quando...”; depois identifique as comparações.</details>

<details><summary>💡 Pista 2</summary>O operador <code>&&</code> exige que duas condições sejam verdadeiras.</details>

## 6. Fluxo Git

Use branches como `feat/product-availability` e `fix/negative-stock`. Repita os comandos da etapa anterior, mas tente primeiro escrevê-los de memória. Um commit deve descrever um comportamento, não “alterações”.

## 7. Antes de abrir o PR

- [ ] Testei valores normais e limites (zero, limite exato, inativo)
- [ ] Li a alteração e revisei o diff
- [ ] Usei nomes que revelam o significado
- [ ] Removi logs que não fazem parte da saída
- [ ] Sei explicar as condições

## 8. Perguntas de revisão

- Qual a diferença entre `string`, `number` e `boolean`?
- Por que o estoque deve ser comparado com zero?
- O que muda se trocar `&&` por `||` na disponibilidade?
- Encontre onde a mensagem final é decidida.

## 9. Critério para avançar

- [ ] Declaro e identifico os tipos básicos
- [ ] Escrevo e testo condições simples sem copiar
- [ ] Prevejo o resultado antes de executar
- [ ] Faço o fluxo Git completo com pouca consulta

## 10. Retrospectiva

O que aprendi? O que ainda não faço sozinho? Onde precisei de ajuda? Qual erro mais me ensinou? O que consigo explicar hoje que não conseguia antes?

[Próxima etapa →](../03-funcoes-arrays-e-objetos/README.md)
