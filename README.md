# E-commerce Web + RabbitMQ

Desenvolva uma solução de e-commerce web para comercialização de produtos na internet.
Devem ser implementados serviços de acordo com a figura a seguir. Os serviços devem **simular
seus respectivos comportamentos**, sem necessidade de implementações reais ou persistência
em banco de dados. A integração dos serviços deve ser realizada por meio da **combinação de
processos coreografados e orquestrados**. Os serviços de Produtos e CEP devem utilizar como
fonte de dados os respectivos arquivos JSON disponibilizados na atividade. Implementar uma **Dead
Letter Queue (DLQ)** na fila de pagamento. A Loja Web deve **armazenar os erros** vindos da **DLQ**
em um arquivo de **Log**. Simule o erro no pagamento informando um valor negativo.

<img width="694" height="494" alt="image" src="https://github.com/user-attachments/assets/a260c2ba-98b0-4d4d-8204-52c2bf70b150" />

O fluxo de compras de produtos deve seguir a ordem a seguir:

1. Loja Web exibe catálogo de produtos
2. Usuário escolhe produtos para comprar
3. Usuário informa dados de pagamento e endereço de entrega
4. Usuário informa CEP para preenchimento automático do endereço
5. Usuário confirma a compra
6. Sistema envia e-mail de confirmação da compra
7. Sistema realiza a transação de pagamento
8. Sistema envia e-mail com resultado do pagamento
9. Sistema gera nota fiscal e baixa o estoque
10. Sistema envia e-mail com a nota fiscal
11. Sistema disponibiliza produtos para entrega
12. Sistema envia e-mail com dados da entrega

---

Atividade desenvolvida para a disciplina de **Arquitetura de Sistemas Distribuídos**.
