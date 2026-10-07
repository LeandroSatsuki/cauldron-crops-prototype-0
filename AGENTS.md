# AGENTS.md — Cauldron Crops Prototype 0

## Projeto

Este repositório contém exclusivamente o **Cauldron Crops — Prototype 0**.

A fonte de verdade de design está na documentação deste repositório, principalmente:

- `PROTOTYPE_0.md`
- `docs/vision.md`
- `docs/alchemy/ALCHEMY_TAGS.md`
- `docs/alchemy/ITEM_CATALOG_0.md`
- `docs/alchemy/ASPECT_MATRIX_0.md`
- `docs/alchemy/RECIPE_SET_0.md`
- `docs/art/VISUAL_TARGET_0.md`

O repositório legado `LeandroSatsuki/Cauldron-Crops` é apenas referência e arqueologia técnica.

## Regra de escopo

Prototype 0 existe para provar o núcleo:

**Plantar → colher → experimentar → descobrir → usar → progredir**

Não adicionar sistemas apenas porque seriam úteis para o jogo final.

Quando uma solução exigir um sistema grande, procurar primeiro uma implementação menor.

Uma ideia pode ser boa e ainda assim ficar fora do Prototype 0.

## Regra contra migração do legado

Não copiar a arquitetura do legado.

Não portar automaticamente:

- `Main.gd`
- `UI.gd`
- `SaveManager.gd`
- seus autoloads;
- sistemas globais;
- infraestrutura de interface;
- árvores de dependências;
- grandes blocos de código.

Consultar o legado somente para extrair comportamentos ou soluções isoladas que sejam realmente úteis.

A pergunta é:

> O que vale preservar como comportamento?

e não:

> Como copiar o sistema antigo?

## Arquitetura

Preferir:

- componentes pequenos;
- responsabilidades claras;
- dados separados da lógica;
- poucas dependências globais;
- uma autoridade clara para cada estado;
- composição simples.

Evitar:

- god objects;
- managers globais desnecessários;
- lógica de gameplay dentro da UI;
- duplicação de estado;
- abstrações criadas antes de existir necessidade real.

Não criar autoload somente por conveniência.

## Design de itens e alquimia

Os itens distinguem:

**tags funcionais**

de

**aspectos alquímicos**.

Os oito aspectos fundamentais são:

- Vida
- Natureza
- Água
- Terra
- Fogo
- Ar
- Luz
- Sombra

Não criar novos aspectos.

`spirit`, `corruption`, `growth`, `magic`, `purification`, `attraction` e conceitos semelhantes não devem ser convertidos automaticamente em novos aspectos.

As cinco receitas fechadas do Prototype 0 estão em:

`docs/alchemy/RECIPE_SET_0.md`

Não alterar essas receitas por conta própria.

## Arte

Seguir:

`docs/art/VISUAL_TARGET_0.md`

A coerência deve ser avaliada no jogo, respeitando:

- câmera 3/4;
- câmera seguindo o gato;
- zoom;
- escala do personagem;
- legibilidade à distância;
- linguagem de pixel art;
- coerência de terreno, objetos e personagens.

Arte gerada isoladamente não é considerada aprovada apenas porque parece boa.

## Processo de implementação

Para tarefas de código:

1. Ler somente a documentação relevante antes de modificar o sistema.
2. Entender a implementação existente.
3. Fazer a menor mudança que resolve a tarefa.
4. Executar testes relevantes.
5. Executar o jogo ou a cena afetada quando possível.
6. Corrigir problemas encontrados.
7. Revisar o diff antes de concluir.

Não modificar documentação de design apenas para fazer uma implementação parecer válida.

Quando uma decisão de design estiver ausente, registrar a lacuna e usar a solução mínima reversível em vez de inventar um sistema grande.

## Testes e validação

Depois de modificar comportamento:

- execute os testes existentes;
- execute verificações específicas da feature;
- abra o projeto/cena afetada quando possível;
- valide o fluxo do jogador, não apenas a ausência de erros.

Não declarar uma feature pronta somente porque o código compila.

## Git

Fazer commits pequenos e temáticos.

Preferir mensagens que expliquem a mudança:

- `feat: ...`
- `fix: ...`
- `test: ...`
- `docs: ...`
- `refactor: ...`

Não misturar uma grande refatoração com uma feature sem necessidade.

## Regra final

Quando houver conflito entre velocidade e integridade do Prototype 0, preservar a integridade do protótipo.

O objetivo não é produzir muito código.

O objetivo é produzir evidência de que o jogo funciona.
