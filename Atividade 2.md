## 1. Acompanhar o pedido

### História de usuário

**Como** cliente do aplicativo de delivery,\
**quero** acompanhar o status do meu pedido após a compra,\
**para** saber em que etapa ele está e quando será entregue.

### Critérios de aceitação

**Cenário 1 — Visualizar o status do pedido**

- **Dado** que o cliente realizou um pedido com sucesso,
- **Quando** acessar a tela de acompanhamento,
- **Então** o aplicativo deve exibir o status atual do pedido.

**Cenário 2 — Atualização do status**

- **Dado** que o pedido está em andamento,
- **Quando** o restaurante ou entregador atualizar o status,
- **Então** o novo status deve ser exibido para o cliente.

**Cenário 3 — Pedido entregue**

- **Dado** que o pedido está em processo de entrega,
- **Quando** o entregador confirmar a entrega,
- **Então** o status do pedido deve ser alterado para "Entregue".

---

## 2. Informar item indisponível

### História de usuário

**Como** restaurante,\
**quero** informar quando um item do meu cardápio estiver indisponível,\
**para** evitar que clientes façam pedidos de produtos que não podem ser preparados.

### Critérios de aceitação

**Cenário 1 : Marcar item como indisponível**

- **Dado** que o restaurante não possui um item cadastrado no cardápio,
- **Quando** marcar o item como indisponível,
- **Então** o item deve ser identificado como indisponível no aplicativo.

**Cenário 2 — Impedir novos pedidos**

- **Dado** que um item está marcado como indisponível,
- **Quando** um cliente tentar adicioná-lo ao pedido,
- **Então** o aplicativo deve impedir a inclusão do item.

**Cenário 3 — Tornar item disponível novamente**

- **Dado** que um item está marcado como indisponível,
- **Quando** o restaurante alterar sua disponibilidade para disponível,
- **Então** o item deve voltar a poder ser adicionado aos pedidos.

---

## 3. Reportar problema durante a entrega

### História de usuário

**Como** entregador,\
**quero** reportar problemas ocorridos durante uma entrega,\
**para** informar o restaurante e o cliente sobre situações que possam afetar a entrega.

### Critérios de aceitação

**Cenário 1 — Registrar um problema**

- **Dado** que o entregador possui uma entrega em andamento,
- **Quando** ocorrer um problema durante a entrega,
- **Então** o entregador deve conseguir registrar o problema no aplicativo.

**Cenário 2 — Informar o tipo do problema**

- **Dado** que o entregador está registrando um problema,
- **Quando** selecionar o motivo da ocorrência,
- **Então** o aplicativo deve registrar o tipo de problema informado.

**Cenário 3 — Comunicar o problema**

- **Dado** que o entregador registrou um problema,
- **Quando** confirmar o registro da ocorrência,
- **Então** o aplicativo deve disponibilizar a informação para as partes responsáveis pelo pedido.

---

# Priorização — MoSCoW

| Prioridade      | História de usuário                 | Justificativa                                                                                                                 |
| --------------- | ----------------------------------- | ----------------------------------------------------------------------------------------------------------------------------- |
| **Must have**   | Acompanhar o pedido                 | É uma funcionalidade essencial para que o cliente saiba o andamento do pedido após a compra.                                  |
| **Must have**   | Informar item indisponível          | Evita que clientes façam pedidos de itens que o restaurante não pode fornecer.                                                |
| **Should have** | Reportar problema durante a entrega | É importante para tratar ocorrências durante a entrega, mas o aplicativo pode funcionar inicialmente sem essa funcionalidade. |
| **Could have**  | —                                   | Nenhuma das três necessidades foi considerada apenas como melhoria opcional.                                                  |
| **Won't have**  | —                                   | Nenhuma das três necessidades precisa ser descartada; todas podem fazer parte do produto.                                     |
