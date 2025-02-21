# Plano de Mudança - Fluxo de Git

## Objetivo
Este documento descreve o plano de mudança para gerenciamento de código no repositório, seguindo o fluxo de trabalho baseado nas branches `master` e `teste`. Todas as **issues** do Git geram novas branches, que devem ser integradas na branch `teste` antes de serem mescladas na `master`.

## Fluxo de Trabalho

### 1. **Criação de Branch**
- **Branch Principal**: `master` (produtiva, versão estável do código).
- **Branch de Teste**: `teste` (utilizada para desenvolvimento e integração das features).
- **Branches de Issue**: Para cada issue criada no Git, uma nova branch será gerada a partir de `teste`. A nomenclatura das branches será baseada no ID da issue:
  - `issue-<ID-da-issue>` (por exemplo, `issue-123` ou `issue-456`).

#### Exemplo de criação de branch:
```bash
git checkout teste
git checkout -b issue-123
