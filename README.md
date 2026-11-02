# Explorando Workflows Automatizados com AWS Step Functions

Repositório criado para documentar o projeto prático do bootcamp da DIO focado em arquiteturas serverless e orquestração de microsserviços utilizando **AWS Step Functions**.

---

## 🎯 Objetivo do Projeto
Compreender e aplicar conceitos de orquestração de fluxos de trabalho distribuídos na nuvem AWS, conectando múltiplos serviços de forma estruturada, resiliente e visual, substituindo lógica complexa de código por máquinas de estados declarativas.

---

## 🛠️ Conceitos e Componentes Explorados

* **AWS Step Functions:** Serviço de orquestração sem servidor (*serverless*) que permite ligar serviços da AWS (como AWS Lambda, Amazon SNS, SQS, DynamoDB) em fluxos de trabalho sequenciais ou paralelos baseados em estados.
* **Máquinas de Estados (State Machines):** Definidas através da linguagem **Amazon States Language (ASL)** em formato JSON ou YAML.
* **Estados Principais Utilizados:**
  * `Task`: Executa uma unidade de trabalho (ex: invocar uma função Lambda).
  * `Choice`: Adiciona lógica condicional (desvios baseados em regras/if-else).
  * `Wait`: Introduz pausas ou atrasos temporizados no fluxo.
  * `Parallel` / `Map`: Permitem a execução simultânea ou iterativa de ramos de processamento.
  * `Succeed` / `Fail`: Estados terminais que definem o sucesso ou falha da execução.

---

## 💡 Principais Vantagens Identificadas
1. **Desacoplamento Visual:** Facilidade para monitorizar o progresso de execuções complexas através de diagramas visuais na consola da AWS.
2. **Resiliência e Tratamento de Erros:** Gestão nativa de reententações (*retries*) e desvios por excepções (*catch*) sem poluir o código das funções de negócio.
3. **Redução de Código de Infraestrutura:** Menos código boilerplate necessário para coordenar chamadas assíncronas entre microsserviços.

---

## 🚀 Conclusão
O projeto permitiu consolidar a prática de arquiteturas modernas baseadas em microsserviços na nuvem, garantindo competências essenciais no desenho de soluções eficientes e automatizadas.
