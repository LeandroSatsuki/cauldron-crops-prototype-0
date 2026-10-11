# Perfil de Asset — Terreno e Caminhos

**ID de categoria:** `terrain`  
**Carregar junto com:** `../ASSET_GENERATION_CORE.md`

## Objetivo visual
Criar superfícies que façam a floresta parecer um lugar vivo e contínuo, sem competir com gato, cultivos, criaturas ou objetos interativos.

## Perspectiva e formato
- Tiles e superfícies vistos pela câmera top-down/3/4 do jogo; o chão é visto predominantemente de cima.
- Para tiles, entregar a unidade ou conjunto solicitado sem inclinar o plano do chão para uma perspectiva lateral.
- Preservar bordas compatíveis para repetição quando o pedido for por tile seamless.
- Fundo transparente para peças isoladas; não adicionar árvores, pedras ou flores que não foram solicitadas.
- Não assumir dimensão fixa do tile se o pedido não a especificar.

## Prioridade de cores
1. Usar os verdes escuros e médios da família Vegetação como base para grama/solo vivo.
2. Usar cores de Madeira/Pedra para terra exposta, trilhas e bordas minerais, escolhendo pela função material.
3. Reservar Atmosfera Azul para sombras frias, umidade ou profundidade, não para pintar todo o chão de azul.
4. Usar violeta/ciano/dourado apenas em terrenos mágicos ou estados específicos solicitados.
5. Manter contraste menor no terreno-base do que em itens interativos.

## Composição e foco
- Base visual discreta e estável; variação organizada em clusters.
- Distribuir grama, manchas, folhas e flores de forma irregular, sem ruído uniforme.
- Caminhos devem surgir organicamente da redução de vegetação, desgaste, diferença de superfície ou pedras ocasionais.
- Preservar áreas de respiro e espaços necessários para movimentação, plantio e leitura do gato.
- Camadas possíveis: base, variação de superfície, transição, solo cultivável, vegetação espontânea, elementos locais e estado ambiental. Usar apenas as necessárias.

## Iluminação
- A superfície deve seguir a luz global definida no Core.
- Variar o valor das manchas para sugerir relevo sem parecer 3D renderizado.
- Não desenhar uma sombra individual em cada pequeno tufo se isso criar ruído.
- Efeitos de sol, chuva ou magia só quando pedidos ou quando fizerem parte do estado ambiental descrito.

## Deve ter
- Textura suficiente para não parecer uma cor sólida.
- Repetição discreta, escala consistente e leitura clara de transições.
- Diferenças funcionais claras entre grama, solo cultivável, trilha, pedra e solo corrompido.
- Variação agrupada, não distribuição perfeitamente uniforme.

## Não pode ter
- Padrão de repetição óbvio, ruído em cada pixel ou contraste excessivo.
- Flores/decorativos cobrindo áreas de gameplay ou escondendo plantas pequenas.
- Tile que parece um quadrado marrom colocado por cima de grama sem integração.
- Caminhos retos e artificiais, salvo solicitação.
- Elementos de cenário embutidos em um tile-base sem pedido.
- Textura de solo mais chamativa que os elementos interativos.

## Critério de aprovação
Testar em repetição e na câmera normal. O tile deve se integrar aos vizinhos sem costuras visíveis, manter leitura e não denunciar repetição rapidamente.
