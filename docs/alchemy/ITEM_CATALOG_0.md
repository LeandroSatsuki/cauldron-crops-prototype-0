# Cauldron Crops — Catálogo de Itens do Prototype 0

Versão: 0.1
Status: proposta de consolidação

## 1. Objetivo

Este documento organiza os itens necessários para o Prototype 0 em quatro grupos:

- recursos naturais;
- cultivos;
- consumíveis e utilidades;
- resultados de alquimia.

O catálogo não deve crescer apenas para “ter mais conteúdo”. Cada item precisa ter uma função clara no loop ou ajudar a ensinar o mundo.

## 2. Regra importante

Nem todo item precisa possuir aspectos alquímicos.

Um item pode ser apenas funcional quando seu papel não exige participação no sistema de descobertas.

Exemplos:

- Adubo Natural pode existir como ferramenta agrícola.
- Madeira pode ser recurso de construção e também ingrediente alquímico.
- Uma poção pode ser resultado do caldeirão e, portanto, possuir uma identidade alquímica.

Não criar aspectos apenas para preencher uma ficha.

## 3. Recursos naturais

### Madeira

Tags:
- material

Aspectos:
- Natureza
- Terra

Funções:
- recurso natural próximo da vila;
- possível ingrediente alquímico;
- futuramente usado em reconstrução.

Observação:
Madeira é uma referência de combinação Natureza + Terra.

### Seiva Bruta

Tags:
- sap
- liquid
- material

Aspectos:
- Vida
- Natureza

Funções:
- ingrediente inicial do caldeirão;
- recurso encontrado em árvores e elementos naturais;
- componente de resultados alquímicos.

### Flor do Vento

Tags:
- material
- flora

Aspectos:
- Natureza
- Ar

Funções:
- recurso de exploração;
- possível ingrediente para descobertas futuras;
- referência de afinidade Natureza + Ar.

### Carvão

Tags:
- material

Aspectos:
- Terra
- Fogo

Funções:
- recurso natural/mineral simples;
- possível ingrediente para uma descoberta ligada a energia, calor ou transformação.

No Prototype 0, carvão só entra caso sua obtenção seja simples e não exija um sistema completo de mineração.

### Escama Brilhante

Tags:
- scale
- material

Aspectos:
- Água
- Luz

Funções:
- ingrediente alquímico;
- reforça a relação entre Água e Luz;
- pode ser obtida de pesca após a primeira restauração.

## 4. Cultivos

### Trigo Dourado

Tags:
- seed
- crop
- grain
- food

Aspectos:
- Vida
- Natureza
- Luz

Funções:
- primeiro cultivo;
- ingrediente da primeira descoberta;
- ensina que uma cultura mágica possui afinidades próprias.

### Tomate Solar

Tags:
- crop
- fruit
- food

Aspectos:
- Vida
- Natureza
- Luz
- Fogo

Funções:
- segundo cultivo do arco inicial;
- recurso para a Poção Purificadora Fraca;
- demonstração prática de um cultivo desbloqueado por descoberta.

### Semente de Tomate Solar

Tags:
- seed

Aspectos:
- Vida
- Natureza
- Luz
- Fogo

Funções:
- resultado da primeira descoberta;
- abre o próximo cultivo.

### Semente de Abóbora Lunar

Tags:
- seed
- crop

Aspectos:
- Vida
- Natureza
- Luz
- Sombra

Status:
- candidata para descoberta posterior;
- não é necessária para o primeiro circuito de progressão.

## 5. Pesca

### Peixe Comum

Tags:
- fish
- food

Aspectos:
- Água
- Vida

Funções:
- primeiro peixe da coleção;
- ingrediente alquímico opcional;
- ensina Água + Vida.

### Peixe Luminoso

Tags:
- fish
- food

Aspectos:
- Água
- Vida
- Luz
- Sombra

Funções:
- peixe especial;
- ingrediente para descoberta posterior;
- reforça a coexistência de Luz e Sombra no mesmo item.

A lista final de peixes continua limitada a aproximadamente 3–5 espécies.

## 6. Adubos

### Adubo Natural

Tags:
- fertilizer
- material

Aspectos:
- nenhum obrigatório

Função:
- consumível agrícola;
- melhora temporariamente o solo ou acelera o próximo ciclo de crescimento;
- cria uma utilidade para excedentes agrícolas.

Aquisição inicial recomendada:
- produzido a partir de restos de colheita e/ou recursos naturais comuns;
- não deve depender do caldeirão para existir.

Motivo:
O adubo cumpre uma função de suporte à agricultura. Transformá-lo em uma receita alquímica obrigatória adicionaria uma dependência artificial ao loop principal.

### Adubo Encantado

Status:
- futuro / não obrigatório no Prototype 0.

Ideia:
Uma versão mágica do adubo pode futuramente surgir de uma descoberta do caldeirão e introduzir efeitos específicos de solo.

Não implementar até o Adubo Natural estar funcionando e sua necessidade estar demonstrada.

## 7. Poções

As poções devem ser tratadas como resultados de transformação e não como uma lista arbitrária de buffs.

### Poção Purificadora Fraca

Tags:
- potion
- consumable

Aspectos conceituais:
- Vida
- Natureza
- Luz

Receita aprovada:
**Trigo Dourado + Tomate Solar → Poção Purificadora Fraca**

Função:
- permite purificar a primeira barreira de corrupção;
- restaura uma pequena área;
- libera exploração e pesca.

Justificativa:
Os dois ingredientes compartilham Vida, Natureza e Luz. A combinação concentra uma afinidade restauradora, expressa mecanicamente como purificação.

A purificação é um efeito do resultado. Não é necessário criar um aspecto “Corrupção” ou “Purificação”.

### Poção de Crescimento

Status:
- candidata.

Ideia:
Uma poção voltada para cultivo, ligada a Vida + Natureza e a uma manifestação de crescimento.

Função possível:
- acelerar o crescimento de uma cultura;
- aumentar temporariamente a eficiência de um solo;
- permitir uma pequena vantagem agrícola sem quebrar a economia.

Não aprovar a receita até existir uma combinação de ingredientes que explique claramente esse resultado.

### Poção de Revelação

Status:
- candidata.

Ideia:
Uma poção associada a Luz e ao ato de revelar algo oculto.

Funções possíveis:
- revelar uma memória;
- destacar uma interação ambiental;
- revelar uma pista de descoberta.

Não usar “revelação” apenas como buff genérico. A função deve estar ligada ao mundo e à descoberta.

## 8. Outros resultados de alquimia

### Seiva Brilhante

Tags:
- sap
- liquid
- material

Aspectos:
- Vida
- Natureza
- Luz

Receita candidata:
**Seiva Bruta + Escama Brilhante → Seiva Brilhante**

Função:
- resultado intermediário para outras descobertas;
- reforça que Luz pode transformar uma matéria natural sem alterar sua identidade básica.

### Seiva Lunar

Tags:
- sap
- liquid
- material

Aspectos:
- Vida
- Natureza
- Luz
- Sombra

Receita candidata:
**Peixe Luminoso + Seiva Brilhante → Seiva Lunar**

Função:
- resultado alquímico mais raro;
- possível preparação para conteúdo noturno/lunar;
- ainda não é obrigatório para a progressão principal.

### Isca Encantada

Tags:
- bait
- material

Aspectos:
- Água
- Vida
- Natureza

Receita candidata:
**Peixe Comum + Seiva Bruta → Isca Encantada**

Função:
- criar uma relação entre recurso da pesca e recurso da natureza;
- melhorar ou expandir uma tentativa de pesca.

A atração é efeito funcional. Não criar um aspecto “Atração”.

## 9. Cobertura inicial dos aspectos

A lista atual já cobre:

- Vida: Trigo Dourado, Seiva Bruta, Tomate Solar, Peixe Comum, Peixe Luminoso.
- Natureza: Trigo Dourado, Seiva Bruta, Tomate Solar, Madeira, Flor do Vento.
- Água: Escama Brilhante, Peixe Comum, Peixe Luminoso.
- Terra: Madeira, Carvão.
- Fogo: Tomate Solar, Carvão.
- Ar: Flor do Vento.
- Luz: Trigo Dourado, Tomate Solar, Escama Brilhante, Peixe Luminoso.
- Sombra: Peixe Luminoso, Seiva Lunar, Semente de Abóbora Lunar.

Ar ainda precisa de um segundo representante natural convincente. Não adicionar um item artificial somente para fechar a contagem.

## 10. Ordem recomendada para implementação

Primeiro:
- Trigo Dourado;
- Seiva Bruta;
- Madeira;
- Adubo Natural;
- Tomate Solar;
- Poção Purificadora Fraca.

Depois:
- Escama Brilhante;
- Peixe Comum;
- Peixe Luminoso;
- Flor do Vento;
- Carvão, somente se sua obtenção couber no mapa atual.

Por último:
- resultados alquímicos opcionais;
- segunda camada de poções;
- itens ligados a exploração adicional.

## 11. Regra de aprovação

Antes de adicionar um item ao Prototype 0:

1. Qual é a função dele?
2. Como o jogador obtém?
3. Ele participa de alguma descoberta ou atividade?
4. Por que ele pertence ao mundo?
5. Ele cria uma dependência nova?

Se a resposta para a última pergunta for “sim”, verificar se essa dependência é desejada. Caso contrário, o item deve ser adiado ou simplificado.
