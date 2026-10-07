# Cauldron Crops — Alchemy Tags

Versão: 0.2
Status: fundamento de design do Prototype 0

## 1. Objetivo

O sistema do caldeirão deve permitir que o jogador aprenda relações entre propriedades dos ingredientes.

A regra central é:

> Uma receita deve parecer uma consequência dos ingredientes, não uma combinação arbitrária escolhida apenas porque precisamos de determinado resultado.

O sistema recebe inspiração conceitual de jogos de descoberta por aspectos, como a ideia de identificar propriedades de itens e combiná-las para produzir novos resultados. Cauldron Crops não precisa copiar regras, nomes ou estruturas de outros jogos.

## 2. Duas camadas de informação

Cada item terá duas categorias de metadados.

### Tags funcionais

Descrevem o que o item é ou como é usado.

Exemplos:
- seed
- crop
- grain
- fruit
- fish
- food
- sap
- scale
- liquid
- bait
- potion
- material

Essas tags ajudam catálogo, coleção, UI, filtros e regras de gameplay.

### Aspectos

Descrevem propriedades conceituais e mágicas que podem participar de descobertas.

Os aspectos precisam ser relativamente estáveis ao longo do jogo.

### Aspectos fundamentais

Os aspectos devem ser **atômicos e poucos**. Eles representam propriedades que o mundo reconhece por si mesmas e que podem aparecer em muitos ingredientes.

Vocabulário-base do sistema:

- life — vida, vitalidade, matéria viva
- nature — vínculo com a natureza e o mundo vegetal
- water — água, umidade e afinidade aquática
- earth — solo, pedra e matéria terrestre
- fire — fogo, combustão e energia térmica
- air — vento, movimento e respiração
- light — luminosidade, brilho e revelação
- shadow — ausência de luz, oculto e profundidade

Esses oito aspectos são a base atual do sistema. O objetivo é manter o vocabulário pequeno o suficiente para o jogador aprender suas relações.

**Spirit** e **corruption** não são aspectos-base do Prototype 0:
- spirit representa consciência/manifestação de seres e poderá aparecer como propriedade especial de resultados ou sistemas futuros;
- corruption representa um estado do mundo e da matéria, não um elemento que todo item precisa carregar.

### Propriedades derivadas

Não transformar efeitos ou combinações conceituais em aspectos independentes sem necessidade.

Exemplos de propriedades que podem ser **derivadas** de aspectos fundamentais:

- growth — pode surgir da combinação de life + nature
- warmth/heat — expressão de fire, possivelmente combinada com life ou light
- cold — pode ser uma manifestação de water/air/shadow conforme o contexto
- sun — conceito do mundo associado principalmente a light + fire
- moon — conceito do mundo associado principalmente a light + shadow e ciclos noturnos
- spirit — estado/propriedade especial ligada a seres conscientes, não aspecto-base
- corruption — estado ambiental, não aspecto-base
- magic — não deve ser um aspecto universal; a magia é a própria forma como o mundo transforma e manifesta propriedades.
- attraction — efeito funcional de uma receita/item, não precisa virar aspecto-base

Essas relações são hipóteses de design, não fórmulas matemáticas obrigatórias. O importante é não criar um aspecto separado para cada consequência ou adjetivo.

Regra:

> **Se uma propriedade pode ser explicada naturalmente a partir de aspectos existentes, ela não deve virar um novo aspecto apenas para simplificar uma receita.**

## 3. Regra de composição

Uma receita de descoberta deve poder ser explicada em termos de aspectos fundamentais e de suas relações. O resultado pode receber uma propriedade derivada ou um significado funcional sem precisar transformar essa propriedade em um novo aspecto.

Exemplo:

Seiva Bruta
- tags: sap, liquid, material
- aspectos: life, nature, growth

Escama Brilhante
- tags: scale, material
- aspectos: water, light, magic

Logo, Seiva Bruta + Escama Brilhante pode produzir um resultado compatível com vida + natureza + brilho/magia, como Seiva Brilhante.

## 4. Tags não decidem sozinhas o resultado

Para o Prototype 0, o caldeirão usará um conjunto pequeno de receitas autoradas e determinísticas.

Os aspectos ajudam a:
- justificar a receita;
- organizar o design;
- ensinar uma linguagem reutilizável ao jogador;
- explicar futuras descobertas;
- permitir validações;
- preparar extensibilidade.

Tags funcionais continuam separadas dos aspectos. Um item pode ser uma fruta, peixe ou isca sem que cada característica funcional precise virar um aspecto alquímico.

Não criar, neste momento, um gerador automático que produza resultados para qualquer combinação de aspectos.

A criação procedural de resultados seria uma etapa futura e exigiria regras próprias.

## 5. Ingredientes iniciais — proposta

### Trigo Dourado
Tags: seed, crop, grain, food
Aspectos fundamentais: life, nature, light

### Seiva Bruta
Tags: sap, liquid, material
Aspectos fundamentais: life, nature

### Tomate Solar
Tags: crop, fruit, food
Aspectos fundamentais: life, nature, light, fire

### Escama Brilhante
Tags: scale, material
Aspectos fundamentais: water, light

### Peixe Comum
Tags: fish, food
Aspectos fundamentais: water, life

### Peixe Luminoso
Tags: fish, food
Aspectos fundamentais: water, life, light, shadow

### Seiva Brilhante
Tags: sap, liquid, material
Aspectos fundamentais: life, nature, light

### Seiva Lunar
Tags: sap, liquid, material
Aspectos fundamentais: life, nature, light, shadow

### Semente de Abóbora Lunar
Tags: seed, crop
Aspectos fundamentais: life, nature, light, shadow

### Isca Encantada
Tags: bait, material
Aspectos fundamentais: water, life, nature

O efeito de atração é uma consequência funcional da receita e não precisa de um aspecto próprio.

## 6. Regra para novas tags e aspectos

Antes de criar uma propriedade nova, responder:

1. Essa propriedade aparece em vários itens?
2. Ela pode participar de mais de uma descoberta?
3. Ela descreve uma característica real do mundo?
4. O jogador conseguiria compreender sua existência pelo contexto?
5. Ela continuará útil fora do Prototype 0?

Se a resposta for não na maioria dos casos, preferir uma tag funcional ou uma regra específica de receita em vez de criar um novo aspecto.

## 7. Regra para criação de receitas

Toda nova receita deve responder:

### Ingrediente A
O que ele traz?

### Ingrediente B
O que ele traz?

### Resultado
Qual propriedade ou transformação surge da combinação?

### Consequência
Por que o resultado importa no mundo?

Uma receita só deve ser aprovada quando essas quatro respostas forem coerentes.

## 8. Cadeia inicial do Prototype 0

A cadeia de receitas continua provisória. Ela deve ser revisada contra os aspectos fundamentais antes de ser congelada.

A cadeia candidata atual é:

Trigo Dourado + Seiva Bruta → Semente de Tomate Solar

Trigo Dourado + Tomate Solar → Poção Purificadora Fraca

Seiva Bruta + Escama Brilhante → Seiva Brilhante

Peixe Comum + Seiva Bruta → Isca Encantada

Peixe Luminoso + Seiva Brilhante → Seiva Lunar

Seiva Lunar + Semente de Tomate Solar → Semente de Abóbora Lunar

A ordem, quantidades e alguns ingredientes ainda podem ser refinados pelo design e balanceamento. O objetivo desta cadeia é validar a coerência das relações, não congelar números.

## 9. Descoberta e conhecimento

No futuro, o jogador não deve precisar memorizar uma lista externa de receitas.

O sistema pode ensinar:
- propriedades dos itens;
- categorias;
- relações entre aspectos;
- resultados descobertos;
- pistas de combinações possíveis.

No Prototype 0, basta que a descoberta seja clara e o jogador consiga formar hipóteses sobre o próximo experimento.

## 10. Filosofia

> O jogador não deveria pensar: “qual receita o jogo quer que eu faça?”

A experiência desejada é:

> “Eu conheço algumas propriedades desses ingredientes. Será que essa combinação produz alguma coisa?”

Esse comportamento é um dos principais candidatos a sustentar a curiosidade do Cauldron Crops.

## 11. Limite do Prototype 0

O Prototype 0 não precisa de:
- dezenas de aspectos;
- centenas de receitas;
- alquimia procedural completa;
- árvores complexas de dependência;
- sistema de combinações infinito;
- análise numérica avançada dos ingredientes.

Precisa somente provar que:

ingrediente → propriedades percebidas → hipótese → experimento → descoberta → consequência

é divertido e compreensível.