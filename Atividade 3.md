## História 1

**Como cliente, quero avaliar o pedido depois da entrega, para ajudar outros clientes a escolherem melhor.**

- **Dado** que o pedido foi entregue, **quando** o cliente abre o app, **então** aparece a opção de avaliar o pedido.
- **Dado** que o cliente avalia com nota e comentário, **quando** confirma o envio, **então** a avaliação aparece no perfil do restaurante.

### RNF

**RNF 1  Usabilidade**\
O aplicativo deve apresentar a opção de avaliação de forma clara e simples, permitindo que o cliente encontre e utilize o recurso sem dificuldade.

**RNF 2  Desempenho**\
O aplicativo deve exibir a opção de avaliação em até 2 segundos após o cliente abrir o pedido entregue.

**RNF 3 Segurança**\
O sistema deve permitir que apenas o cliente que realizou o pedido possa registrar ou alterar a avaliação daquele pedido.

---

## História 2

**Como cliente, quero salvar um cartão de pagamento, para não digitar os dados a cada compra.**

- **Dado** que o cliente cadastra um cartão válido, **quando** confirma o cadastro, **então** o cartão fica disponível para escolha no checkout.
- **Dado** que o cliente tem um cartão salvo, **quando** faz um novo pedido, **então** pode selecionar esse cartão sem redigitar os dados.

### RNF

**RNF 4  Segurança**\
Os dados do cartão salvo devem ser protegidos contra acesso não autorizado e não devem ser armazenados de forma que exponha os dados completos do cartão.

**RNF 5  Usabilidade**\
O cliente deve conseguir selecionar um cartão previamente salvo no checkout sem precisar informar novamente seus dados.

**RNF 6 — Confiabilidade**\
O sistema deve manter os cartões cadastrados disponíveis para o cliente em novos pedidos, desde que o cartão ainda esteja válido.



## História 3

**Como dono de restaurante, quero ver um resumo diário de vendas, para acompanhar o desempenho do dia.**

- **Dado** que o dia comercial termina, **quando** o restaurante abre o painel de vendas, **então** vê o total de pedidos e o faturamento do dia.
- **Dado** que o restaurante seleciona um período diferente, **quando** aplica o filtro, **então** o resumo é recalculado para aquele período.

### RNF

**RNF 7 — Eficiência de desempenho**\
O painel de vendas deve apresentar o resumo do período selecionado em até 3 segundos após a aplicação do filtro.

**RNF 8 — Adequação funcional**\
O sistema deve calcular corretamente o total de pedidos e o faturamento considerando somente as vendas pertencentes ao período selecionado.

**RNF 9 — Usabilidade**\
O painel deve apresentar os valores de pedidos e faturamento de forma clara, permitindo que o restaurante compreenda o resumo sem dificuldade.

#
