# Regra de Versionamento de Prompts

## Comportamento obrigatório ao modificar prompts

Sempre que o usuário pedir qualquer alteração, melhoria ou modificação em um prompt:

1. **Identifique a versão mais recente** — Navegue até a pasta do agente (ex: `clinica_sorriso_real/SDR/`) e identifique qual é o arquivo de versão mais alta (ex: `v3`, `v4`, etc.).

2. **Leia a versão mais recente** — Abra e leia o conteúdo completo da última versão para entender o estado atual do prompt.

3. **NUNCA modifique a versão existente** — Os arquivos de versão anteriores são imutáveis. Não edite, não sobrescreva, não altere nenhum arquivo de versão já existente.

4. **Crie uma nova versão** — Aplique as mudanças solicitadas pelo usuário criando um novo arquivo com o número de versão incrementado (ex: se a última é `v3`, crie `v4`). O novo arquivo deve conter o prompt completo com todas as alterações aplicadas.

5. **Atualize o título** — No cabeçalho do novo prompt, atualize a referência de versão (ex: `(v3)` → `(v4)`).

## Exemplo

Se o usuário pedir "adiciona uma regra de horário no prompt da SDR":
- Vá em `clinica_sorriso_real/SDR/`
- Identifique que a última versão é `v3`
- Leia o conteúdo de `v3`
- Crie `v4` com todo o conteúdo de `v3` + a nova regra de horário
- Nunca toque no arquivo `v3`

## Formato de nomes de arquivo

- Arquivos de versão seguem o padrão: `v1`, `v2`, `v3`, `v4`, etc. (sem extensão)
- Ficam dentro da pasta do agente correspondente (ex: `SDR/`, `closer/`, etc.)
