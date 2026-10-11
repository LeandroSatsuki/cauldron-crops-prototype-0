# Perfil de Asset — Efeitos Mágicos e Iluminação

**ID de categoria:** `magic-effects`  
**Carregar junto com:** `../ASSET_GENERATION_CORE.md`

## Objetivo visual
Representar magia como parte da natureza: crescimento, transformação, energia localizada ou luz que revela algo. O efeito deve servir ao gameplay e à composição, não encobrir o asset de origem.

## Perspectiva e formato
- Efeitos no mundo seguem a câmera top-down/3/4 e precisam encaixar com o objeto/solo ao qual pertencem.
- Sprite de efeito isolado com alpha; não incluir fundo, personagem, fonte emissiva ou cenário que não tenha sido solicitado.
- Para animação, manter centro de emissão, escala aparente e forma consistentes entre frames. Não inventar contagem de frames.
- Criar variações de duração, intensidade ou estado apenas quando solicitadas.

## Prioridade de cores
1. Escolher uma única família emissiva principal por efeito: ciano, violeta/lilás ou luz dourada.
2. Usar a família Sombras Profundas e Atmosfera Azul para o corpo/sombra do efeito quando necessário.
3. Reservar os tons mais claros da família escolhida para o núcleo ou o ponto de maior emissão.
4. Manter o resto do efeito menos saturado e com contraste controlado.
5. Não misturar todas as famílias mágicas em um mesmo efeito por padrão.

## Forma, foco e movimento
- O núcleo de emissão deve ser identificável.
- Usar formas claras e clusters de pixels; pequenas partículas são acentos, não preenchimento total.
- Variação de tamanho/direção deve sugerir comportamento intencional, não ruído.
- Efeitos de purificação podem sugerir recuperação de cor, brotos ou luz; corrupção pode sugerir distorção/escurecimento orgânico. Evitar depender só de filtro de matiz.
- Efeito não pode ocultar o gato, o objeto interativo ou o limite funcional da área.

## Iluminação
- Brilho restrito ao núcleo e aos pixels próximos.
- Glow externo mínimo; se remover o glow, a forma principal ainda deve funcionar.
- Não usar blur, bloom fotográfico, gradientes suaves ou partículas incontáveis.
- Os raios de luz da floresta devem ser usados na composição da cena, não anexados a cada sprite.

## Deve ter
- Hierarquia clara entre núcleo, corpo e partículas.
- Paleta limitada.
- Estado/função reconhecível pela forma e pela cor.
- Transparência limpa para composição sobre o mundo.

## Não pode ter
- Tela coberta por partículas ou glow.
- Neon em excesso ou aura grande em todos os objetos.
- Mistura de cores sem hierarquia.
- Efeito genérico que poderia servir indistintamente para qualquer magia.
- Fundo opaco em efeitos que precisam ser compostos sobre o jogo.

## Critério de aprovação
O efeito comunica uma função específica, continua legível em gameplay e complementa em vez de substituir a forma do objeto ou do ambiente.
