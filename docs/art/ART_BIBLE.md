# Cauldron Crops — Art Bible

Versão: 0.1
Status: princípios visuais amplos do projeto; complementado pelas especificações do Prototype 0.

## 1. Propósito

Este documento reúne os princípios visuais que devem permanecer coerentes no universo de Cauldron Crops.

Ele não substitui o contrato operacional de VISUAL_TARGET_0.md.

A hierarquia visual é:

1. decisões humanas explícitas e mais recentes;
2. VISUAL_TARGET_0.md;
3. especificações especializadas, como TERRAIN_LANGUAGE.md e GOLEM_LANGUAGE.md;
4. este documento;
5. referências externas;
6. interpretação de ferramentas ou agentes.

## 2. Identidade

Cauldron Crops deve transmitir:

- cozy fantasy;
- natureza mágica;
- descoberta;
- reconstrução;
- mistério;
- mundo vivo;
- sensação de aconchego com uma camada sutil de estranheza.

A arte deve parecer parte de um mundo que possui história e vida própria.

## 3. Linguagem visual

Direção geral:

- pixel art 2D contemporânea e refinada;
- formas orgânicas;
- silhuetas claras;
- assimetria controlada;
- detalhe moderado;
- materiais reconhecíveis;
- iluminação coerente;
- riqueza visual controlada.

A inspiração em Stardew Valley e Sun Haven é de linguagem geral, composição, escala e legibilidade. Não copiar identidade visual, personagens, tiles, objetos ou layouts.

## 4. Escala e câmera

A câmera é top-down/3/4 e acompanha o gato.

O jogo possui zoom.

Todos os assets precisam ser avaliados dentro da câmera real.

O gato é relativamente pequeno em relação à área visível, aproximadamente 2/3 do tamanho aparente do protagonista de Stardew Valley como referência visual.

A dimensão concreta de sprites e a pixel density oficial devem ser determinadas por benchmark, não por convenção arbitrária.

## 5. Leitura

Um asset precisa funcionar em:

- zoom próximo;
- zoom normal;
- zoom afastado.

No zoom normal, silhueta, função, massa de cor e contraste devem ser claros.

No zoom afastado, a leitura não pode depender de microdetalhes.

> Um asset que só funciona ampliado ainda não está pronto para o jogo.

## 6. Pixel Art

Não assumir automaticamente 16x16, 32x32, 64x64 ou 128x128.

O que deve permanecer consistente é a densidade aparente do pixel, a escala relativa e o tratamento visual.

Evitar:

- pixelização artificial de uma ilustração digital;
- aparência 8-bit sem intenção;
- pixels excessivamente finos para a escala do jogo;
- microdetalhes que desaparecem na câmera.

## 7. Formas e silhuetas

Priorizar:

- formas orgânicas;
- massas legíveis;
- irregularidade controlada;
- assimetria intencional;
- detalhes concentrados em pontos de interesse.

Evitar:

- perfeição geométrica artificial em natureza;
- formas genéricas;
- excesso de detalhes para compensar uma silhueta fraca.

## 8. Paleta

A direção cromática combina natureza acolhedora e fantasia.

Famílias recorrentes:

- verdes e verdes profundos;
- verdes azulados;
- marrons naturais;
- azuis;
- violetas;
- lilases;
- rosas;
- cianos;
- pequenos acentos dourados e amarelos.

A paleta hexadecimal definitiva não está congelada.

> Saturação é hierarquia, não preenchimento.

Nem todo objeto precisa ser saturado. Nem toda magia precisa ser luminosa.

## 9. Luz, sombra e contorno

Preferir contraste por:

- valor;
- temperatura;
- cor;
- silhueta;
- sombra.

Não depender de outline preto espesso.

Outlines, quando usados, devem ser subordinados ao material e ao contexto.

Evitar:

- preto universal;
- gradientes suaves usados como substituto de forma;
- highlights excessivos;
- bloom/glow dominante.

## 10. Natureza

A natureza é o principal veículo da identidade.

A floresta deve parecer:

- viva;
- orgânica;
- acolhedora;
- ligeiramente estranha;
- mágica sem ser neon.

A fantasia pode nascer de espécies, combinações de cores, crescimento, comportamento, iluminação localizada e transformações do ambiente.

## 11. Magia

A magia é parte natural do mundo.

Pode aparecer por:

- crescimento incomum;
- luz localizada;
- mudanças de cor;
- raízes;
- cristais;
- água;
- pequenos efeitos;
- comportamento ambiental.

Regra:

> Magia modifica ou revela a natureza; não deve apenas ser sobreposta como efeito.

Evitar:

- grandes auras;
- excesso de partículas;
- glow em todos os objetos;
- roxo como filtro universal.

## 12. Materiais

Cada material deve ter uma linguagem própria, perceptível por:

- silhueta;
- textura;
- cor;
- peso visual;
- highlights;
- irregularidade.

Madeira não deve parecer pedra com textura marrom. Pedra não deve parecer metal. Plantas não devem parecer decoração genérica.

## 13. Terreno e ambiente

O terreno é estrutura visual.

Deve:

- sustentar grandes áreas;
- repetir sem padrão evidente;
- preservar áreas de respiro;
- permitir leitura de agricultura;
- permitir leitura de personagens e criaturas;
- aceitar estados ambientais.

A linguagem específica está em TERRAIN_LANGUAGE.md.

## 14. Agricultura

Cultivos precisam ser imediatamente reconhecíveis.

Devem manter:

- mesma densidade visual do mundo;
- contraste suficiente;
- relação clara com o solo;
- silhueta reconhecível;
- leitura de fase de crescimento.

Não transformar cada cultura em uma pequena ilustração detalhista.

## 15. Objetos importantes

Objetos centrais de gameplay devem possuir prioridade visual adequada.

O caldeirão é especialmente importante porque é o instrumento central de descoberta.

Ele deve parecer:

- ancestral;
- natural;
- mágico;
- legível;
- forte;
- não tecnológico.

## 16. Criaturas e personagens

Personagens devem possuir:

- silhueta clara;
- proporção consistente com a câmera;
- identidade forte;
- leitura em pequena escala.

O Visual Master do gato é a principal referência de personagem do Prototype 0.

Novos personagens e criaturas devem parecer pertencentes ao mesmo mundo.

## 17. Golems

Golems devem derivar seu corpo da matéria que os forma.

Princípios:

- magia + matéria → criatura;
- material cria anatomia;
- silhueta deve funcionar sem depender do rosto;
- magia interna deve ser sutil;
- estranheza vem antes da fofura;
- não usar humanoide como molde universal.

Consultar GOLEM_LANGUAGE.md para regras específicas.

## 18. Corrupção e purificação

Corrupção e purificação são transformações do mundo.

Podem afetar:

- solo;
- vegetação;
- raízes;
- pedras;
- água;
- iluminação;
- densidade;
- composição.

Não tratar corrupção como simples filtro roxo/preto.

Purificação deve parecer restauração de vida e continuar visualmente ligada ao mesmo lugar corrompido.

## 19. UI

A interface pertence ao mesmo universo, mas sua prioridade é legibilidade.

Durante o Prototype 0:

- funcionalidade vem primeiro;
- decoração é secundária;
- não copiar interfaces de jogos de referência;
- manter linguagem cromática e de materiais compatível com o mundo.

## 20. Conceito versus asset

Concept art e asset de produção são coisas diferentes.

Uma imagem pode ser excelente para explorar uma ideia e inadequada para entrar diretamente no jogo.

Antes de considerar algo pronto, validar:

- escala;
- pixel density;
- transparência;
- silhueta;
- footprint;
- estados;
- animação;
- legibilidade;
- integração com a câmera;
- integração com os outros assets.

## 21. Produção

Não produzir assets em massa antes de validar um benchmark.

Fluxo:

decisão humana → Visual Target → benchmark → avaliação em contexto → aprovação → produção → integração

Uma imagem bonita isoladamente não é aprovação.

## 22. Regras negativas globais

Revisar ou rejeitar assets que apresentem:

- estética genérica de IA;
- aparência de ilustração digital apenas pixelizada;
- 8-bit não intencional;
- outlines pretos pesados;
- excesso de gradientes;
- microdetalhamento;
- saturação global;
- pastel excessivo;
- glow excessivo;
- escala incompatível;
- repetição procedural evidente;
- perspectiva incorreta;
- aparência 3D renderizada;
- cópia evidente de outro jogo;
- incompatibilidade com o Visual Master.

## 23. Critério de aprovação

Um asset ou conjunto visual deve responder positivamente:

1. Parece Cauldron Crops?
2. Pertence ao mesmo mundo que o gato?
3. Funciona na câmera real?
4. Continua legível no zoom normal?
5. Sua função é clara?
6. Sua escala faz sentido?
7. A densidade visual é compatível?
8. A magia parece orgânica?
9. Não rouba atenção desnecessariamente do gameplay?
10. É reproduzível para outros assets da mesma categoria?

## 24. Regra central

> Bonito isoladamente não é suficiente. Precisa funcionar dentro do jogo.
