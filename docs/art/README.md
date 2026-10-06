# Cauldron Crops — Direção de Arte

Esta pasta contém a fonte de verdade visual do Prototype 0.

## Hierarquia

A ordem de autoridade é:

1. decisões humanas explícitas e mais recentes;
2. `VISUAL_TARGET_0.md`;
3. especificações especializadas desta pasta, como `TERRAIN_LANGUAGE.md` e `GOLEM_LANGUAGE.md`;
4. `ART_BIBLE.md`;
5. referências externas;
6. interpretação de ferramentas ou agentes.

Quando houver conflito, não escolher silenciosamente uma regra. Registrar o conflito e preservar a decisão humana mais recente.

## Papéis

O autor continua sendo o diretor criativo e aprova ou rejeita a direção.

Gemini/Antigravity + PixelLab podem propor e produzir arte de acordo com estas regras.

Codex cuida de integração técnica, testes e documentação. Um asset bonito, um screenshot de QA ou uma implementação funcionando não significam aprovação artística.

## O que está neste repositório

- `VISUAL_TARGET_0.md`: contrato operacional visual do Prototype 0. É o arquivo que deve ser consultado antes de produzir um asset para o protótipo.
- `ART_BIBLE.md`: princípios visuais amplos que devem sobreviver além do Prototype 0.
- `TERRAIN_LANGUAGE.md`: linguagem do terreno e da vegetação.
- `GOLEM_LANGUAGE.md`: linguagem específica dos golems.
- `TERRAIN_BENCHMARK_01.md`: primeiro experimento controlado para validar terreno, escala, densidade e integração.

## Regra de produção

Não produzir assets em massa antes de o benchmark correspondente ser aprovado.

Um benchmark é um experimento, não uma aprovação automática e não deve substituir o jogo real antes de validação.

## Legado

As referências artísticas antigas continuam preservadas no repositório legado `LeandroSatsuki/Cauldron-Crops`.

Elas não são copiadas para esta pasta indiscriminadamente porque isso recriaria múltiplas fontes de verdade. O material que continua válido foi consolidado aqui; o restante permanece como arqueologia.

## Fluxo

Decisão humana → Visual Target → benchmark → avaliação em contexto → aprovação → produção → integração técnica.

Quando uma decisão visual global mudar (câmera, grid, escala, pixel density, paleta estrutural ou linguagem de renderização), atualizar primeiro o documento apropriado antes de produzir uma grande quantidade de assets.
