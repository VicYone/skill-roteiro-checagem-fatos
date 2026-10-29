# Agente de roteiro com checagem de fatos

Skill para o **Claude Code** que escreve roteiros de vídeo sobre casos reais e só libera o texto para narração depois de **duas revisões de fatos**. A segunda revisão é feita por um **subagente revisor independente**, que não vê a pesquisa original e tem a missão de provar que cada afirmação está errada.

## O problema

Modelos de linguagem escrevem bem e erram com confiança: completam datas, inventam nomes de personagens secundários, põem entre aspas frases que ninguém disse e tratam lenda como fato. Num canal sobre casos reais, um erro desses derruba a credibilidade e pode acusar alguém injustamente.

## Como funciona

```
pesquisa → ficha de fatos (F1, F2…, com fonte e nível de confiança)
        → rascunho v1 (cada afirmação marcada com o fato que a sustenta)
        → revisão 1: todas as afirmações, frase por frase, contra a fonte reaberta
        → revisão 2: só os pontos críticos, checados por um subagente que busca as próprias fontes
        → texto final para narração + relatório do que conferir à mão
```

- **Níveis de confiança na ficha:** A (2+ fontes independentes), B (1 fonte confiável), C (versões conflitantes), L (lenda: só entra como "conta-se que").
- **Revisão 2 em funil:** acusações a pessoas identificáveis, o fato central, tudo que o título promete, citações, superlativos e o que a Justiça decidiu.
- **Checklist de erros** ([`checklist-erros.md`](checklist-erros.md)): os 13 erros mais comuns do modelo, montado a partir dos erros reais encontrados nos pilotos.
- **Relatório final honesto:** nunca diz "100% checado"; lista o que ficou com fonte única para o humano conferir.

## Resultado no primeiro roteiro

O exemplo completo está em [`exemplo-mascaras-de-chumbo/`](exemplo-mascaras-de-chumbo/) (caso das Máscaras de Chumbo, Niterói, 1966).

| Etapa | Afirmações checadas | Corrigidas | Cortadas |
|---|---|---|---|
| Revisão 1 | 48 | 13 | 1 |
| Revisão 2 (revisor independente) | 23 | 11 | 1 |

O erro mais grave, dizer que a revista O Cruzeiro *defendeu* a tese extraterrestre quando na verdade *ironizou*, passou pela revisão 1 e **só foi pego pelo revisor independente**. Ele veio de um resumo automático de página tomado como fonte, e virou o item 13 do checklist.

## Arquivos

| Arquivo | O que é |
|---|---|
| `SKILL.md` | As instruções que o Claude Code segue (etapas, formatos, regras) |
| `checklist-erros.md` | Lista dos erros mais frequentes, conferida item a item na revisão 1 |
| `exemplo-mascaras-de-chumbo/` | Ficha, rascunho, as duas revisões, texto final e relatório de um roteiro real |

## Como usar

1. Copie esta pasta para `~/.claude/skills/roteiro-dark/`.
2. No Claude Code, peça: *"faz o roteiro da pauta 3"*. A skill é acionada pela descrição no topo do `SKILL.md`.

Feito com Claude Code, usando subagentes para a verificação independente.
