# Cauldron Crops — Alchemy Tags

Versão: 0.1
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

### Aspectos-base propostos

- life — vida, vitalidade, matéria viva
- nature — vínculo com natureza vegetal e mundo selvagem
- growth — crescimento, germinação, desenvolvimento
- water — água, umidade, afinidade aquática
- earth — solo, pedra, matéria terrestre
- fire — calor, combustão, energia térmica
- air — vento, movimento, liberdade, respiração
- light — luminosidade, brilho, revelação
- shadow — oculto, ausência de luz, profundidade
- sun — ciclo solar, calor vital, energia diurna
- moon — ciclo lunar, noite, transformação, mistério
- spirit — consciência, alma, manifestação da vida
- magic — energia sobrenatural diretamente manipulável
- corruption — deterioração, contaminação, influência da corrupção
- cold — frio, preservação, afinidade gélida
- warmth — calor confortável, energia, acolhimento

Esses aspectos formam o vocabulário-base atual. Novos aspectos não devem ser criados para resolver uma única receita.

## 3. Regra de composição

Uma receita de descoberta deve poder ser explicada em termos de propriedades.

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
- explicar futuras descobertas;
- permitir validações;
- preparar extensibilidade.

Não criar, neste momento, um gerador automático que produza resultados para qualquer combinação de aspectos.

A criação procedural de resultados seria uma etapa futura e exigiria regras próprias.

## 5. Ingredientes iniciais — proposta

### Trigo Dourado
Tags: seed, crop, grain, food
Aspectos: life, nature, growth, sun

### Seiva Bruta
Tags: sap, liquid, material
Aspectos: life, nature, growth

### Tomate Solar
Tags: crop, fruit, food
Aspectos: life, nature, growth, sun

### Escama Brilhante
Tags: scale, material
Aspectos: water, light, magic

### Peixe Comum
Tags: fish, food
Aspectos: water, life

### Peixe Luminoso
Tags: fish, food
Aspectos: water, life, light, moon, magic

### Seiva Brilhante
Tags: sap, liquid, material
Aspectos: life, nature, growth, light, magic

### Seiva Lunar
Tags: sap, liquid, material
Aspectos: life, nature, moon, magic

### Semente de Abóbora Lunar
Tags: seed, crop
Aspectos: life, nature, growth, moon, magic

### Isca Encantada
Tags: bait, material
Aspectos: water, magic, attraction

Attraction é tratada neste momento como propriedade funcional específica, não como aspecto-base obrigatório. Sua permanência será validada quando a pesca for definida.

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