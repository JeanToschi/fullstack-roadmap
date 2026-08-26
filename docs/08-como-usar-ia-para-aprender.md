# Como usar IA para aprender

> IA pode ajudar a explicar, investigar erros e sugerir caminhos, mas você precisa conseguir explicar todo código que coloca em um Pull Request.

Use IA para pedir explicações, pistas graduais, ajuda com erros, comparação de alternativas, perguntas de entendimento e review da sua tentativa. Nunca aceite código sem ler e testar. Confira documentação oficial quando a resposta depender de versão. Não envie segredos, dados pessoais ou código privado a ferramentas não aprovadas.

Ruim: `Faça essa tarefa para mim.`

Melhor:

```text
Estou tentando filtrar apenas produtos ativos com TypeScript.
Minha tentativa está abaixo e o resultado foi [...].
Explique o conceito que estou confundindo e dê uma pista,
mas não escreva a solução completa.
```

Para investigar:

```text
Recebi esta mensagem de erro [...].
Ajude-me a separar o que ela informa das hipóteses que devo testar.
Faça uma pergunta por vez e não altere meu código por mim.
```

Antes do PR, feche a resposta da IA e explique com suas palavras o problema, o caminho do dado, cada alteração e como o teste demonstra o comportamento. Se não conseguir, ainda não está pronto para enviar.
