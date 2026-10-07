# Cauldron Crops — Receitas Fechadas do Prototype 0

Versão: 0.1
Status: decisão de design

## 1. Regra

O Prototype 0 terá cinco receitas alquímicas principais.

As receitas 1 e 2 são parte da progressão obrigatória.

As receitas 3, 4 e 5 formam uma cadeia opcional de descoberta que utiliza conteúdo desbloqueado posteriormente.

O objetivo não é maximizar a quantidade de receitas. É provar que o jogador consegue reconhecer propriedades, formar hipóteses, experimentar e obter consequências úteis.

## 2. Receita 1 — Nascimento Solar

**Trigo Dourado + Seiva Bruta → Semente de Tomate Solar**

Ingredientes:
- Trigo Dourado — Vida + Natureza + Luz
- Seiva Bruta — Vida + Natureza

Resultado:
- Semente de Tomate Solar — Vida + Natureza + Luz + Fogo

Lógica:
A seiva fornece a matéria viva necessária para gerar um novo potencial de cultivo. O Trigo Dourado já possui uma afinidade solar, e essa qualidade se manifesta na nova cultura como Tomate Solar.

Consequência:
O jogador desbloqueia uma nova cultura.

Função no P0:
Primeira descoberta significativa e primeiro exemplo da gramática do caldeirão.

## 3. Receita 2 — Restauração

**Trigo Dourado + Tomate Solar → Poção Purificadora Fraca**

Ingredientes:
- Trigo Dourado — Vida + Natureza + Luz
- Tomate Solar — Vida + Natureza + Luz + Fogo

Resultado:
- Poção Purificadora Fraca — efeito de restauração/purificação

Lógica:
Os dois cultivos compartilham uma afinidade forte com Vida, Natureza e Luz. O resultado concentra essas propriedades em uma preparação capaz de restaurar um ambiente corrompido.

Consequência:
A primeira barreira de corrupção pode ser purificada.

Função no P0:
Provar que uma descoberta do caldeirão pode alterar o próprio mundo, e não apenas gerar outro item.

## 4. Receita 3 — Seiva Brilhante

**Seiva Bruta + Escama Brilhante → Seiva Brilhante**

Ingredientes:
- Seiva Bruta — Vida + Natureza
- Escama Brilhante — Água + Luz

Resultado:
- Seiva Brilhante — Vida + Natureza + Luz

Lógica:
A seiva é matéria natural viva. A escama é um material aquático que concentra luz. Ao ser incorporada à seiva, a luminosidade passa a fazer parte da própria matéria.

A Água não precisa permanecer como aspecto do resultado: ela participa como meio/material da transformação, enquanto a característica relevante para a nova seiva é a Luz.

Consequência:
A Seiva Brilhante torna-se um ingrediente para uma descoberta posterior.

Função no P0:
Ensinar que uma combinação pode transformar a propriedade de um material sem simplesmente somar todos os aspectos dos ingredientes.

## 5. Receita 4 — Seiva Lunar

**Seiva Brilhante + Peixe Luminoso → Seiva Lunar**

Ingredientes:
- Seiva Brilhante — Vida + Natureza + Luz
- Peixe Luminoso — Água + Vida + Luz + Sombra

Resultado:
- Seiva Lunar — Vida + Natureza + Luz + Sombra

Lógica:
A Seiva Brilhante já possui a expressão luminosa. O Peixe Luminoso introduz a relação entre Luz e Sombra. A combinação cria uma seiva associada à luminosidade noturna, preservando a conexão com a floresta.

A Água do peixe não precisa aparecer no resultado final porque o processo transforma a essência aquática em uma nova matéria vegetal.

Consequência:
A Seiva Lunar prepara uma descoberta ligada à Lua e ao ciclo noturno.

Função no P0:
Dar motivo para explorar a pesca após a restauração e demonstrar que novas atividades alimentam o caldeirão.

## 6. Receita 5 — Semente Lunar

**Seiva Lunar + Semente de Tomate Solar → Semente de Abóbora Lunar**

Ingredientes:
- Seiva Lunar — Vida + Natureza + Luz + Sombra
- Semente de Tomate Solar — Vida + Natureza + Luz + Fogo

Resultado:
- Semente de Abóbora Lunar — Vida + Natureza + Luz + Sombra

Lógica:
A Semente de Tomate Solar representa uma cultura de expressão solar. A Seiva Lunar introduz a afinidade noturna. A transformação desloca a expressão solar para uma nova cultura lunar.

O resultado não mantém Fogo porque essa propriedade pertence à expressão solar do ingrediente e não é a característica dominante da nova semente.

Consequência:
O jogador obtém uma cultura especial associada à noite.

Função no P0:
Fechar uma pequena cadeia opcional e mostrar que o sistema permite transformar uma descoberta em outra descoberta.

## 7. O que foi retirado da cadeia principal

### Isca Encantada

A ideia:

**Peixe Comum + Seiva Bruta → Isca Encantada**

não entra nas cinco receitas principais do Prototype 0.

O conceito não é ruim, mas cria um ramo lateral específico para pesca e aumenta a quantidade de conteúdo sem ser necessário para provar o núcleo.

Pode voltar futuramente quando a pesca tiver regras suficientes para justificar diferentes tipos de isca.

### Poção de Crescimento

Não entra no P0.

O efeito é facilmente explicado por Vida + Natureza, mas ainda não existe necessidade clara de adicionar uma segunda poção agrícola além da purificação.

### Poção de Revelação

Não entra no P0.

A ideia continua válida para conteúdo futuro, especialmente para memórias e segredos do mundo, mas não precisamos dela para demonstrar o núcleo.

## 8. Adubo

Adubo Natural não é receita do caldeirão.

Ele deve ser uma utilidade agrícola simples, produzida por reaproveitamento de excedentes, sem criar dependência entre agricultura e alquimia.

Uma versão mágica poderá surgir no futuro como descoberta explícita.

## 9. Dependências

### Progressão obrigatória

Trigo Dourado
→ Seiva Bruta
→ Semente de Tomate Solar
→ Tomate Solar
→ Poção Purificadora Fraca
→ primeira purificação
→ pesca

### Cadeia opcional

Escama Brilhante
→ Seiva Brilhante
→ Peixe Luminoso
→ Seiva Lunar
→ Semente de Abóbora Lunar

A cadeia opcional não pode bloquear a conclusão da progressão principal do Prototype 0.

## 10. Estado

Estas cinco receitas estão fechadas como design.

Ainda permanecem abertas:
- quantidades exatas por ingrediente;
- tempo de produção, se houver;
- apresentação visual das descobertas;
- números dos efeitos;
- balanceamento de obtenção dos ingredientes;
- momento exato em que as receitas opcionais são descobertas pelo jogador.

Esses pontos são implementação e balanceamento, não novas decisões de design sobre quais receitas existem.
