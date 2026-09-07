# Proposta — Jinbe Client

## 1. Visão do produto

```
Para         Desenvolvedores de aplicações Android
Que          querem implementar soluções utilizando o Triton Inference Server
O            Jinbe-Client é uma biblioteca em Kotlin
Que          implementa um cliente Triton Inference com suporte a gRPC
Diferente da biblioteca em Java disponibilizada pela Alibaba Cloud PAI Team.
```

**Hipótese de valor:** acreditamos que o uso de uma biblioteca própria em vez do uso do protoc compiler pode trazer benefícios para o desenvolvimento de aplicações android que dependem de servidores de inferência por redes neurais.

---

## 2. MVP

**No MVP**
* Busca por modelos ou calculadoras disponíveis
* Status dos modelos ou calculadoras disponíveis
* Solicitação de inferência via HTTP 
* Solicitação de inferência via gRPC
* Receber e decodificar resposta do servidor de inferência
* Documentação dos métodos implementados

**Fora do MVP**
* Servidor de testes Triton Server
  * Implementa modelo de detecção de faces
* Aplicação móvel de exemplo
  * Escolhe servidor de inferência
  * Envia imagem em tempo real via HTTP
  * Envia imagem em tempo real via gRPC
  * Exibe a face detectada


> O que fica de fora do MVP é apenas referente a demonstrativo da biblioteca desenvolvida.

---

## 3. Backlog inicial

| Prio | História | Critérios de aceitação | Sprint |
|---|---|---|---|
| P1 | Como desenvolvedor, quero saber o status do meu servidor | Recupera status do servidor; sem resultado, mostra sem servidor disponível | 1 |
| P1 | Como desenvolvedor, quero saber os modelos disponíveis no meu servidor | Recupera os modelos do servidor; sem resultado, mostra sem modelos disponíveis | 1 |
| P1 | Como desenvolvedor, quero realizar requisições de inferências por HTTP  | Realiza inferência por HTTP a partir do modelo, caso servidor disponível | 1 |
| P2 | Como desenvolvedor, quero realizar requisições de inferências por gRPC  | Realiza inferência por gRPC a partir do modelo, caso servidor disponível | 2 |

---

## 4. Decisões técnicas, por disciplina

Em [`docs/acordo-de-processo.md`](../docs/acordo-de-processo.md).

---

## 5. Equipe

| Nome | Matrícula | Papel |
|---|---|---|
| José Manoel Freitas da Silva | 20220039467 | Product Owner e desenvolvedor |

---

## 6. Coorte e integração

**Coorte:** B, remoto.

**Integração entre disciplinas:** Não possui integração com outras disciplinas.
