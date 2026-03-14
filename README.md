# Template ABNT — abntex2

Template LaTeX para trabalhos acadêmicos conforme ABNT NBR 14724:2011, construído sobre a classe `abntex2`.

## Requisitos

- TeX Live 2020 ou superior (ou MiKTeX equivalente)
- Pacotes: `newtxtext`, `newtxmath`, `abntex2cite`, `fancyhdr`, `hyperref`

## Estrutura

```
.
├── main.tex          # Arquivo principal
├── referencias.bib   # Referências bibliográficas
└── README.md
```

## Uso

1. Clone o repositório ou baixe os arquivos.
2. Preencha os metadados no preâmbulo de `main.tex`:

```latex
\titulo{Título do Trabalho}
\autor{Nome do Autor}
\instituicao{Nome da Instituição}
\local{Cidade}
\data{2025}
```

3. Adicione suas referências em `referencias.bib` em UTF-8.
4. Faça upload dos arquivos `main.tex` e `referencias.bib` para um projeto no [Overleaf](https://www.overleaf.com).
5. O Overleaf compila automaticamente. Caso o sumário ou as referências não apareçam na primeira vez, clique em **Recompile**.

## Formatação aplicada

| Elemento | Configuração |
|---|---|
| Fonte | Times New Roman (newtxtext) |
| Tamanho | 12pt |
| Margens | Superior 3cm, inferior 2cm, esquerda 3cm, direita 2cm |
| Recuo de parágrafo | 1,25cm |
| Espaçamento | 1,5 entre linhas |
| Numeração | Canto superior direito, a partir da introdução |

## Referências bibliográficas

O arquivo `referencias.bib` deve ser salvo em **UTF-8 sem BOM**. Caracteres acentuados devem ser escritos diretamente em UTF-8 — nunca como sequências de escape latin-1.

```bibtex
% Correto
title = {Informação e documentação},

% Incorreto
title = {Informa{\c{c}}{\~a}o e documenta{\c{c}}{\~a}o},
```

## Normas atendidas

- ABNT NBR 14724:2011 — Trabalhos acadêmicos
- ABNT NBR 10520:2023 — Citações
- ABNT NBR 6028:2021 — Resumo
