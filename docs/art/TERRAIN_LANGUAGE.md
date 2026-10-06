# Cauldron Crops — Terrain Language

**Versão:** 0.2  
**Status:** direção conceitual; não congelado

## 1. Princípio central

> O terreno deve parecer vivo, composto e específico do lugar, mas nunca parecer um conjunto aleatório de detalhes.

A identidade nasce de regras compartilhadas.

## 2. O que deve permanecer consistente

Entre diferentes regiões e estados do mundo, devem permanecer reconhecíveis:

- densidade de pixel;
- escala visual;
- linguagem de silhuetas;
- tratamento de luz e sombra;
- lógica de contraste;
- filosofia de repetição;
- relação entre terreno e vegetação;
- leitura do solo cultivável;
- tratamento de transições;
- integração com os demais assets.

## 3. Camadas

O terreno pode ser pensado em camadas:

1. terreno base;
2. variações de superfície;
3. transições;
4. solo cultivável;
5. vegetação espontânea;
6. elementos locais;
7. estado ambiental;
8. clima/evento;
9. iluminação/efeitos.

Nem toda célula precisa conter todas as camadas.

## 4. Terreno base

A textura base deve ser estável e relativamente discreta.

Precisa:

- preencher grandes áreas;
- repetir sem padrão evidente;
- sustentar objetos e personagens;
- permitir leitura de agricultura;
- possuir textura suficiente para não parecer vazia;
- não competir com landmarks.

Evitar:

- padrões grandes facilmente reconhecíveis;
- ruído uniforme;
- contraste exagerado;
- aparência 8-bit não intencional;
- textura tão detalhada que domine a tela.

## 5. Variações

Variação deve acontecer em clusters, não em distribuição perfeitamente uniforme.

Exemplos:

- pequenos grupos de grama;
- diferenças sutis de tonalidade;
- pedras;
- folhas;
- flores;
- manchas;
- pequenas áreas de solo exposto.

A variação deve parecer composta.

## 6. Repetição

A repetição é inevitável.

O objetivo não é eliminá-la matematicamente, e sim torná-la visualmente discreta.

Combinar:

- tiles alternativos;
- microvariações controladas;
- vegetação;
- clusters;
- áreas de respiro;
- mudança de densidade;
- elementos de cenário.

Não adicionar detalhes somente para esconder repetição.

## 7. Densidade visual

A densidade deve ser deliberada.

### Baixa densidade
Descanso visual e leitura de gameplay.

### Média densidade
Estado normal do ambiente.

### Alta densidade
Landmarks, bordas, pontos especiais, magia localizada e eventos.

## 8. Vegetação espontânea

Vegetação pequena deve funcionar como parte do terreno.

Pode incluir:

- tufos de grama;
- flores;
- folhas;
- pequenas plantas;
- cogumelos;
- pequenos arbustos;
- brotos;
- elementos mágicos raros.

A distribuição deve considerar:

- proximidade de landmarks;
- caminhos;
- áreas cultiváveis;
- interesse do jogador;
- visibilidade na câmera.

## 9. Áreas de respiro

Nem todo espaço precisa de detalhe.

Áreas relativamente simples ajudam:

- leitura do gato;
- leitura de plantações;
- navegação;
- contraste;
- composição.

> Detalhe só é valioso quando existe espaço visual para percebê-lo.

## 10. Caminhos

Caminhos devem parecer consequência de uso.

Preferir:

- desgaste;
- pequenas diferenças de cor;
- bordas orgânicas;
- vegetação reduzida;
- pedras ou folhas ocasionais.

Evitar faixas artificiais sobre a grama.

## 11. Solo cultivável

O solo preparado precisa ser imediatamente distinguível, mas integrado.

A diferença pode vir de:

- cor;
- textura;
- borda;
- umidade;
- pequenas marcas.

Relação desejada:

**terreno → solo preparado → planta**

e não:

**grama → quadrado marrom → sprite de planta**.

## 12. Clima e estações

Clima e estações devem alterar a sensação sem destruir a base.

Podem modificar:

- brilho;
- temperatura;
- saturação;
- umidade;
- densidade;
- flores;
- folhas;
- iluminação;
- elementos temporários.

Evitar trocar toda a identidade visual a cada estado ambiental.

## 13. Territórios

Territórios devem se diferenciar por combinação de:

- paleta;
- espécies;
- densidade;
- materiais;
- composição;
- clima;
- iluminação.

Não depender de uma única cor.

## 14. Magia

Magia pode surgir como:

- mudança localizada de cor;
- plantas incomuns;
- crescimento anormal;
- pequenas fontes luminosas;
- raízes;
- cristais;
- partículas raras;
- alteração de iluminação.

> Magia modifica a natureza; não deve simplesmente sobrepor efeitos sobre ela.

## 15. Corrupção

Corrupção deve alterar o sistema ambiental.

Pode afetar:

- vegetação;
- solo;
- pedras;
- raízes;
- água;
- iluminação;
- densidade;
- composição.

Conceitualmente:

**saudável → contaminado → fortemente corrompido**

## 16. Purificação

Purificação deve parecer restauração da vida.

Pode reintroduzir:

- vegetação;
- cor;
- água;
- flores;
- criaturas;
- elementos mágicos;
- iluminação mais saudável.

Evitar transformação baseada apenas em troca de textura quando a transição puder ser percebida.

## 17. Proceduralidade

Proceduralidade pode controlar distribuição.

Regra:

> assets definem aparência; sistemas definem distribuição.

Proceduralidade não deve inventar identidade visual arbitrariamente.

## 18. Shader

Shaders podem ajudar em:

- clima;
- transições;
- variações sutis;
- estados temporários.

Não devem substituir arte específica quando a mudança exige forma ou composição diferente.

## 19. Relação com agricultura e criaturas

Em áreas cultivadas, reduzir decoração onde ela prejudicar:

- brotos;
- plantas maduras;
- frutos;
- ferramentas;
- golems;
- navegação.

O terreno é o contexto das criaturas. Não esconder silhuetas com decoração ou efeitos.

## 20. Teste de câmera

O terreno deve ser avaliado na câmera real.

### Zoom normal
A textura não pode competir com os elementos interativos.

### Zoom afastado
O terreno deve continuar composto por massa, cor e densidade, mesmo quando pequenos detalhes somem.

### Zoom próximo
O acabamento não pode parecer incompleto ou excessivamente simplificado.

## 21. Critérios de sucesso

- não parecer tile genérico;
- não denunciar repetição rapidamente;
- não parecer 8-bit sem intenção;
- não dominar a tela;
- suportar diferentes paletas;
- suportar diferentes densidades;
- permitir leitura de agricultura;
- permitir leitura de criaturas;
- aceitar clima e eventos;
- aceitar mudança de território;
- aceitar corrupção/purificação;
- continuar reconhecível como Cauldron Crops.
