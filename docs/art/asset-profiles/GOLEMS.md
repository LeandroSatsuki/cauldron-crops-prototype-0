# Perfil de Asset — Golems

**ID de categoria:** `golems`  
**Carregar junto com:** `../ASSET_GENERATION_CORE.md` e, quando disponível, consultar `../GOLEM_LANGUAGE.md`.

## Objetivo visual
Golems são manifestações físicas da magia do mundo formadas através da matéria. Conceito-base: **magia + matéria → criatura**; não um humanoide pronto com textura de pedra.

## Perspectiva e formato
- Vista top-down/3/4 coerente com os personagens do jogo.
- Sprite isolado com alpha por padrão. Não incluir cenário ou base de pedestal se não for solicitado.
- A matéria deve permanecer legível na silhueta e no volume.
- Não escolher dimensões ou quantidade de frames por conta própria se o pipeline ainda não as definiu.
- Se houver animação, manter âncoras e proporções; movimento pode ser estranho/orgânico, mas os frames precisam funcionar em sequência.

## Prioridade de cores
1. Começar pela cor e pelo valor do material principal: pedra, madeira, argila, raízes, fungo ou mistura autorizada pelo conceito.
2. Usar Madeira/Pedra e Sombras Profundas para materiais naturais.
3. Usar Vegetação para musgo/folhas integradas ao corpo.
4. Violetas, cianos ou dourados devem indicar magia interna, feridas, veios ou pontos de energia específicos — não revestir o corpo todo com brilho.
5. Manter contraste suficiente para a forma funcionar em silhueta.

## Anatomia e foco
- Material cria corpo, extensões, peso, textura, cor e comportamento.
- Não começar de um esqueleto humano universal.
- A silhueta deve funcionar sem depender do rosto.
- Preferir assimetria, juntas ou extensões que pareçam ter crescido/condensado a partir do material.
- A personalidade desejada começa com estranheza; a fofura pode aparecer por contraste e comportamento, não por anatomia kawaii automática.
- Um golem deve parecer vivo, mas não uma pessoa em miniatura.

## Iluminação
- A luz externa segue o Core.
- A magia interna deve ser sutil e localizada; iluminar só as superfícies próximas quando fizer sentido.
- Não usar aura externa grande como substituto para anatomia ou material.
- Os highlights devem reforçar o material (rocha, madeira, argila etc.).

## Deve ter
- Silhueta estranha, memorável e legível.
- Material reconhecível mesmo em escala pequena.
- Relação convincente entre massa, apoio e movimento.
- Magia integrada ao corpo.
- Um equilíbrio entre mistério e simpatia, sem mascote genérico.

## Não pode ter
- Guerreiro, guardião ou boss de RPG genérico.
- Humanoide com armadura ou roupa como estrutura principal.
- Aparência de ancião humano ou adulto humano em miniatura.
- Olhos enormes como único recurso de personalidade.
- Glow em todo o contorno.
- Mistura arbitrária de materiais sem lógica física/visual.
- Reutilizar a mesma silhueta para todos os tipos de golem.

## Critério de aprovação
A criatura deve parecer ter surgido do material e da magia, ser reconhecível sem zoom e não se confundir com um NPC humano ou um objeto decorativo.
