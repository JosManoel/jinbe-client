# Acordo de processo — Jinbe-Client
> O acordo de processo considera apenas uma pessoa.
---

## Cadência

| | |
|---|---|
| Duração da sprint | 3 semanas, alinhada ao cronograma da disciplina |
| Planejamento | Primeira segunda-feira da sprint, 15 min |
| Fechamento | Sexta-feira da última semana, 23:59 |
| Revisão e retrospectiva | Segunda seguinte à entrega |

---

## Definição de Pronto

Um item sai de "Em revisão" quando **todos** os itens abaixo são verdade:

- [ ] Código integrado na `main`
- [ ] Revisado no pull request (conflitos)
- [ ] Pipeline de CI verde no job do componente tocado
- [ ] Critérios de aceitação do item verificados

---

## Papéis

| Papel | Quem | Responsabilidade |
|---|---|---|
| Product Owner | José Manoel | Ordena o backlog; aceita ou recusa itens |
| Desenvolvimento | José Manoel | Constrói o incremento |

---

## Ferramentas

| Para quê | Onde |
|---|---|
| Backlog e quadro | GitHub Projects |
| Decisões | `docs/decisoes/`, em ADRs |
| Métricas de fluxo | Insights do GitHub Projects |
| Código e revisão | GitHub, com pull request obrigatório |

---

## Limites de trabalho em progresso

| Coluna | WIP máximo |
|---|---|
| Em progresso | 1 por pessoa |
| Em revisão | 1 no total |

---

## Como mediremos

| Métrica | De onde vem | Para quê |
|---|---|---|
| Itens concluídos por sprint | Quadro | Previsão, a partir da terceira sprint |
| Tempo em "Em revisão" | Histórico do quadro | Detectar revisão como gargalo |
| Itens parados > 1 semana | Visão *Parados* | Pauta automática da retrospectiva |

