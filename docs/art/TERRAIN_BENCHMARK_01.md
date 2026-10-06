# Cauldron Crops — Terrain Benchmark 01

**Versão:** 0.2  
**Status:** experimento artístico — não final

## Objetivo

Validar a linguagem do terreno antes de produzir assets em escala.

A pergunta é:

> "Esse terreno continua parecendo Cauldron Crops quando repetido em uma área real e observado na câmera do jogo?"

## Escopo mínimo

Produzir somente:

1. terreno base;
2. 2–3 variações compatíveis;
3. uma transição para solo preparado;
4. pequena vegetação espontânea;
5. uma flor;
6. uma planta agrícola;
7. uma composição pequena em repetição.

Não produzir ainda:

- dezenas de tiles;
- múltiplos biomas;
- estações completas;
- corrupção completa;
- UI;
- grandes árvores;
- produção em massa.

## Pré-condições

Antes de gerar:

1. consultar `docs/art/VISUAL_TARGET_0.md`;
2. consultar `docs/art/ART_BIBLE.md`;
3. consultar `docs/art/TERRAIN_LANGUAGE.md`;
4. inspecionar os assets de referência aprovados disponíveis;
5. não assumir 16×16, 32×32, 64×64 ou 128×128;
6. medir a densidade aparente a partir da câmera e do contexto;
7. usar o terreno legado, quando consultado, apenas como evidência técnica/histórica, não como aprovação estética.

## Conteúdo de teste

A composição mínima deve demonstrar:

- área de baixa densidade;
- área de densidade média;
- pequeno ponto de alta densidade;
- solo cultivável integrado;
- pelo menos uma planta legível;
- espaço suficiente para o gato;
- espaço suficiente para o golem;
- espaço suficiente para o caldeirão em teste de integração.

## Teste de câmera

O benchmark deve ser avaliado em:

### Zoom próximo
Verificar materiais, pixels e acabamento.

### Zoom normal
Verificar leitura de gameplay e relação entre os objetos.

### Zoom afastado
Verificar se o terreno continua composto e se gato, planta, golem e caldeirão continuam identificáveis por silhueta, cor e posição.

Também verificar se o terreno não exige microdetalhes para parecer interessante.

## Teste de repetição

Visualizar o terreno em área suficientemente grande para detectar:

- repetição;
- padrões diagonais;
- bordas evidentes;
- excesso de ruído;
- variações que destoam;
- densidade inconsistente.

## Teste de integração

Colocar no mesmo contexto:

- terreno;
- uma planta;
- uma ferramenta;
- um golem;
- uma pequena construção/objeto;
- o caldeirão provisório de referência.

Não comparar apenas cada asset separadamente.

## Regras visuais

O terreno deve ser:

- orgânico;
- vivo;
- acolhedor;
- fantástico sem ser neon;
- rico sem ser ruidoso.

Evitar:

- aparência 8-bit;
- outline preto pesado;
- microdetalhe excessivo;
- saturação uniforme;
- ruído procedural como substituto de composição;
- padrões grandes fáceis de perceber.

## Critérios de avaliação

Avaliar o conjunto de 0–5 nos seguintes eixos:

- identidade Cauldron Crops;
- densidade de pixel;
- leitura em zoom normal;
- leitura em zoom afastado;
- repetição;
- silhueta;
- paleta;
- contraste;
- densidade;
- integração com agricultura;
- integração com criaturas;
- potencial para clima;
- potencial para territórios;
- potencial para corrupção/purificação.

Uma boa nota isolada não aprova o benchmark.

## Regra de rejeição

Rejeitar ou iterar quando:

- o terreno é bonito, mas desaparece em zoom normal;
- o tile precisa de ampliação para parecer bom;
- a repetição é perceptível rapidamente;
- a plantação desaparece;
- o gato ou o golem se confundem com o chão;
- a cena parece pertencer a outro jogo;
- a magia é transmitida apenas por brilho/efeito;
- a densidade exige detalhes que a câmera não mostra.

## Prompt operacional

"Trabalhe no Benchmark 01 de terreno de Cauldron Crops.

Antes de gerar, consulte:
- docs/art/VISUAL_TARGET_0.md
- docs/art/ART_BIBLE.md
- docs/art/TERRAIN_LANGUAGE.md

A câmera é top-down 3/4, acompanha o gato e possui zoom. O gato é visualmente pequeno na composição, com referência aproximada de 2/3 do tamanho aparente do personagem de Stardew Valley. Não copie Stardew Valley ou Sun Haven.

Não assuma resolução fixa de 16×16, 32×32, 64×64 ou 128×128. A densidade visual deve ser determinada pelo contexto e validada no Godot.

Produza somente o conjunto mínimo:
- terreno base repetível;
- 2–3 variações;
- transição para solo cultivável;
- pequena vegetação;
- uma flor;
- uma planta agrícola;
- composição pequena para teste.

Prioridade: linguagem do terreno > beleza isolada do tile.

O terreno deve ser vivo, orgânico e acolhedor, com fantasia sutil. Deve permitir áreas de respiro e variação por clusters. Não use ruído procedural como substituto de composição.

Evite aparência 8-bit, outlines pretos pesados, excesso de microdetalhes, saturação uniforme, brilho mágico excessivo e padrões grandes de repetição.

Mostre o resultado:
1. isoladamente;
2. em repetição;
3. na escala de gameplay;
4. em zoom normal e afastado.

O benchmark só será considerado aprovado depois da avaliação em contexto real."

## Resultado esperado

O benchmark precisa permitir decidir entre:

- aprovado;
- iterar;
- rejeitado.

Nenhum asset do benchmark vira automaticamente arte final do jogo.
