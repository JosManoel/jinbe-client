# ADR-0003 — Determina a forma de implementação do envio de dados via HTTP

**Estado:** Aceita | **Data:** 29-09-2026

## Contexto

Definir como os dados utilizados para a inferência de elementos com redes neurais serão empacotados para requisições HTTP.

## Soluções

**Tudo dentro do JSON**

* Prós: fácil implementação;

* Contras: overhead crítico de performance. Um tensor de imagem de 1 MB em bytes se transforma em um JSON de vários megabytes;

**Triton HTTP Extension (JSON Header + Raw Binary Append)**

* Prós: performance equivalente à do gRPC. O JSON conterá apenas a descrição do tensor, enquanto os dados brutos (byte[]) são anexados diretamente no final da requisição HTTP (e lidos da mesma forma na resposta).

* Contras: implementação complexa. Exigirá a manipulação de leitura de streams de bytes (ByteReadChannel no Ktor) e cálculo exato de offsets nos cabeçalhos HTTP.

## Decisão

Optou-se por aderir ao Triton HTTP Extension devido à necessidade de maiores pacotes de dados.

[Documentação](https://docs.nvidia.com/deeplearning/triton-inference-server/user-guide/docs/protocol/extension_binary_data.html)


## Consequências

Fica definida uma arquitetura apropriada para a implementação das funções em HTTP.
