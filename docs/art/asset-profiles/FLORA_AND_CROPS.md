# Perfil de Asset — Flora, Cultivos e Cogumelos

**ID de categoria:** `flora`  
**Carregar junto com:** `../ASSET_GENERATION_CORE.md`

## Objetivo visual
Criar plantas reconhecíveis, orgânicas e mágicas, integradas à floresta. Cultivos precisam comunicar função e fase de crescimento; flora selvagem deve enriquecer o cenário sem transformar o chão em uma decoração uniforme.

## Perspectiva e formato
- Vista top-down/3/4 coerente com o chão e a câmera do jogo.
- Plantas isoladas devem vir como sprites com alpha, sem vaso, canteiro, chão ou cena não solicitados.
- Cultivos: produzir a fase exata pedida; não combinar broto, flor, fruto maduro e raízes em um único sprite se forem fases diferentes.
- Se for solicitada uma sequência de crescimento, manter mesma câmera, base/footprint e identidade entre fases.
- Cogumelos devem ter chapéu e haste legíveis nessa perspectiva; não retratar em vista lateral pura.

## Prioridade de cores
1. Para plantas comuns, começar pela família Vegetação.
2. Para flores, escolher uma cor focal e manter folhas/haste secundárias.
3. Para flora mágica, usar violeta/lilás ou ciano em áreas delimitadas; preservar sombras e cores-base naturais.
4. Para plantas luminosas, usar a família Luz Mágica e/ou Luz Quente somente nos pontos emissivos e reflexos próximos.
5. Evitar que todas as espécies usem a mesma cor mágica; diferenciar espécies por silhueta e distribuição de cor também.

## Silhueta e foco
- Uma planta deve ser reconhecida pela forma antes de depender de detalhes internos.
- Diferenciar folhas, haste, flor, fruto, chapéu e caule por silhueta e massas de cor.
- Grupos de flores e cogumelos variam de tamanho, inclinação e espaçamento; evitar cópias idênticas organizadas uniformemente.
- Para cultivos, fase e função devem ficar claras em escala de gameplay.
- O centro de interesse deve ter contraste suficiente sem competir com o personagem.
- Manter footprint compatível com o solo, sem parecer flutuar.

## Iluminação
- Luz e sombra obedecem ao Core. Usar highlights em grupos pequenos, seguindo o volume.
- Em cogumelos luminosos, o chapéu pode ser mais claro que a haste; a emissão deve parecer ter origem no organismo.
- Glow deve ser mínimo e localizado; o sprite precisa manter leitura mesmo sem glow.
- Não usar bloom digital, blur ou aura grande para comunicar magia.

## Deve ter
- Clusters de pixels deliberados e contorno orgânico.
- Diferenças perceptíveis entre espécies.
- Separação legível entre silhueta da planta e fundo.
- Uma quantidade limitada de detalhes concentrados nos pontos focais.
- Consistência entre etapas de crescimento, quando aplicável.

## Não pode ter
- Aparência de emoji, sticker ou ilustração suave apenas reduzida.
- Textura de folhas composta por ruído uniforme.
- Glow exagerado ao redor de toda a planta.
- Cultivos ornamentais tão detalhados que sua fase/função fique menos clara.
- Paletas muito saturadas em todos os elementos.
- Vasos, terra, sombras ou acessórios extras se não foram solicitados.

## Critério de aprovação
A espécie e sua fase devem ser identificáveis no zoom normal. Cultivos devem poder ser distinguidos de flora selvagem, e plantas mágicas devem comunicar magia sem depender exclusivamente de brilho.
