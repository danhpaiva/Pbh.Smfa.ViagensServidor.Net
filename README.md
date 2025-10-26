# 🚀 Proposta de Arquitetura: <br> Hub de Integração e Orquestração Resiliente

## 📌 Contexto do Desafio

Neste repositorio ha 02 conteudos: 01 Solucao Inicial de Arquitetura e 01 diagrama da mesma.<br>

Este repositorio apresenta uma proposta de arquitetura para um sistema que atuará como um **Hub de Integração e Orquestração**. <br>
A finalidade principal deste hub é intermediar a comunicação e o fluxo de dados entre diversos sistemas de terceiros, garantindo um processamento robusto e confiável.

O sistema será responsável por:
* **Recebimento de Requisições Externas:** Ingerir dados através de APIs e/ou filas de mensagens.
* **Processamento Interno:** Aplicar regras de negócio complexas sobre os dados recebidos.
* **Envio de Dados para Outros Sistemas:** Distribuir informações processadas para sistemas downstream.
* **Gerenciamento de Estados e Workflow:** Controlar o ciclo de vida e o progresso de cada requisição.

O foco primordial é garantir **resiliência, rastreabilidade, observabilidade e escalabilidade** em todas as operações.

## 🎯 Objetivo da Proposta

Propor uma arquitetura técnica que satisfaça os requisitos funcionais e não funcionais detalhados, alinhada com as melhores práticas de desenvolvimento e operação de sistemas distribuídos modernos.

## 🖼️ Visão Conceitual da Arquitetura

Representação visual conceitual (clique na imagem para expandir):

<p align="center">
   <img src="https://i.ibb.co/b5Qrf2WV/pbh.png?raw=true" width="700" alt="Diagrama">
</p>

## ✨ Codigo Fonte:

### [PBH - API Principal](https://github.com/danhpaiva/Pbh.Smfa.ViagensServidor.Api.Net)
~~~
https://github.com/danhpaiva/Pbh.Smfa.ViagensServidor.Api.Net
~~~

### [Cliente Consumer da API (Terceiros)](https://github.com/danhpaiva/Consumer.Pbh.Smfa.ViagensServidor.Api.Console.Net)
~~~
https://github.com/danhpaiva/Consumer.Pbh.Smfa.ViagensServidor.Api.Console.Net
~~~

### [Cliente ResilientSender (Resiliencia Dados RabbitMq)](https://github.com/danhpaiva/ResilientSender.Pbh.Smfa.ViagensServidor.Net)
~~~
https://github.com/danhpaiva/ResilientSender.Pbh.Smfa.ViagensServidor.Net
~~~

### [Worker ConsumerRabbitMq](https://github.com/danhpaiva/ConsumerRabbitMq.Pbh.Smfa.ViagensServidor.Console.Net)
~~~
https://github.com/danhpaiva/ConsumerRabbitMq.Pbh.Smfa.ViagensServidor.Console.Net
~~~

## 👤 Desenvolvedor

Este projeto foi desenvolvido por:

  * **Nome:** Daniel Paiva
  * **LinkedIn:** [https://www.linkedin.com/in/danhpaiva/](https://www.linkedin.com/in/danhpaiva/)

Sinta-se à vontade para conectar-se e discutir padrões de arquitetura e resiliência\!

***Criado com ❤️ e .NET***
