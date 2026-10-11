# Perfil de Asset — Vegetação, Árvores e Copas

**ID de categoria:** `vegetation`  
**Carregar junto com:** `../ASSET_GENERATION_CORE.md`

## Objetivo visual
Transmitir floresta densa, viva, antiga e orgânica. A vegetação deve envolver clareiras e caminhos; o mundo não deve parecer uma fazenda aberta com árvores decorativas ao redor.

## Perspectiva e formato
- Usar câmera top-down/3/4: a copa é vista de cima, mas tronco, raízes e volume podem sugerir profundidade de modo consistente.
- Árvore ou arbusto isolado: sprite centralizado com alpha, sem chão ou cenário extra, a menos que seja solicitado.
- Não escolher resolução universal; preservar escala e densidade de pixels dos exemplos aprovados.
- Em árvores altas, a copa e o tronco precisam ser pensados como um conjunto espacial coerente; não mudar o ângulo de câmera entre copa e base.
- Para asset de copa isolada, não acrescentar tronco, raízes, flores ou pedras sem pedido explícito.

## Prioridade de cores
1. Verdes escuros e profundos para massa principal e áreas sob a copa.
2. Verdes médios para planos iluminados e grupos de folhas.
3. Verdes claros para pequenos highlights, sem distribuir uniformemente.
4. Azuis profundos/atmosféricos para sombras frias e planos afastados quando necessários.
5. Violetas/lilases apenas para espécies mágicas ou detalhes intencionais.
6. Ciano e dourado somente em flora mágica, orvalho ou luz especial solicitada.

## Silhueta, densidade e foco
- Formar copas por grandes grupos orgânicos, com irregularidade controlada.
- Usar variação de escala e orientação para evitar aparência de bolinhas idênticas.
- Preferir assimetria e massas de folhas conectadas a pequenas folhas isoladas.
- Árvores grandes podem formar uma moldura escura nas bordas da floresta; não devem bloquear caminhos ou pontos interativos importantes sem intenção de composição.
- Manter vazios funcionais para caminhos, interação e leitura dos personagens.
- Musgo, raízes e vegetação baixa devem parecer ligados ao tronco/terreno, não adesivos soltos.

## Iluminação
- Aplicar a luz do Core em grupos de folhas e planos de copa, não como contorno luminoso completo.
- A sombra deve ter massas claras; evitar salpicar muitos highlights individuais.
- Em cenas de floresta, raios de luz são elementos de composição do ambiente, não parte obrigatória de cada sprite de árvore.
- Brilho interno só quando espécie ou pedido justificar.

## Deve ter
- Silhueta legível em zoom normal.
- Variação de densidade e grupos de folhas reconhecíveis.
- Volume sugerido por contraste entre planos, não por gradiente suave.
- Material consistente entre copas, arbustos, trepadeiras, raízes e musgo.
- Opções de variação compatíveis, sem parecerem espécies de outro jogo.

## Não pode ter
- Copas perfeitamente circulares e repetidas por padrão.
- Folhas distribuídas como ruído uniforme ou escamas idênticas.
- Outline preto grosso em todas as folhas.
- Rosa, roxo ou ciano aplicado à vegetação inteira por padrão.
- Glow em todas as árvores.
- Microfolhas que desaparecem no zoom de gameplay.
- Assets com a mesma silhueta apenas recoloridos, salvo variantes solicitadas.

## Critério de aprovação
Verificar em grupo e no cenário, não apenas isoladamente. As copas devem ajudar a criar densidade e profundidade sem esconder o gato, confundir colisões ou dominar a leitura do caminho.
