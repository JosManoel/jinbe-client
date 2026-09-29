# Definição de Preparado e de Pronto

## Definição de Preparado (DoR)

Um item só entra em sprint se:

- [ ] Está escrito como **resultado**, não como atividade
- [ ] Tem critério de aceitação verificável por alguém que não o escreveu
- [ ] Tem `Tamanho` P ou M. Item G volta para ser quebrado
- [ ] Se toca uma decisão de projeto, a ADR existe e está `Aceita`
- [ ] Se `Risco: Alto`, declara **o que se aprende se falhar**

## Definição de Pronto (DoD)
### História ou Tarefa de código

- [ ] Critérios de aceitação satisfeitos, verificados por outra pessoa
- [ ] CI verde no job do componente
- [ ] Teste automatizado que **falharia** sem a mudança
- [ ] Se mudou `contratos/`, os três componentes atualizados **no mesmo PR**
- [ ] PR revisado por alguém que não escreveu o código
- [ ] Uso de IA declarado no PR

### Defeito

- [ ] Teste que reproduz o defeito, escrito **antes** da correção
- [ ] Causa raiz descrita na issue, em uma frase
- [ ] Se a causa raiz foi decisão de projeto, ADR revisada ou nova ADR aberta

### Decisão

- [ ] ADR escrita, com a seção de alternativas **preenchida**
- [ ] Consequências negativas listadas; uma ADR sem custos declarados volta para revisão
- [ ] Estado `Aceita` e índice atualizado

### Débito técnico

- [ ] Descreve o custo de não resolver, e não apenas o que se deseja melhorar
- [ ] Tem gatilho: *"resolver quando X acontecer"*

## Sobre uso de inteligência artificial

O Jinbe-Client usa IA generativa e declara isso. A mesma regra vale para as entregas:

- Declarar **onde** foi usada, no corpo do PR
- A autoria e a responsabilidade são de quem submete
- Código assistido por IA passa pela mesma revisão. Não há via expressa
- Não usar `Co-Authored-By:` para ferramentas, já que a coautoria é uma afirmação de
  titularidade e de responsabilidade
