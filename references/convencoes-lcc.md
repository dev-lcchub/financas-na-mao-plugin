# Convenções dos dados do Finanças na Mão

## Dinheiro

Valores em dinheiro (`amount`, `available_value`, totais de Pix, saldos,
recebíveis) chegam como **inteiros em centavos**. Na resposta à pessoa, formate
em reais: `123456` vira R$ 1.234,56. Nunca mostre centavos crus nem some
valores de unidades diferentes.

## Taxas

A `rate` de uma proposta é **percentual decimal** (`"1.5"` = 1,5% ao mês).
Taxa não é dinheiro: não converta taxa para centavos.

## Dados

- Use só o que as tools devolveram. Não invente valor, status ou proposta.
- A conexão mostra só os dados da própria pessoa. Erro de acesso é acionável:
  leia a mensagem antes de tentar de novo.
- O assistente lê o que já está gravado na plataforma; ler não dispara
  atualização com o banco. Diga quando o dado pode estar desatualizado.
