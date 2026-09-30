# ADR-0002 — Determina o motor de requisições HTTP

**Estado:** Aceita | **Data:** 29-09-2026

## Contexto

Definir o motor de requisições HTTP que será utilizado para a implementação das funcionalidades em HTTP.


## Soluções

**Ktor Client**

* Prós:
    * Nativo com Coroutines (processamento assíncrono);
    * Suporte ao KMP;
    * Sintaxe limpa;
* Contras:
    * Muito minimalista (necessário implementar outros plugins);

**OkHttp**

* Prós:
    * Padrão de indústria;
    * Gerenciamento de rede otimizado;
* Contras:
    * API Java-First;

## Decisão

Optou-se por aderir ao Ktor por oferecer suporte nativo a processamento assíncrono e maior suporte a aplicações Android em Kotlin.

[Documentação](https://ktor.io/docs/welcome.html)

## Alternativas consideradas

| Alternativa | Por que não |
|---|---|
|OkHttp | API Java-First |

## Consequências

Fica definida uma arquitetura apropriada para a implementação das funções em HTTP.


