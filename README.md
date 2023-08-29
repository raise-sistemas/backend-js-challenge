# backend-js-challenge

Teste para candidatos backend javascript.
Nós amamos JS e usamos para backend(Deno e Cloudflare), frontend(React) e Mobile.
O objetivo é avaliar a capacidade do candidato de aprender uma tecnologia nova (Cloudflare worker + D1) e a habilidade de trabalhar com Javascript/Typescript puro, sem depender de bibliotecas externas. Entender como funciona o protocolo http, request, response, cabeçalhos, middleares, roteamento, etc.

O desafio é implementar um contador de page views conforme o serviço: https://pageview.appjs.workers.dev/pageview/test

Criar uma única rota no formato: /pageview/:key onde key é um identificador do contador (alfanumérico com 10 caracteres no máximo).

Cada visita nesta rota, incrementa um contador daquele :key específico. A resposta é um Content-Type: text/plain contendo apenas o número do contador.

Enviar junto com a resposta um cabeçalho no formato **X-Runtime: 318** com a quantidade de milisegundos que o serviço levou para executar, do começo ao fim.

## Requisitos

- Criar um projeto público no github e enviar para dev@e-inscricao.com
- Criar uma conta gratuita no Cloudflare e publicar o worker (não é preciso informar cartão de crédito)
- Utilizar o serviço D1 para armazenar os dados
- Não é permitido importar pacotes externos, toda a solução precisa ser implementada com código próprio (roteamento, acesso a banco, etc).
- Utilizar Typescript
- Criar testes automatizados utilizando [Vitest](https://vitest.dev/)
- Será avaliado a organização do código
- Não criar classes, preferimos uma abordagem funcional

Boa sorte!
