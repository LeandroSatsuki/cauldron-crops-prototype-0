# Cauldron Crops — Matriz de Aspectos do Prototype 0

Versão: 0.1
Status: revisão de design

## 1. Objetivo

Esta matriz existe para verificar se os aspectos fundamentais aparecem em uma rede de itens coerente.

Ela não é uma obrigação de implementação imediata.

A regra é:

> Não criar um item apenas para preencher uma célula vazia.

A cobertura deve surgir de itens que já possuem uma razão clara para existir.

## 2. Aspectos fundamentais

| Aspecto | Significado de design |
|---|---|
| Vida | vitalidade, força vital, organismo vivo |
| Natureza | vínculo mágico com plantas, floresta e matéria natural |
| Água | água, umidade e afinidade aquática |
| Terra | solo, pedra e matéria terrestre |
| Fogo | combustão, calor e energia térmica |
| Ar | vento, movimento e respiração |
| Luz | luminosidade, brilho e revelação |
| Sombra | ausência de luz, oculto e profundidade |

## 3. Matriz atual

| Item | Vida | Natureza | Água | Terra | Fogo | Ar | Luz | Sombra | Status |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---|
| Trigo Dourado | X | X |  |  |  |  | X |  | P0 |
| Seiva Bruta | X | X |  |  |  |  |  |  | P0 |
| Madeira |  | X |  | X |  |  |  |  | P0 |
| Tomate Solar | X | X |  |  | X |  | X |  | P0 |
| Escama Brilhante |  |  | X |  |  |  | X |  | P0 |
| Peixe Comum | X |  | X |  |  |  |  |  | P0 |
| Peixe Luminoso | X |  | X |  |  |  | X | X | P0 |
| Flor do Vento |  | X |  |  |  | X |  |  | candidato |
| Carvão |  |  |  | X | X |  |  |  | candidato |
| Semente de Tomate Solar | X | X |  |  | X |  | X |  | resultado |
| Seiva Brilhante | X | X |  |  |  |  | X |  | resultado |
| Isca Encantada | X | X | X |  |  |  |  |  | resultado |
| Seiva Lunar | X | X |  |  |  |  | X | X | candidato |
| Semente de Abóbora Lunar | X | X |  |  |  |  | X | X | candidato |

## 4. Leitura da cobertura

Vida:
- Trigo Dourado
- Seiva Bruta
- Tomate Solar
- Peixes

Natureza:
- Trigo Dourado
- Seiva Bruta
- Madeira
- Tomate Solar
- Flor do Vento

Água:
- Escama Brilhante
- Peixe Comum
- Peixe Luminoso

Terra:
- Madeira
- Carvão

Fogo:
- Tomate Solar
- Carvão

Ar:
- Flor do Vento

Luz:
- Trigo Dourado
- Tomate Solar
- Escama Brilhante
- Peixe Luminoso

Sombra:
- Peixe Luminoso
- Seiva Lunar
- Semente de Abóbora Lunar

## 5. Problemas atuais

### Ar

Ar ainda possui somente um representante claro:

**Flor do Vento → Natureza + Ar**

Não precisamos resolver isso imediatamente.

Um segundo representante deve aparecer de forma natural em exploração, fauna, flora ou outro sistema que já tenha motivo para existir.

Exemplos de direção, ainda não aprovados:
- folha ou semente carregada pelo vento;
- pluma de criatura;
- pólen ou esporo dispersado pelo vento.

Não escolher um deles somente por causa da tabela.

### Sombra

Sombra já possui múltiplos candidatos, mas o único representante claramente P0 no momento é o Peixe Luminoso.

Isso é suficiente para manter a hipótese, mas ainda não para considerar a cobertura fechada do P0.

Uma fonte natural futura pode resolver isso sem criar um item artificial.

## 6. Regra importante sobre resultados

Resultados de alquimia podem herdar, perder ou transformar aspectos.

Não existe regra de que:

> aspectos do resultado = união matemática dos ingredientes.

A combinação deve fazer sentido no mundo.

Por exemplo:

**Seiva Bruta + Escama Brilhante → Seiva Brilhante**

A Seiva Bruta traz Vida + Natureza.
A Escama Brilhante traz Água + Luz.
O resultado mantém a identidade de seiva e adquire uma expressão luminosa.

Não é necessário que Água apareça no resultado simplesmente porque estava presente na Escama.

## 7. Regra sobre propriedades derivadas

growth, warmth, heat, sun, moon, magic, attraction, purification e corruption não são aspectos fundamentais.

Eles são conceitos, efeitos ou estados derivados.

O jogador pode aprender:

**Vida + Natureza → crescimento**

sem existir um aspecto chamado Growth.

Da mesma forma:

**Vida + Luz + Natureza → purificação/restauração**

pode ser uma consequência de uma receita sem existir um aspecto Purification.

## 8. Consequência para o caldeirão

O jogador deve perceber relações como:

- Vida + Natureza → algo ligado a crescimento ou vitalidade;
- Natureza + Ar → algo ligado a vento, dispersão ou movimento;
- Água + Luz → algo aquático e luminoso;
- Luz + Sombra → algo ligado à noite, lua ou revelação do oculto;
- Terra + Fogo → algo ligado a calor, combustão ou matéria transformada.

Essas relações são linguagem de design, não fórmulas rígidas.

## 9. Critério para fechar a matriz

A matriz poderá ser considerada madura quando:

1. cada aspecto tiver mais de um representante plausível;
2. os itens tiverem função própria;
3. os aspectos participarem de mais de uma relação;
4. nenhuma combinação parecer criada artificialmente para “fechar a tabela”;
5. o jogador puder descobrir padrões por experimentação.

Até lá, a matriz é uma ferramenta de design, não uma lista de implementação obrigatória.
