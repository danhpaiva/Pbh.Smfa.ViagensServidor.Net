# 🚀 Proposta de Arquitetura: Hub de Integração e Orquestração Resiliente

## 📌 Contexto do Desafio

Este documento apresenta uma proposta de arquitetura para um sistema que atuará como um **Hub de Integração e Orquestração**. <br>
A finalidade principal deste hub é intermediar a comunicação e o fluxo de dados entre diversos sistemas de terceiros, garantindo um processamento robusto e confiável.

O sistema será responsável por:
* **Recebimento de Requisições Externas:** Ingerir dados através de APIs e/ou filas de mensagens.
* **Processamento Interno:** Aplicar regras de negócio complexas sobre os dados recebidos.
* **Envio de Dados para Outros Sistemas:** Distribuir informações processadas para sistemas downstream.
* **Gerenciamento de Estados e Workflow:** Controlar o ciclo de vida e o progresso de cada requisição.

O foco primordial é garantir **resiliência, rastreabilidade, observabilidade e escalabilidade** em todas as operações.

## 🎯 Objetivo da Proposta

Propor uma arquitetura técnica que satisfaça os requisitos funcionais e não funcionais detalhados, alinhada com as melhores práticas de desenvolvimento e operação de sistemas distribuídos modernos.

## 📦 Componentes da Proposta

A proposta de arquitetura detalhada, a ser entregue em formato PDF, abordará os seguintes tópicos:

1.  **Diagrama de Arquitetura (Alto Nível):** Uma representação visual clara dos principais componentes e seus relacionamentos.
2.  **Justificativas Técnicas:** Explanação detalhada das escolhas de tecnologias e padrões arquiteturais.
3.  **Estratégias para Estabilidade, Rastreabilidade e Segurança:** Medidas e implementações para garantir a robustez, monitoramento e proteção do sistema.
4.  **Pontos de Atenção e Riscos Identificados:** Análise proativa de desafios potenciais e suas mitigações.

## 🧩 Requisitos Não Funcionais Esperados

A arquitetura proposta será desenhada para atender aos seguintes requisitos cruciais:

* **Alta Disponibilidade e Tolerância a Falhas:** O sistema deve permanecer operacional mesmo diante de falhas de componentes individuais.
* **Observabilidade com Logs Estruturados e Métricas:** Capacidade de monitorar o estado interno do sistema através de logs detalhados e métricas de desempenho.
* **Escalabilidade Horizontal:** Habilidade de aumentar a capacidade de processamento adicionando mais instâncias do sistema.
* **Segurança na Comunicação entre Sistemas:** Garantia de que todas as interações entre componentes e sistemas externos são protegidas.
* **Facilidade de Manutenção e Evolução:** O design deve permitir a introdução de novas funcionalidades e a manutenção contínua de forma eficiente.

## 🖼️ Visão Conceitual da Arquitetura

Para dar uma ideia do que será abordado no diagrama de arquitetura, aqui está uma representação visual conceitual:

## ✨ Codigo Fonte Desenvolvido - Repositorios do Projeto:

API Principal
~~~
https://github.com/danhpaiva/Pbh.Smfa.ViagensServidor.Api.Net
~~~

Consumer da API
~~~
https://github.com/danhpaiva/Consumer.Pbh.Smfa.ViagensServidor.Api.Console.Net
~~~

Aplicacao que faz Resiliencia dos Dados no RabbitMq
~~~
https://github.com/danhpaiva/ResilientSender.Pbh.Smfa.ViagensServidor.Net
~~~
` `
