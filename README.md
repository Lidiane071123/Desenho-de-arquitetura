# AWS Step Functions - Desafio Prático DIO

Este repositório foi criado como parte do desafio proposto pela DIO com o objetivo de consolidar workflows automatizados utilizando o serviço **AWS Step Functions**.

## Objetivos de Aprendizagem

- Aplicar conceitos teóricos em um ambiente prático real.
- Automatizar processos utilizando AWS Step Functions.
- Orquestrar serviços AWS como Lambda, SQS, SNS e DynamoDB.
- Documentar o processo técnico de forma clara e reusável.
- Utilizar o GitHub como repositório de conhecimento técnico.

## Tecnologias e Serviços Utilizados

- AWS Step Functions
- AWS Lambda
- Amazon SQS (opcional)
- Amazon SNS (opcional)
- Amazon DynamoDB (opcional)
- Amazon CloudWatch (monitoramento)
- Git e GitHub

## Visão Geral do Workflow Automatizado

O fluxo de trabalho implementado simula o **processamento de um pedido online**, com as seguintes etapas:

1. **Receber Pedido** - Função Lambda que valida os dados de entrada.
2. **Verificar Pagamento** - Simulação de verificação de pagamento.
3. **Atualizar Banco de Dados** - Armazena os dados do pedido no DynamoDB.
4. **Notificar Cliente** - Envia notificação via SNS.
5. **Finalizar ou Lidar com Erros** - Tratamento de exceções via Step Functions.


##  Estrutura do Projeto

- `state-machine-definition.json`: Definição da máquina de estados da Step Function em Amazon States Language (ASL).
- `lambda-functions/`: Código fonte das funções Lambda utilizadas.
- `images/`: Capturas de tela e diagramas utilizados na documentação.
- `docs/insights.md`: Insights e anotações adquiridas durante o desafio.

## 📸 Capturas de Tela

Imagens do ambiente AWS, definições da máquina de estado e execução dos workflows.

## Insights

Durante a execução do desafio, foram identificados pontos importantes:
- A definição clara dos estados ajuda na leitura e manutenção do fluxo.
- A integração entre serviços AWS é facilitada por roles e permissões bem definidas no IAM.
- O uso de CloudWatch foi essencial para depurar e monitorar as execuções.

## Como Executar

> Pré-requisitos:
> - Conta na AWS
> - AWS CLI configurado
> - Permissões para Lambda, Step Functions, DynamoDB e SNS

1. Faça o deploy das funções Lambda.
2. Crie uma máquina de estado na AWS Step Functions utilizando o JSON fornecido.
3. Execute a máquina com uma entrada de teste (JSON).
4. Monitore os resultados via console ou pelo CloudWatch.

##  Conclusão

Este laboratório foi fundamental para aplicar os conceitos vistos em aula, desde a criação da lógica até a orquestração e o monitoramento. A prática com AWS Step Functions traz uma visão clara de como orquestrar microserviços de forma resiliente e escalável.

---

Feito com 💻 por [Lidiane Aparecida de Souza Pereira]
