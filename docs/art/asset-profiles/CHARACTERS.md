# Perfil de Asset — Personagens e Criaturas

**ID de categoria:** `characters`  
**Carregar junto com:** `../ASSET_GENERATION_CORE.md`

## Objetivo visual
Criar personagens legíveis e expressivos para uma câmera elevada apontada para baixo, com inclinação moderada. O personagem é um elemento de gameplay e precisa se destacar do terreno sem parecer colado sobre o mundo.

## Perspectiva e formato
- Ver o personagem de cima, com a parte superior da cabeça/corpo visível e as laterais aparecendo só parcialmente. Pose e orientação devem fazer sentido vistos de uma câmera elevada; não usar postura frontal de retrato nem vista lateral pura.
- Para sprite isolado, fundo transparente/alpha. Não incluir cenário, chão, sombra grande, balão de fala, interface ou texto.
- Não inventar dimensões do sprite nem número de frames. Para animação, manter escala, âncora/footprint, proporções e direção da luz consistentes entre frames.
- Usar o Visual Master aprovado do gato como referência de identidade, não redesenhar a identidade ao gerar novas poses.

## Prioridade de cores
1. Preservar a paleta específica e as cores de identidade do personagem aprovado.
2. Separar personagem e ambiente com contraste de valor e temperatura, não com outline preto espesso obrigatório.
3. Usar tons de sombra do Core de forma coerente com o ambiente.
4. Cores mágicas devem corresponder à função ou identidade do personagem, não ser aplicadas indiscriminadamente.

## Silhueta, foco e proporção
- A silhueta deve ser reconhecível mesmo em uma única cor.
- Expressão e personalidade devem vir de pose, proporção e comportamento, não só de detalhes faciais.
- Manter proporções entre vistas e poses.
- Não deixar cauda, orelhas, acessórios ou efeitos importantes cortados pelo canvas.
- Evitar detalhes muito pequenos que desaparecem em movimento ou zoom normal.

## Iluminação
- Seguir a luz do Core e a iluminação da cena.
- Highlights devem reforçar volume e material sem redesenhar as cores de identidade.
- Não adicionar glow, contorno luminoso ou partículas a personagens comuns sem pedido.

## Deve ter
- Silhueta e pose legíveis.
- Identidade estável entre poses e animações.
- Escala coerente com o mundo e o gato.
- Contraste suficiente contra ambientes escuros e vegetação densa.
- Transparência limpa nas áreas externas do sprite.

## Não pode ter
- Alterar características visuais aprovadas do gato sem solicitação explícita.
- Misturar proporções, densidade de pixel ou iluminação entre frames.
- Aparência 3D, anime suave ou ilustração apenas pixelizada.
- Cenário de fundo em um sprite de personagem isolado.
- Membros ou acessórios cortados por falta de margem.
- Efeitos decorativos que prejudiquem a leitura da pose.

## Critério de aprovação
O personagem deve ser reconhecido no zoom normal, manter identidade em diferentes poses e continuar legível sobre terreno e vegetação.
