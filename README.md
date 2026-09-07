<div align="center">
  <img src = "images/jinbe_icon.png" width="200px">
</div>

<h1 align = "center">

  Jinbe Client [[🇧🇷](README.md)/...]
  
  <p>NVIDIA Triton Inference - Kotlin/Android Client</p>
  <p align="center">
    <img src="https://img.shields.io/github/last-commit/JosManoel/jinbe-client">
    <img src="https://img.shields.io/github/license/JosManoel/jinbe-client">
  </p>
</h1>

<p align ="center">
<a href= "#sobre-este-projeto">🔍 Sobre este projeto</a> &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
<a href="#consideracoes">📑 Considerações</a> &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
<a href="#licenca">📝 Licença</a>
</p>

<hr>

<h2 id = "sobre-este-projeto">🔍 Sobre este projeto</h2>

O **Jinbe Client** implementa uma biblioteca para comunicação entre aplicações **Android Nativo _(Kotlin)_** e servidores **NVIDIA Triton Inference**, utilizando [HTTP](https://developer.mozilla.org/pt-BR/docs/Web/HTTP/Reference/Methods) ou [gRPC](https://grpc.io). 

### O que é o NVIDIA Triton Inference

O [NVIDIA Triton Inference](https://github.com/triton-inference-server/server) é um projeto de código aberto voltado à padronização de serviços de inferência de redes neurais, independente do modelo, nos formatos TensorRT, PyTorch, ONNX, OpenVINO, Python e RAPIDS FIL.

O Triton Inference Server, especificamente, funciona como um servidor de processamento por modelos de IA, abstraindo toda a lógica de processamento para servidores externos, que podem ser hospedados em máquinas x86, com ou sem GPUs, máquinas ARM ou hospedados na AWS.

Para mais informações: [NVIDIA Triton Inference Server](https://docs.nvidia.com/deeplearning/triton-inference-server/user-guide/docs/index.html)


### Qual o propósito dessa biblioteca?

Atualmente, para desenvolver aplicações Android que consomem soluções do Triton Server é necessário utilizar o [protoc compiler](https://protobuf.dev/getting-started/) para compilar uma API gRPC, diferente das aplicações criadas em C++ e Python, que possuem clientes próprios. 

Ainda existe uma [API em java](https://github.com/triton-inference-server/client/tree/main/src/java), desenvolvida pela [Alibaba Cloud PAI Team](https://www.alibabacloud.com/en?_p_lc=1&utm_content=se_1024016509&gclid=CjwKCAjwnvTUBhBoEiwAZNDxZ3jKFQxFVLWfrUGclGxMyK-AKQ2INCyNEU-nsL1wyRQGrXy_3eFJNRoCQ0EQAvD_BwE) e que poderia ser utilizada para o desenvolvimento de aplicativos Android, mas ela é limitada e só suporta requisições em HTTP, que não possuem um bom desempenho com processamento de imagem.

Dessa forma, o **Jinbe Client** busca facilitar o uso de servidores de inferência NVIDIA, suprindo as lacunas deixadas pelo cliente em Java, porém padronizando com as chamadas já presentes no cliente em Python e C++.

### Por que esse projeto tem nome de personagem de One Piece ?

Eu achei que ficaria legal.

<hr>

<h2 id="consideracoes">📑 Considerações</h2>

Este projeto está sendo desenvolvido exclusivamente dentro da disciplina de **Processos de Software (DIM0510)**, ministrada como matéria optativa para o curso de **Bacharelado em Tecnologia da Informação**, no **[Instituto Metrópole Digital](https://www.metropoledigital.ufrn.br/portal/)/[UFRN](https://ufrn.br)**.

* **Grupo de desenvolvimento:** Switch Desbloqueado Team
* **Discente:** José Manoel Freitas da Silva (**Mat.:** 20220039467) | [JosManoel](https://github.com/JosManoel)


> Esse projeto ainda terá o desenvolvimento de uma pequena documentação e a implementação de um aplicativo de testes simples, com detecção facial utilizando o modelo [Ultra Light Fast Generic Face Detector](https://github.com/linzaer/ultra-light-fast-generic-face-detector-1mb), rodando locamente em uma máquina sem GPU.

Para **MVP** e **Visão**, ver [proposta.md](docs/proposta.md).
<hr>

<h2 id="licenca">📝 Licença</h2>

- Este projeto está sob a licença [MIT](https://github.com/Arco-de-Treinamento/Shishin-no-Ken/blob/main/LICENSE).

<hr>

<div align = "center">
  
  👋🏾 Feito por [JosManoel](https://github.com/JosManoel) com ☕ ☕ ☕ ☕ ☕ , 🎧 e 💻.
</div> 
