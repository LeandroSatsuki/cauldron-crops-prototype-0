# Cauldron Crops — Visual Target 0

**Versão:** 0.1  
**Status:** direção de trabalho para Prototype 0; ainda não é a direção artística definitiva do jogo.

## 1. Objetivo

Este documento transforma a direção artística conceitual em um conjunto pequeno de regras operacionais.

A pergunta que ele precisa responder é:

> "Quando os assets aparecem juntos na câmera real do jogo, eles parecem pertencer ao mesmo mundo e continuam legíveis?"

O objetivo não é definir toda a arte futura de Cauldron Crops. O objetivo é impedir tentativa e erro desnecessária durante o Prototype 0.

## 2. Câmera

A referência de câmera do Prototype 0 é próxima de Stardew Valley e Sun Haven.

- perspectiva top-down em 3/4;
- câmera acompanha o gato;
- zoom é permitido;
- a distância da câmera deve preservar leitura do mundo e das interações;
- a câmera não deve exigir microdetalhes para que o cenário pareça rico.

Stardew Valley e Sun Haven são referências de composição e legibilidade, não modelos para copiar identidade, personagens, tiles, objetos ou interface.

## 3. Escala do personagem

O gato deve parecer relativamente pequeno em relação à área visível.

Referência inicial informada pelo autor:

> o gato deve aparecer aproximadamente com 2/3 do tamanho aparente do personagem de Stardew Valley.

Essa é uma relação visual, não uma especificação de sprite em pixels.

A dimensão concreta do sprite será determinada após o teste de câmera e dos assets em contexto.

## 4. Regra de leitura por zoom

A arte deve funcionar em três estados:

### Zoom próximo
Detalhes e materiais podem ser percebidos.

### Zoom normal
Este é o estado principal de gameplay. Silhueta, função, cor e relação entre objetos devem ser imediatamente legíveis.

### Zoom afastado
Os elementos pequenos perdem microdetalhes. Portanto, a leitura deve sobreviver principalmente através de:

- silhueta;
- massa de cor;
- contraste;
- escala relativa;
- posição/composição;
- movimento;
- agrupamento.

Regra:

> Se um asset só funciona quando ampliado, ele ainda não está pronto para o jogo.

## 5. Pixel art e densidade

Cauldron Crops utiliza pixel art 2D.

A resolução oficial por categoria ainda não está congelada.

Não assumir automaticamente 16×16, 32×32, 64×64 ou 128×128.

Primeiro precisamos medir o conjunto real em contexto:

- gato;
- planta;
- ferramenta;
- caldeirão;
- golem;
- árvore;
- terreno;
- ícones.

O que deve permanecer coerente é a densidade aparente do pixel, o nível de detalhe e a escala relativa.

Regra:

> resolução do arquivo não é a mesma coisa que tamanho do objeto no mundo.

## 6. Linguagem de formas

Direção atual:

- formas orgânicas;
- silhuetas claras;
- irregularidade controlada;
- assimetria intencional;
- formas simples o bastante para sobreviver ao zoom afastado;
- detalhes concentrados em áreas de interesse.

Evitar:

- excesso de microdetalhes;
- formas genéricas;
- perfeição geométrica artificial em elementos naturais;
- detalhe adicionado apenas para "parecer mais pixel art".

## 7. Nível de detalhe

O objetivo é **moderate detail / refined contemporary pixel art**.

Detalhes devem ter função:

- comunicar material;
- diferenciar estados;
- reforçar personalidade;
- guiar o olhar;
- criar descoberta.

Detalhes não devem ser usados para esconder uma base fraca.

Áreas de respiro são obrigatórias no cenário.

## 8. Paleta

A direção cromática deve combinar natureza acolhedora com fantasia.

Famílias desejadas:

- verdes e verdes profundos;
- verdes azulados;
- marrons naturais;
- azuis;
- violetas;
- lilases;
- rosas;
- cianos;
- pequenos acentos amarelos/dourados.

A paleta hexadecimal definitiva ainda não está congelada.

Regra:

> saturação é hierarquia, não preenchimento.

Nem tudo deve ser saturado. Nem toda magia deve ser brilhante.

## 9. Contraste e outlines

A leitura precisa existir sem depender de outline preto espesso.

Preferir contraste por:

- valor;
- temperatura;
- cor;
- silhueta;
- sombra.

Outline, quando usado, deve ser subordinado ao material e ao contexto.

Evitar aparência pesada de contorno preto universal.

## 10. Luz e sombra

A iluminação deve transmitir mundo mágico sem parecer uma ilustração digital suave.

Ainda estão abertas:

- direção global da luz;
- intensidade;
- temperatura;
- profundidade das sombras;
- tratamento de efeitos mágicos.

Não usar gradientes e brilho como substitutos de forma e material.

## 11. Natureza

A natureza é o principal veículo da identidade visual.

A floresta deve parecer:

- viva;
- orgânica;
- acolhedora;
- ligeiramente estranha;
- mágica sem ser neon.

A sensação de fantasia pode nascer de:

- espécies;
- combinação de cores;
- pequenas ocorrências incomuns;
- iluminação;
- composição;
- crescimento;
- corrupção e purificação.

## 12. Terreno

A grama e o terreno são assets estruturais.

Eles precisam:

- sustentar grandes áreas;
- repetir sem padrão evidente;
- preservar áreas de respiro;
- permitir leitura de agricultura;
- permitir leitura de personagens e objetos;
- suportar mudanças ambientais.

A linguagem detalhada está em `TERRAIN_LANGUAGE.md`.

## 13. Agricultura

Cultivos devem ser imediatamente reconhecíveis.

Eles devem manter:

- mesma densidade visual do mundo;
- relação clara entre fase e função;
- contraste suficiente;
- silhueta reconhecível;
- integração com o solo.

Não transformar cada cultura em uma mini-ilustração detalhada.

## 14. Caldeirão

O caldeirão possui prioridade visual alta porque é o instrumento central de descoberta.

Direção:

- ancestral;
- ligado à natureza;
- mágico;
- legível;
- forte sem parecer tecnológico.

O efeito mágico deve complementar o objeto, não dominá-lo.

## 15. Golems

A filosofia dos golems está detalhada em `GOLEM_LANGUAGE.md`.

Princípios fundamentais:

- material cria a anatomia;
- silhueta funciona sem depender do rosto;
- magia interna é descoberta, não anunciada;
- estranheza vem antes da fofura;
- não usar esqueleto humano como molde universal.

## 16. Magia

A magia é orgânica ao mundo.

Pode aparecer por:

- crescimento;
- luz localizada;
- cor;
- raízes;
- cristais;
- comportamento ambiental;
- água;
- pequenos efeitos.

Evitar:

- excesso de brilho;
- grandes auras;
- roxo como filtro universal;
- partículas usadas para compensar ausência de direção visual.

## 17. Corrupção e purificação

A corrupção deve parecer alteração do mundo.

Ela pode modificar:

- vegetação;
- solo;
- raízes;
- pedras;
- água;
- iluminação;
- densidade;
- composição.

A purificação deve parecer restauração de vida.

Não tratar nenhum dos dois apenas como troca global de matiz.

## 18. UI e ícones

A UI deve pertencer ao mesmo universo, mas não precisa copiar literalmente o cenário.

Ainda estão abertas:

- composição final dos painéis;
- tipografia;
- ícones;
- bordas;
- decoração;
- paleta final.

Durante o Prototype 0, a prioridade é legibilidade funcional e coerência básica.

## 19. Regras negativas globais

Resultado deve ser revisado quando apresentar:

- aparência genérica de pixel art;
- aparência claramente 8-bit sem intenção;
- aparência de ilustração digital reduzida;
- contorno preto pesado;
- excesso de gradientes;
- excesso de microdetalhes;
- saturação global;
- aparência excessivamente pastel;
- excesso de efeitos mágicos;
- repetição procedural evidente;
- asset bonito isoladamente, mas incompatível com a cena;
- imitação direta de outro jogo;
- escala incompatível com o mundo.

## 20. Critério de aprovação

Um conjunto visual do Prototype 0 precisa responder positivamente:

1. Parece Cauldron Crops?
2. Funciona na câmera real?
3. Continua legível no zoom normal?
4. Continua funcionalmente compreensível quando afastado?
5. Os assets parecem feitos para coexistir?
6. A densidade visual é controlada?
7. A magia parece parte da natureza?
8. A agricultura continua legível?
9. O visual não rouba atenção do gameplay?
10. O conjunto gera curiosidade sem parecer ruidoso?

## 21. Processo

Antes de produzir:

1. definir função do asset;
2. consultar este documento;
3. consultar a especificação especializada relevante;
4. produzir benchmark pequeno;
5. testar em contexto;
6. avaliar;
7. aprovar ou iterar;
8. somente depois produzir em escala.

## 22. O que ainda está deliberadamente aberto

Não congelar ainda:

- resolução por categoria;
- pixel density exata;
- paleta hexadecimal;
- iluminação global;
- regra universal de outline;
- tratamento definitivo da água;
- escala final de árvores;
- UI final;
- quantidade de frames por categoria;
- paleta definitiva de corrupção/purificação.

Essas decisões devem ser descobertas pelos benchmarks.

## 23. Regra central

> **Bonito isoladamente não é suficiente. Precisa funcionar dentro do jogo.**

O objetivo da direção visual do Prototype 0 é construir um conjunto coerente, legível e reproduzível, não uma coleção de assets impressionantes.
