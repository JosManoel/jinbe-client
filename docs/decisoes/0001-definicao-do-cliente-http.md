# ADR-0001 — Base de implementação do projeto

**Estado:** Aceita | **Data:** 13-08-2026

## Contexto

Definir o cliente Triton Server em python (_[tritonclient](https://pypi.org/project/tritonclient/)_) como a base de implementação da biblioteca em Kotlin a ser desenvolvida.

O cliente em Python é o que possui a maior quantidade de recursos implementados, com a documentação mais robusta entre todos, sendo o ideal para a base de implementação do cliente para dispositivos móveis.

* [Documentação](https://docs.nvidia.com/deeplearning/triton-inference-server/user-guide/docs/_reference/tritonclient_api.html)

## Decisão

Optou-se por aderir a sugestão.

## Alternativas consideradas

| Alternativa | Por que não |
|---|---|
| Biblioteca [Alibaba Cloud PAI Team](https://www.alibabacloud.com/en?_p_lc=1&utm_content=se_1024016509&gclid=CjwKCAjwnvTUBhBoEiwAZNDxZ3jKFQxFVLWfrUGclGxMyK-AKQ2INCyNEU-nsL1wyRQGrXy_3eFJNRoCQ0EQAvD_BwE) | Poucos recursos implementados e biblioteca desatualizada |


## Consequências

Fica mais fácil definir um roadmap com os métodos a serem implementados.
