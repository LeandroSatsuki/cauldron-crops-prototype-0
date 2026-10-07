# Cauldron Crops — Prototype 0

## Propósito

O Prototype 0 existe para responder uma única pergunta:

> É divertido jogar Cauldron Crops quando o jogador cultiva, experimenta no caldeirão, descobre coisas, utiliza suas descobertas e percebe que está reconstruindo um mundo mágico?

O objetivo não é criar uma versão pequena do jogo final. O objetivo é provar que o coração do jogo funciona.

## Identidade

Cauldron Crops é um jogo cozy de reconstrução de uma floresta mágica.

O jogador controla um gato que possui uma ligação com uma antiga entidade da natureza. Conforme o mundo é reconstruído, o gato recupera memórias e começa a compreender seu passado, a corrupção e o que aconteceu com a floresta.

O jogador não está simplesmente administrando uma fazenda. Ele está descobrindo, experimentando, reconstruindo, conhecendo o mundo, recuperando memórias e trazendo vida de volta à floresta.

## Pilares

- Descoberta
- Caldeirão como principal instrumento de descoberta
- Mundo vivo
- Liberdade para jogar fazendo o que gosta
- Reconstrução da natureza

## Loop

Conceitual: **Fazer → Encontrar → Experimentar → Descobrir → Usar → Avançar → Fazer novamente**

No Prototype 0: **Plantar → colher → experimentar no caldeirão → descobrir → utilizar a descoberta → progredir**

## Escopo obrigatório

- [ ] Gato jogável
- [ ] Movimentação por clique
- [ ] Pequena área jogável
- [ ] Agricultura
- [ ] Colheita
- [ ] Caldeirão
- [ ] Descobertas
- [ ] Utilidade para as descobertas
- [ ] Pelo menos um golem funcional
- [ ] Pequena progressão
- [ ] Pequena coleção
- [ ] Demonstração da história
- [ ] Demonstração da corrupção
- [ ] Pelo menos um evento contextual
- [ ] Experiência visual coerente
- [ ] Um loop jogável e repetível

## Escopo opcional

Só entra se for pequeno o suficiente para não comprometer o objetivo:

- [ ] Pesca simples
- [ ] Uma quest simples
- [ ] Segundo golem
- [ ] Interação adicional com a corrupção
- [ ] Pequena quantidade de NPCs
- [ ] Pequena demonstração de outro tipo de atividade

Se exigir um sistema grande, sai do Prototype 0.

## Fora do Prototype 0

- Combate completo
- Expedições
- Grandes mapas de exploração
- Sistema completo de mineração
- Cavernas complexas
- Grande quantidade de NPCs
- Sistema completo de quests
- Animais mágicos completos
- Fazenda customizável
- Sistema completo de maestria
- Achievements completos
- Árvore de talentos completa
- Economia complexa
- Equipamentos completos
- Sistema avançado de transmutação
- IA emocional avançada dos golems
- Grande quantidade de receitas
- Grandes regiões
- História completa
- Todas as memórias do gato
- Progressão completa da corrupção
- Multiplayer
- Produção em massa
- Grandes sistemas de automação

Esses sistemas não foram descartados. Pertencem ao futuro.

## Regra contra expansão de escopo

Durante o desenvolvimento, toda nova ideia deve responder:

> Isso é necessário para provar o coração do jogo?

Se não, não entra no Prototype 0. A ideia vai para docs/future.md.

Uma ideia pode ser excelente e ainda assim estar proibida de entrar no Prototype 0.

## Definition of Done

- [ ] O jogador inicia uma sessão sem orientação externa.
- [ ] Planta e colhe.
- [ ] Utiliza o caldeirão.
- [ ] Realiza descobertas.
- [ ] Descobertas possuem consequências práticas.
- [ ] Existe pelo menos um ajudante golem funcional.
- [ ] O mundo apresenta pelo menos um acontecimento inesperado/contextual.
- [ ] O jogador percebe que existe uma história maior.
- [ ] Existe pequena progressão.
- [ ] Existe pequena coleção.
- [ ] O ciclo principal pode ser repetido.
- [ ] A experiência visual possui direção coerente.
- [ ] O jogo produz curiosidade para descobrir o próximo resultado.
- [ ] Não existem sistemas adicionais necessários para demonstrar a fantasia central.

Quando a Definition of Done for atingida, o Prototype 0 termina. Não adicionaremos conteúdo apenas para “deixar mais completo”.

## Critério final

1. **Curiosidade:** “Eu quero descobrir o que acontece se eu experimentar mais coisas?”
2. **Mundo:** “Eu sinto que existe um mundo mágico acontecendo ao meu redor?”
3. **Continuidade:** “Depois de terminar o protótipo, eu quero continuar jogando para descobrir o que existe além?”

Se as três respostas forem positivas, Cauldron Crops terá provado seu núcleo.

## Regra definitiva

**Prototype 0 não é Cauldron Crops completo. É a prova de que Cauldron Crops merece ser construído.**

Tudo que não estiver neste documento fica para depois.

**Depois é depois.**


## Decisões aprovadas — arco inicial

Estas decisões passam a orientar o design e a implementação do Prototype 0. Detalhes não listados como aprovados continuam abertos.

### Convenção de nomes mágicos

Itens naturais e culturas devem preferencialmente seguir a estrutura:

**nome conhecido + adjetivo mágico**

Exemplos de referência inicial:
- Trigo Dourado
- Tomate Solar
- Abóbora Lunar
- Raiz Gélida

Regra: o nome conhecido comunica o que o item é; o adjetivo comunica sua característica mágica, origem ou comportamento.

O adjetivo não deve ser apenas decorativo quando o design permitir que ele carregue significado mecânico ou contextual.

### Primeiro arco de descoberta

O primeiro circuito aprovado é:

**Trigo Dourado → Seiva Bruta → Caldeirão → descoberta de Semente de Tomate Solar → cultivo de Tomate Solar → descoberta de Poção Purificadora Fraca → purificação de uma primeira barreira → nova área → acesso à pesca.**

A forma exata de aquisição inicial de todos os recursos e as receitas posteriores ainda podem ser refinadas dentro deste circuito.

### Primeira receita

A primeira hipótese aprovada para o protótipo é:

**Trigo Dourado + Seiva Bruta → Semente de Tomate Solar**

Objetivo: fazer a primeira descoberta imediatamente útil abrir uma nova possibilidade de cultivo.

A descoberta principal de progressão deve ser determinística. Aleatoriedade não deve bloquear a progressão obrigatória.

### Segunda receita

A segunda hipótese aprovada é:

**Trigo Dourado + Tomate Solar → Poção Purificadora Fraca**

Objetivo: demonstrar que uma descoberta do caldeirão não serve apenas para fabricar; ela altera o mundo e permite progressão.

A receita pode ser ajustada durante o design, mas não deve criar dependência acidental de pesca, expedição ou outro sistema fora do recorte inicial.

### Agricultura fora da corrupção

A regra conceitual aprovada é:

> O jogador pode cultivar em solo apropriado e não corrompido.

O Prototype 0 não deve impor uma única pequena área artificialmente autorizada como a única área cultivável da vila. Áreas corrompidas bloqueiam cultivo até serem restauradas.

O sistema ainda precisa definir os critérios mínimos de “solo apropriado” no mapa novo.

### Primeira barreira e reconstrução

A corrupção está próxima da área inicial. A primeira zona desbloqueável serve também como demonstração de restauração do mundo e libera uma nova atividade, a pesca.

Ao purificar a barreira:
- a área torna-se explorável;
- o jogador pode cultivar onde houver solo apropriado e não corrompido;
- a pesca fica acessível nessa zona;
- o mundo deve comunicar visualmente a mudança.

### Aquisição local de recursos

O Prototype 0 deve evitar depender de expedições ou regiões externas para os ingredientes necessários à progressão principal.

Recursos iniciais podem vir de:
- agricultura;
- missão simples;
- pesca após desbloqueio;
- árvores e elementos naturais próximos da vila, fornecendo materiais como seiva e madeira.

A progressão obrigatória deve ter um caminho determinístico e local.

### Troca natural e fornecedor

Existe uma oportunidade aprovada para uma válvula de excesso de recursos: um fornecedor misterioso ou sistema semelhante de troca natural.

Princípio:
**excedente de recursos naturais → moeda específica de troca → sementes/itens de catálogo variável**

Essa economia não deve bloquear a progressão principal.

O nome e a forma exata da moeda continuam abertos. O fornecedor é tratado como apoio econômico, não como centro do Prototype 0.

### Coleções

O Prototype 0 deve possuir uma coleção pequena, inicialmente organizada em:
- peixes;
- cultivos;
- poções.

A coleção serve para reforçar descoberta e vontade de completar, sem exigir um sistema completo de achievements.

### Ciclo de tempo

A hipótese de tempo aprovada para o Prototype 0 é:

**1 hora do mundo = 1 minuto real.**

Portanto:
- 1 dia = 24 minutos reais;
- 7 dias do mundo = 1 estação;
- 1 estação = aproximadamente 2h48 de tempo real.

Esse relógio deve permitir manhã, tarde, noite e eventos ligados ao horário sem exigir espera de horas reais.

A duração exata poderá ser ajustada por balanceamento de playtest sem mudar o princípio do ciclo acelerado.

### Pesca

A pesca simples passa a ser uma atividade de apoio do Prototype 0 porque a primeira área restaurada a libera e ela participa da identidade de coleção/descoberta.

Escopo mínimo:
- acesso somente após restauração da primeira zona;
- poucos peixes;
- poucos estados/regras;
- integração com coleção e, quando necessário, com o caldeirão.

Não transportar o minigame e a infraestrutura externa do legado por inteiro.

### Alquimia orientada por propriedades

O caldeirão será orientado por duas camadas de metadados nos itens:

- **tags funcionais**, que descrevem o que o item é ou como é usado;
- **aspectos**, que descrevem propriedades conceituais/mágicas reutilizáveis nas descobertas.

As receitas do Prototype 0 devem ser autoradas, determinísticas e justificáveis pelas propriedades dos ingredientes. O objetivo é que o jogador aprenda relações entre ingredientes em vez de decorar combinações arbitrárias.

A especificação do sistema está em `docs/alchemy/ALCHEMY_TAGS.md`.

O Prototype 0 não implementará um gerador automático de receitas por aspectos. O sistema de aspectos é uma fundação extensível para o presente e para conteúdo futuro.

## O que ainda está deliberadamente aberto

Ainda precisamos definir:
- receitas 3, 4 e 5;
- conjunto final de 3–5 peixes;
- conjunto final de 3–5 cultivos;
- conjunto final de poções;
- evento contextual;
- conteúdo exato da primeira missão;
- texto da primeira memória do gato;
- nome e regras da moeda natural;
- catálogo inicial do fornecedor;
- critérios exatos de solo cultivável;
- duração final do ciclo após playtest.

Esses pontos são decisões de design pendentes, não lacunas técnicas a serem preenchidas automaticamente pelo Codex.
