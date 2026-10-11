# Perfil de Asset — Objetos, Estruturas e Ruínas

**ID de categoria:** `props-structures`  
**Carregar junto com:** `../ASSET_GENERATION_CORE.md`

## Objetivo visual
Criar objetos com função clara e história material. Estruturas podem parecer antigas, recuperadas pela floresta e parcialmente cobertas por musgo, mas precisam continuar legíveis e utilizáveis no gameplay.

## Perspectiva e formato
- Vista top-down/3/4 consistente com o jogo. Não misturar vista frontal de catálogo com assets vistos de cima.
- Sprite isolado com alpha por padrão. Incluir chão, sombra projetada extensa, decoração ou contexto arquitetônico somente quando solicitado.
- Para estruturas maiores, preservar uma composição coerente entre partes superiores, laterais visíveis e footprint no chão.
- Não fixar dimensões universais; seguir dimensões fornecidas ou validar no benchmark.
- Não incluir texto, interface, placas legíveis ou elementos funcionais inventados sem solicitação.

## Prioridade de cores
1. Identificar primeiro o material dominante: pedra, madeira, metal, cerâmica ou material orgânico.
2. Usar Madeira/Pedra para materiais naturais e arquitetônicos.
3. Usar Sombras Profundas e Atmosfera Azul para recessos e planos em sombra.
4. Vegetação para musgo, raízes e plantas que realmente crescem sobre a estrutura.
5. Violetas/cianos/dourados somente em partes mágicas específicas; não cobrir todo o objeto com uma cor de efeito.

## Foco e hierarquia
- A silhueta comunica a função antes dos detalhes.
- Um objeto central de gameplay precisa de prioridade visual proporcional à importância.
- O caldeirão é um instrumento ancestral de descoberta: natural, mágico, robusto e legível, sem aparência tecnológica.
- Ruínas devem sugerir idade por desgaste, rachaduras, musgo e irregularidade controlada; evitar dano aleatório em todas as superfícies.
- Decorar somente onde ajuda a contar a história do objeto.

## Iluminação
- Seguir o Core e manter a mesma direção de luz entre peças que serão usadas juntas.
- Planos superiores recebem mais luz; reentrâncias e partes inferiores recebem sombra.
- Evitar brilho de contorno; highlights devem descrever arestas e materiais.
- Em itens mágicos, a fonte emissiva deve ser localizada e não apagar a silhueta.

## Deve ter
- Função visual reconhecível.
- Material legível e detalhe em nível moderado.
- Desgaste coerente com uso, idade e exposição.
- Integração com raízes/musgo quando o contexto é uma ruína florestal.
- Silhueta legível no zoom normal.

## Não pode ter
- Aparência de prop 3D isométrico/renderizado.
- Contorno preto espesso e uniforme.
- Ornamentos ou runas sem função visual clara em todo o objeto.
- Excesso de musgo escondendo a forma.
- Efeitos mágicos que dominem a estrutura.
- Perspectiva inconsistente entre peças.
- Cenário extra em um sprite isolado.

## Critério de aprovação
O objeto continua identificável e funcional na câmera do jogo, combina com materiais vizinhos e não exige ampliação para ser compreendido.
