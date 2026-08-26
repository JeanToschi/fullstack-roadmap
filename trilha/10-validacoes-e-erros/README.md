# Etapa 10 — Validações e tratamento de erros

```text
Você está aqui:
[✓] 09 — Integração Full Stack
[→] 10 — Validações e erros
[ ] 11 — Testes e Docker
```

## 1. Objetivo da etapa

Tornar os fluxos de produto seguros e compreensíveis diante de dados inválidos, ausência de dados e falhas.

## 2. O que será aprendido

Validação no frontend e backend, exceções, respostas HTTP, mensagens úteis e estados de loading, vazio e erro.

## 3. Conceitos mínimos

O frontend orienta cedo, mas o backend protege a regra independentemente do cliente. Erros previsíveis devem ter status e mensagem consistentes. A interface precisa distinguir carregando, vazio, sucesso e falha, sem esconder o que ocorreu.

## 4. O que pesquisar

- documentação NestJS: validation e exception filters
- documentação Angular: form validation e HTTP error handling
- “HTTP 400 404 409 500 quando usar”
- “loading empty error states UI”

## 5. Tarefas práticas

### Feature: regras de entrada

- nome é obrigatório e não pode ser apenas espaços;
- preço deve ser maior que zero;
- estoque não pode ser negativo;
- categoria é obrigatória e deve existir.

### Melhoria: estados da interface

- mostrar carregamento durante requisições;
- distinguir catálogo vazio de falha na API;
- exibir mensagens acionáveis e preservar dados do formulário quando for seguro;
- impedir envio duplicado enquanto uma operação está em andamento.

### Bugs para investigar

1. produto inexistente deixa a tela carregando indefinidamente;
2. API indisponível é apresentada como lista vazia;
3. espaços são aceitos como nome;
4. erro interno expõe detalhes técnicos ao usuário.

### Critérios de aceite

- regras são garantidas no backend e refletidas no formulário;
- respostas distinguem entrada inválida, ausência e falha inesperada;
- todos os quatro estados visuais são demonstráveis;
- cada bug tem reprodução, hipótese, correção e teste registrados;
- mensagens ajudam o usuário sem revelar stack trace ou detalhes internos.

## 6. Fluxo Git

Trate cada bug em uma Issue própria usando o template. Antes de implementar, registre evidência e hipótese. Prefira PRs por comportamento completo, incluindo backend e frontend quando ambos forem necessários.

## 7. Antes de abrir o PR

- [ ] Reproduzi o problema antes de corrigir
- [ ] Testei limites e chamadas fora do frontend
- [ ] Confirmei os estados loading, vazio, sucesso e erro
- [ ] Verifiquei que a mensagem não expõe detalhes internos
- [ ] Registrei como evitei regressão

## 8. Perguntas de revisão

- Por que validar também no backend?
- Como a tela distingue lista vazia de API indisponível?
- Onde uma exceção vira status e mensagem HTTP?
- Qual evidência confirmou sua hipótese do bug?

## 9. Critério para avançar

- [ ] Implemento validações nas duas camadas e justifico cada uma
- [ ] Modelo estados de interface explicitamente
- [ ] Investigo bugs por reprodução, hipótese e confirmação
- [ ] Retorno erros úteis sem vazar detalhes técnicos

## 10. Retrospectiva

O que aprendi? O que ainda não faço sozinho? Onde precisei de ajuda? Qual erro mais me ensinou? O que consigo explicar hoje que não conseguia antes?

[Próxima etapa →](../11-testes-e-docker/README.md)
