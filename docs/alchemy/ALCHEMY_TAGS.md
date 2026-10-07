# Cauldron Crops — Alchemy Tags

Versão: 0.3
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
- fertilizer

Essas tags ajudam catálogo, coleção, UI, filtros e regras de gameplay.

### Aspectos

Descrevem propriedades conceituais e mágicas que podem participar de descobertas.

Os aspectos precisam ser relativamente estáveis ao longo do jogo.

### Aspectos fundamentais

Vocabulário-base:

- life — vida, vitalidade, matéria viva
- nature — vínculo com a natureza e o mundo vegetal
- water — água, umidade e afinidade aquática
- earth — solo, pedra e matéria terrestre
- fire — fogo, combustão e energia térmica
- air — vento, movimento e respiração
- light — luminosidade, brilho e revelação
- shadow — ausência de luz, oculto e profundidade

Esses oito aspectos são a base atual do sistema.

### Regras fechadas

- Aspectos representam afinidades mágicas, não propriedades físicas universais.
- Um item pode carregar 1, 2 ou 3 aspectos; mais de 3 exige justificativa forte.
- Cada aspecto deve aparecer em pelo menos dois itens relevantes quando a cobertura do sistema estiver madura.
- Não criar itens artificialmente apenas para preencher cobertura.
- Um mesmo item pode representar vários aspectos.
- Propriedades derivadas, efeitos de gameplay e estados do mundo não viram automaticamente novos aspectos.
- Tags funcionais permanecem separadas dos aspectos.

Spirit e corruption não são aspectos-base:
- spirit representa consciência/manifestação de seres e poderá aparecer como propriedade especial;
- corruption representa um estado do mundo e da matéria.

## 3. Propriedades derivadas

Não transformar efeitos ou combinações conceituais em aspectos independentes sem necessidade.

Exemplos:

- growth — pode surgir da combinação de life + nature;
- warmth/heat — expressão de fire, possivelmente combinada com life ou light;
- cold — pode ser manifestação de water/air/shadow conforme o contexto;
- sun — conceito associado principalmente a light + fire;
- moon — conceito associado principalmente a light + shadow e ciclos noturnos;
- spirit — estado/propriedade especial ligada a seres conscientes;
- corruption — estado ambiental;
- magic — não é aspecto universal;
- attraction — efeito funcional;
- purification — efeito funcional.

Regra:

> Se uma propriedade pode ser explicada naturalmente a partir de aspectos existentes, ela não deve virar um novo aspecto apenas para simplificar uma receita.

## 4. Regra de composição

Uma receita deve poder ser explicada em termos dos aspectos dos ingredientes e de uma transformação coerente.

Não existe regra de que:

> aspectos do resultado = união matemática dos ingredientes.

Um resultado pode:
- preservar aspectos;
- perder aspectos;
- ganhar uma expressão derivada;
- mudar sua função;
- mudar de forma ou categoria.

O resultado precisa continuar fazendo sentido dentro do mundo.

## 5. Ingredientes de referência

### Trigo Dourado
Tags: seed, crop, grain, food
Aspectos: life, nature, light

### Seiva Bruta
Tags: sap, liquid, material
Aspectos: life, nature

### Madeira
Tags: material
Aspectos: nature, earth

### Tomate Solar
Tags: crop, fruit, food
Aspectos: life, nature, light, fire

### Escama Brilhante
Tags: scale, material
Aspectos: water, light

### Peixe Comum
Tags: fish, food
Aspectos: water, life

### Peixe Luminoso
Tags: fish, food
Aspectos: water, life, light, shadow

### Flor do Vento
Tags: material, flora
Aspectos: nature, air

### Carvão
Tags: material
Aspectos: earth, fire

### Semente de Tomate Solar
Tags: seed
Aspectos: life, nature, light, fire

### Seiva Brilhante
Tags: sap, liquid, material
Aspectos: life, nature, light

### Isca Encantada
Tags: bait, material
Aspectos: water, life, nature

### Seiva Lunar
Tags: sap, liquid, material
Aspectos: life, nature, light, shadow

### Semente de Abóbora Lunar
Tags: seed, crop
Aspectos: life, nature, light, shadow

## 6. Adubo

### Adubo Natural

Tags:
- fertilizer
- material

Aspectos:
- nenhum obrigatório

O Adubo Natural é uma utilidade agrícola e não precisa ser um resultado de alquimia.

Função:
- transformar excedentes agrícolas em recurso útil;
- melhorar temporariamente uma plantação;
- reduzir desperdício de colheita.

A implementação inicial recomendada é simples e determinística. O adubo não deve ser requisito da progressão principal.

Uma versão mágica poderá existir no futuro, mas somente se houver uma descoberta que a justifique.

## 7. Regras para receitas

Toda nova receita deve responder:

### Ingrediente A
O que ele traz?

### Ingrediente B
O que ele traz?

### Resultado
Qual transformação surge?

### Consequência
Por que o resultado importa no mundo?

Exemplos atualmente bem justificados:

**Trigo Dourado + Seiva Bruta → Semente de Tomate Solar**

Vida + Natureza estão fortemente presentes nos dois ingredientes, enquanto a Luz do trigo aponta para uma manifestação solar. O resultado abre uma nova cultura.

**Trigo Dourado + Tomate Solar → Poção Purificadora Fraca**

Os dois ingredientes possuem Vida + Natureza + Luz. A combinação concentra uma afinidade restauradora, traduzida em purificação do ambiente.

**Seiva Bruta + Escama Brilhante → Seiva Brilhante**

A seiva oferece matéria natural viva; a escama oferece uma manifestação luminosa ligada à água. O resultado continua sendo seiva, mas agora possui expressão de luz.

**Peixe Comum + Seiva Bruta → Isca Encantada**

O peixe fornece Água + Vida e a seiva fornece Vida + Natureza. O resultado combina vida aquática e matéria natural em um item funcional para pesca.

As demais receitas continuam candidatas até que sua transformação tenha uma justificativa igualmente clara.

## 8. Cadeia atual

A cadeia de progressão obrigatória permanece:

1. Trigo Dourado + Seiva Bruta → Semente de Tomate Solar
2. cultivar Tomate Solar
3. Trigo Dourado + Tomate Solar → Poção Purificadora Fraca
4. usar a poção na primeira barreira
5. restaurar a área
6. liberar exploração e pesca

Receitas paralelas podem existir sem bloquear essa progressão.

Candidatas:
- Seiva Bruta + Escama Brilhante → Seiva Brilhante
- Peixe Comum + Seiva Bruta → Isca Encantada
- Peixe Luminoso + Seiva Brilhante → Seiva Lunar
- Seiva Lunar + Semente de Tomate Solar → Semente de Abóbora Lunar

Essas receitas permanecem sujeitas a revisão de design.

## 9. Descoberta e conhecimento

O jogador deve aprender:

- propriedades dos itens;
- categorias;
- relações entre aspectos;
- resultados descobertos;
- pistas para novas hipóteses.

A meta não é memorizar uma lista externa de receitas.

A experiência desejada é:

> “Eu conheço algumas propriedades desses ingredientes. Será que essa combinação produz alguma coisa?”

## 10. Limite do Prototype 0

O Prototype 0 não precisa de:

- dezenas de aspectos;
- centenas de receitas;
- alquimia procedural completa;
- árvores complexas de dependência;
- combinações infinitas;
- análise numérica avançada.

Precisa provar:

ingrediente → propriedades percebidas → hipótese → experimento → descoberta → consequência

é divertido e compreensível.
