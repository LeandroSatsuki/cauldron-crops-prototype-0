# Perfil de Asset — Pedras, Rochas e Minerais

**ID de categoria:** `rocks-minerals`  
**Carregar junto com:** `../ASSET_GENERATION_CORE.md`

## Objetivo visual
Representar materiais com peso e estrutura, integrados à floresta. Rochas comuns devem parecer minerais opacos; cristais e recursos mágicos podem ter luminosidade localizada sem transformar todas as pedras em itens mágicos.

## Perspectiva e formato
- Câmera elevada apontada para baixo: a superfície superior da pedra/cristal deve ocupar a maior parte do sprite; faces laterais são discretas e apenas sugerem volume. Evitar projeção isométrica em losangos.
- Sprite isolado com alpha por padrão. Não adicionar chão, plantas, minério solto ou partículas sem pedido.
- Grupos de pedras devem variar escala, orientação e distância; evitar conjuntos simétricos ou cópias duplicadas evidentes.
- Não assumir uma resolução fixa; manter a densidade aparente do pixel da referência aprovada.

## Prioridade de cores
1. Base opaca: família Madeira/Pedra, escolhendo cinzas e neutros para rochas.
2. Sombras: Sombras Profundas e Atmosfera Azul, conforme a iluminação.
3. Musgo e líquen: família Vegetação em pequenas regiões de contato.
4. Mineral mágico: usar violetas/lilases ou cianos como material principal apenas se a espécie for explicitamente mágica.
5. Luz quente só como reflexo/veio raro ou quando solicitado.

## Forma, material e foco
- Grandes planos e facetas devem explicar a forma da rocha.
- Usar poucos agrupamentos grandes e alguns pequenos detalhes; evitar ruído de pixels espalhado por toda a superfície.
- A borda deve ser irregular, mas estruturalmente plausível.
- Musgo e plantas devem acompanhar rachaduras, áreas úmidas ou a base; não parecerem colados aleatoriamente.
- Em grupos, uma pedra maior pode servir de foco, com menores apoiando a silhueta.

## Iluminação
- Highlights no plano superior/alto à esquerda conforme o Core; sombras mais fortes nos planos inferiores e à direita.
- Contraste suficiente para diferenciar facetas, sem contorno preto espesso universal.
- Para cristais emissivos, luz concentrada na origem e reflexo local contido. A rocha ao redor não deve ter uma aura grande por padrão.

## Deve ter
- Peso visual e planos legíveis.
- Distinção clara entre rocha, cristal, minério e musgo.
- Textura adaptada ao material e à escala.
- Leitura da silhueta quando reduzido ao tamanho real do jogo.

## Não pode ter
- Aparência de esfera lisa, metal polido ou modelo 3D renderizado.
- Facetas minúsculas distribuídas sem lógica.
- Glow uniforme ao redor de todas as pedras.
- Musgo em padrão repetitivo ou cobrindo a forma mineral principal.
- Pedras perfeitamente iguais em grupos naturais.
- Fundo/cenário quando solicitado um recurso isolado.

## Critério de aprovação
A forma e o material principal continuam legíveis sem glow. Em grupos, o conjunto deve parecer assentado no terreno e não flutuar.
