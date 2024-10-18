## RabbitMQ 

O RabbitMQ é um sistema de mensageria amplamente utilizado para comunicação assíncrona entre serviços e componentes em uma arquitetura distribuída. Ele permite o envio e recebimento de mensagens através de filas de forma confiável e escalável.

### Principais Características:

1. **Modelo de Mensageria Assíncrona**: Facilita a troca de mensagens entre produtores (que enviam mensagens) e consumidores (que as recebem), desacoplando o envio do processamento.

2. **Suporte a Diversos Protocolos**: Compatível com protocolos como AMQP (Advanced Message Queuing Protocol), MQTT e STOMP, tornando-o versátil para diversos cenários.

3. **Trocas (Exchanges) e Filas**:
   - **Direct**: Roteia mensagens para filas específicas com base em chaves.
   - **Topic**: Permite roteamento baseado em padrões de chave.
   - **Fanout**: Envia mensagens para todas as filas associadas à troca.
   - **Headers**: Roteia mensagens com base nos cabeçalhos das mensagens.

4. **Durabilidade e Persistência**: Mensagens e filas podem ser persistentes, garantindo que as mensagens não se percam em caso de falha no servidor.

5. **Confirmação de Mensagens**: Suporte a confirmação de entrega (acknowledgement) para garantir que as mensagens sejam processadas corretamente, evitando perda ou duplicação.

6. **Alta Disponibilidade e Escalabilidade**: Com suporte a clusters, o RabbitMQ permite a execução de várias instâncias, garantindo alta disponibilidade e escalabilidade horizontal. Suporte a replicação de filas também está disponível.

7. **Plugins e Extensibilidade**: Possui uma arquitetura de plugins, permitindo a adição de funcionalidades, como novos protocolos, ferramentas de monitoramento e muito mais.

8. **Políticas de Qualidade de Serviço (QoS)**: Controla o fluxo de mensagens para evitar sobrecarga nos consumidores, limitando a quantidade de mensagens não confirmadas.

Essas características tornam o RabbitMQ uma solução robusta para implementar filas de mensagens em sistemas distribuídos, proporcionando alta confiabilidade e flexibilidade.

### Executando o rabbitmq management com docker-compose
```bash
    docker-compose up --build
```
após isso só acessar o `http://localhost:15672/` com o user: `rabbitmq` pass: `rabbitmq`

### RabbitMQ Simulator
[![Testar RabbitMQ](https://img.shields.io/badge/Try%20RabbitMQ-Click%20Here-orange)](https://tryrabbitmq.com/)
