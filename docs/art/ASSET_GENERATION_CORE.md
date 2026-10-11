# Cauldron Crops — Asset Generation Core

**Versão:** 0.1  
**Uso:** contexto global obrigatório do gerador de assets  
**Status:** regras operacionais do gerador; a paleta permanece em validação pelo benchmark.

Este arquivo foi escrito para ser carregado em toda solicitação de asset. Carregue também **apenas um perfil de categoria** em `asset-profiles/`. Não carregue todos os perfis de uma vez.

## 1. Identidade visual obrigatória

Cauldron Crops é um jogo 2D de pixel art refinada, cozy fantasy e floresta mística. A natureza deve parecer viva, antiga, densa e orgânica; a magia deve parecer parte do ecossistema, não um efeito decorativo aplicado por cima.

Prioridades, nesta ordem:
1. Silhueta reconhecível e função do asset.
2. Leitura na câmera real e no zoom normal.
3. Coerência com a paleta e com os materiais do jogo.
4. Luz, sombra e volume em agrupamentos deliberados de pixels.
5. Detalhes decorativos, somente quando reforçam forma, material ou magia.

## 2. Câmera, perspectiva e formato

- **Perspectiva do mundo:** top-down em 3/4, consistente com o jogo. Não usar vista lateral, isométrica em diamante ou perspectiva de câmera de primeira pessoa, salvo solicitação explícita.
- **Pixel art nativa:** desenhar com agrupamentos intencionais de pixels. Não produzir uma ilustração suave e apenas reduzi-la/pixelizá-la.
- **Entrega padrão:** um asset isolado, centralizado, em PNG com fundo transparente/alpha quando suportado. Não incluir cenário completo, moldura, texto, UI, assinatura, marca-d'água ou elementos que não foram pedidos.
- **Canvas e escala:** usar as dimensões fornecidas pelo pedido, pela referência ou pelo pipeline. Se não estiverem disponíveis, não inventar um padrão universal de 16×16, 32×32, 64×64 ou 128×128; manter proporções razoáveis e indicar que a escala ainda precisa de validação.
- **Composição:** deixar margem suficiente para não cortar silhueta, folhas, pontas, brilho essencial ou sombra de contato. Não adicionar espaço vazio excessivo ao redor do sprite.
- **Câmera e leitura:** priorizar silhueta, massas de cor, contraste e agrupamento. O asset deve continuar identificável quando reduzido para a escala normal de gameplay.
- **Variações:** só gerar spritesheet, múltiplos ângulos, poses ou variantes quando explicitamente pedido.

## 3. Paleta operacional padrão — Mystical Forest 32

Usar somente as cores abaixo por padrão. Não inventar cores intermediárias, antialiasing ou gradientes fora da paleta. Esta é a paleta operacional do gerador para testes; ela **ainda deve ser validada em conjunto no benchmark antes de ser considerada a paleta definitiva de todo o jogo**.

- **Sombras profundas:** `#101522`, `#1A2133`, `#252B43`, `#34334F`
- **Vegetação:** `#163A37`, `#205247`, `#2D6B55`, `#438366`, `#629B75`, `#8CB487`, `#C0CFA0`
- **Atmosfera azul:** `#243F5B`, `#355A7A`, `#527C9C`, `#82A4B7`
- **Violetas/lilases:** `#38294F`, `#4B3568`, `#674783`, `#8860A1`, `#B18AC2`
- **Luz mágica/ciano:** `#2B6979`, `#4196A4`, `#78C8C9`
- **Luz quente:** `#C29B59`, `#E2C77D`, `#F2E8B5`
- **Madeira/pedra neutra:** `#332C32`, `#514049`, `#70585A`, `#927879`, `#A8A4A3`, `#D0D1C8`

### Prioridade de cor

1. Escolher primeiro as cores do material principal.
2. Usar sombras profundas para volume e separação, não como contorno preto universal.
3. Usar azuis frios para sombras/planos atmosféricos quando adequado.
4. Reservar violetas e lilases para materiais mágicos, detalhes específicos ou iluminação coerente — não aplicar um filtro roxo global.
5. Ciano é acento luminoso, não cor dominante de toda a cena.
6. Tons dourados/quentes são acentos raros de luz ou foco.
7. Não é obrigatório usar todas as famílias em um asset. Usar somente as cores necessárias.
8. Se o pedido fornecer um mapeamento explícito de paleta, respeitar esse mapeamento; não introduzir novas cores.

## 4. Iluminação padrão

- Padrão operacional: luz principal suave e direcional vinda do alto à esquerda do asset; sombras mais profundas embaixo e à direita.
- Construir luz e sombra com grupos discretos de pixels e transições deliberadas, não com blur, airbrush ou gradientes digitais suaves.
- Highlights devem seguir a forma e o material; evitar linhas de brilho uniformes contornando tudo.
- Fontes mágicas podem iluminar localmente os elementos próximos, mas o brilho precisa ter uma origem visual clara.
- Não adicionar glow, aura, partículas ou raios de luz quando não forem relevantes para a categoria ou para o pedido.
- Se a referência aprovada do asset estabelecer outra direção de luz, preservar a referência e manter a consistência do conjunto.

## 5. Linguagem de pixels e materiais

- Priorizar clusters legíveis, bordas controladas, assimetria intencional e planos claros.
- Diferenciar materiais por silhueta, agrupamento, valor, temperatura e textura.
- Manter densidade aparente e escala compatíveis com os assets já aprovados.
- Textura deve descrever o material; não preencher cada área com ruído.
- Não usar outline preto grosso ao redor de todos os elementos. Contornos escuros são opcionais e devem acompanhar o material.
- Não depender de microdetalhes para que o asset seja reconhecível.

## 6. Não pode ter

- Estilo 3D renderizado, pintura suave ou ilustração digital simplesmente pixelizada.
- Perspectiva incompatível com top-down/3/4.
- Cores fora da paleta padrão sem autorização explícita.
- Antialiasing, blur ou gradientes que introduzam cores intermediárias.
- Contorno preto grosso universal.
- Saturação alta em todos os elementos, excesso de neon ou glow.
- Roxo aplicado como filtro universal de magia.
- Ruído de pixels sem função, detalhes minúsculos que desaparecem na câmera, ou texturas uniformes e repetitivas.
- Fundo, chão, cenário, texto, moldura, interface ou objetos extras não solicitados em um sprite isolado.
- Imitação direta de personagens, tiles, objetos ou composições identificáveis de outro jogo.

## 7. O que é desejável

- Silhueta forte e identificável.
- Formas naturais com irregularidade controlada.
- Paleta limitada e coerente com o material.
- Hierarquia clara de valores: sombra, base, luz e acento.
- Magia localizada e integrada à natureza.
- Detalhes concentrados em pontos focais.
- Identidade legível em tamanho pequeno e no contexto top-down/3/4.
- Consistência com o Visual Master do gato e com assets da mesma categoria.

## 8. Como o gerador deve montar o contexto

Enviar ao modelo:
1. Este arquivo `ASSET_GENERATION_CORE.md`.
2. Apenas o perfil correspondente em `asset-profiles/`.
3. A solicitação atual do usuário.
4. Uma imagem de referência, somente quando houver uma.

Não carregar perfis de outras categorias sem necessidade. Não reescrever as regras globais em cada prompt. Em caso de conflito, preservar a instrução humana mais recente e sinalizar contradições não resolvidas.

## 9. Checklist de saída

Antes de aceitar o resultado, verificar:
- A categoria e a função estão imediatamente claras?
- A perspectiva top-down/3/4 está correta?
- As cores pertencem à paleta permitida?
- A luz e a sombra seguem a regra definida?
- O fundo/alpha e o enquadramento estão corretos?
- A silhueta continua legível em escala de jogo?
- Há detalhes ou efeitos sem função?
- O asset combina com Cauldron Crops e com seu perfil específico?

**Regra final:** o perfil define como o asset deve ser construído; o pedido define o que precisa ser criado. O pedido não deve apagar a identidade global, salvo decisão explícita do autor.
