# Perfil de Asset — Ícones de Recursos e Inventário

**ID de categoria:** `resource-icons`  
**Carregar junto com:** `../ASSET_GENERATION_CORE.md`

## Objetivo visual
Criar ícones de leitura imediata para itens, ingredientes, materiais e recursos. Cada ícone deve ser reconhecível e distinguível na interface sem abandonar a linguagem de pixel art do mundo.

## Perspectiva e formato
- Usar uma vista top-down/3/4 simplificada e consistente; a orientação pode ser mais frontal em objetos cuja forma só seja reconhecida assim, mas não alternar sem motivo entre ícones da mesma família.
- Um item por canvas por padrão, centralizado, com alpha.
- Não incluir slot de inventário, borda de UI, texto, legenda, número, sombra de cartão ou fundo.
- Manter margem suficiente e não cortar pontas, folhas ou acessórios.
- Não assumir dimensões fixas sem especificação do inventário/pipeline.

## Prioridade de cores
1. Preservar a cor intuitiva do material/objeto quando relevante para reconhecimento.
2. Aplicar as famílias do Core para sombras e luz.
3. Usar cor mágica como distinção funcional, não como filtro global.
4. Usar poucas cores por ícone; preferir massa de cor clara e contraste forte ao microdetalhe.
5. Ícones da mesma família devem partilhar lógica de iluminação e nível de saturação.

## Foco e detalhe
- Um objeto principal por imagem.
- A silhueta deve ser compreendida rapidamente em tamanho pequeno.
- Limitar detalhes internos a um ou dois grupos visuais importantes.
- Distinguir itens parecidos por forma ou acento de cor consistente, não apenas por textura minúscula.
- Sombra de contato discreta apenas se fizer parte do estilo do conjunto.

## Iluminação
- Seguir a iluminação do Core, mas simplificar a hierarquia para tamanhos pequenos.
- Uma região clara, uma base e uma sombra geralmente bastam; adicionar mais níveis apenas se necessários.
- Não usar glow para aumentar artificialmente a legibilidade de todos os itens.

## Deve ter
- Silhueta instantaneamente reconhecível.
- Forte leitura em tamanho de UI.
- Quantidade de detalhe compatível com o canvas.
- Consistência de perspectiva, luz e contorno dentro da família.

## Não pode ter
- Múltiplos itens sem pedido.
- Texto ou rótulos embutidos.
- Fundo ou tile de inventário.
- Microdetalhes que somem no tamanho final.
- Render 3D, perspectiva ou direção de luz diferentes dos outros ícones.
- Cores fora da paleta operacional sem autorização explícita.

## Critério de aprovação
O ícone deve ser identificável no tamanho real da UI e diferenciado de outros recursos próximos sem depender de texto.
