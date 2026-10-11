# Cauldron Crops — Direção de Arte

Esta pasta contém a fonte de verdade visual do Prototype 0 e os perfis operacionais utilizados pelo aplicativo de geração de assets.

## Hierarquia

A ordem de autoridade é:

1. decisões humanas explícitas e mais recentes;
2. `VISUAL_TARGET_0.md`;
3. especificações especializadas desta pasta;
4. `ASSET_GENERATION_CORE.md` e os perfis em `asset-profiles/` para a operação do gerador;
5. `ART_BIBLE.md`;
6. referências externas;
7. interpretação de ferramentas ou agentes.

Quando houver conflito, não escolher silenciosamente uma regra. Registrar o conflito e preservar a decisão humana mais recente. Os perfis do gerador operacionalizam a direção visual; eles não tornam automaticamente definitiva uma decisão que o Visual Target mantém aberta.

## Papéis

O autor continua sendo o diretor criativo e aprova ou rejeita a direção.

Gemini/Antigravity + PixelLab podem propor e produzir arte de acordo com estas regras.

Codex cuida de integração técnica, testes e documentação. Um asset bonito, um screenshot de QA ou uma implementação funcionando não significam aprovação artística.

## Documentos de direção

- `VISUAL_TARGET_0.md`: contrato operacional visual do Prototype 0.
- `ART_BIBLE.md`: princípios visuais amplos que devem sobreviver além do Prototype 0.
- `TERRAIN_LANGUAGE.md`: linguagem do terreno e da vegetação.
- `GOLEM_LANGUAGE.md`: linguagem específica dos golems.
- `TERRAIN_BENCHMARK_01.md`: experimento para validar terreno, escala, densidade e integração.
- `LEGACY_ART_CONSOLIDATION.md`: histórico da consolidação do material antigo.

## Perfis para o aplicativo de geração de assets

Esses arquivos existem para reduzir tokens e tornar as gerações previsíveis. Eles são instruções operacionais direcionadas por categoria e podem ser carregados sem carregar toda a documentação de arte.

**Contexto recomendado por geração:**

1. Carregar sempre `ASSET_GENERATION_CORE.md`.
2. Identificar a categoria solicitada.
3. Carregar somente um perfil correspondente em `asset-profiles/`.
4. Acrescentar o pedido do usuário e, quando houver, a referência visual aprovada.
5. Não carregar os outros perfis, salvo quando o asset realmente combinar categorias.

### Contexto global

- `ASSET_GENERATION_CORE.md`: estilo global, câmera, formato padrão, paleta operacional Mystical Forest 32, prioridade de cores, iluminação, regras negativas e checklist.

### Perfis por categoria

- `asset-profiles/TERRAIN.md`: tiles, terreno, solo cultivável e caminhos.
- `asset-profiles/VEGETATION.md`: árvores, copas, arbustos, grama, raízes e musgo.
- `asset-profiles/FLORA_AND_CROPS.md`: flores, cultivos, plantas mágicas e cogumelos.
- `asset-profiles/ROCKS_AND_MINERALS.md`: pedras, rochas, minerais e cristais.
- `asset-profiles/PROPS_AND_STRUCTURES.md`: caldeirão, objetos, ruínas e estruturas.
- `asset-profiles/CHARACTERS.md`: gato, NPCs e criaturas que não usem regras específicas de golems.
- `asset-profiles/GOLEMS.md`: anatomia orientada pelo material e identidade visual de golems.
- `asset-profiles/MAGIC_EFFECTS.md`: luz mágica, feitiços, partículas e efeitos.
- `asset-profiles/RESOURCE_ICONS.md`: ícones de inventário, ingredientes e recursos.

A paleta Mystical Forest 32 é a paleta operacional padrão do gerador para experimentação. Ela continua sujeita à validação em contexto antes de ser promovida a paleta definitiva global do jogo.

## Regra de produção

Não produzir assets em massa antes de o benchmark correspondente ser aprovado.

Um benchmark é um experimento, não uma aprovação automática e não deve substituir o jogo real antes de validação.

## Legado

As referências artísticas antigas continuam preservadas no repositório legado `LeandroSatsuki/Cauldron-Crops`.

Elas não são copiadas para esta pasta indiscriminadamente porque isso recriaria múltiplas fontes de verdade. O material que continua válido foi consolidado aqui; o restante permanece como arqueologia.

## Fluxo

Decisão humana → Visual Target → benchmark → avaliação em contexto → aprovação → produção → integração técnica.

Quando uma decisão visual global mudar (câmera, grid, escala, pixel density, paleta estrutural ou linguagem de renderização), atualizar primeiro o documento apropriado antes de produzir uma grande quantidade de assets.
