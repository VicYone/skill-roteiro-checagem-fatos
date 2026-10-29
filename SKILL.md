---
name: roteiro-dark
description: Cria o roteiro de um vídeo do canal dark "Brasil estranho e misterioso" (mistérios e casos reais do Brasil), com pesquisa, ficha de fatos e no mínimo duas revisões de checagem antes de liberar para narração. Use sempre que o Victor pedir roteiro, texto de narração ou vídeo de uma pauta do canal (ex.: "faz o roteiro das máscaras de chumbo", "pauta 3", "próximo vídeo").
---

# Roteiro do canal dark, com revisão obrigatória

O canal conta casos reais. Um erro de fato derruba a credibilidade, pode gerar acusação injusta contra alguém e entrega o canal como "conteúdo gerado em massa". Por isso **nenhum roteiro vai para narração sem passar pelas duas revisões de fatos (etapas 3 e 4)**. Isso foi pedido pelo Victor e não é opcional, nem com pressa.

Pasta do canal: a pasta do projeto do canal (onde ficam `banco-de-pautas.xlsx` e `videos\`). Pautas em `banco-de-pautas.xlsx` (aba "Pautas"). Lista dos erros que você mais comete: [checklist-erros.md](checklist-erros.md). Leia o checklist antes da etapa 3.

## Arquivos de cada vídeo

Crie `videos\NN-slug\` (NN = nº da pauta com dois dígitos) e salve cada etapa no seu arquivo, sem apagar as anteriores:

| Arquivo | Etapa |
|---|---|
| `01-ficha.md` | Ficha de fatos com fontes |
| `02-roteiro-v1.md` | Primeiro rascunho, com marcadores [F#] |
| `03-revisao-1.md` | Revisão 1: checagem de todas as afirmações |
| `04-revisao-2.md` | Revisão 2: funil nos pontos críticos |
| `05-roteiro-final.md` | Texto limpo, pronto para narrar |
| `06-relatorio.md` | Resumo para o Victor |

## 1. Pesquisa e ficha de fatos

- Pesquise na web (WebSearch/WebFetch) e no navegador embutido quando precisar. Prefira fonte primária: jornal da época (Hemeroteca Digital, https://bndigital.bn.gov.br/hemeroteca-digital/), documento oficial (Arquivo Nacional, https://sian.an.gov.br), livro ou artigo acadêmico. A Wikipédia só serve para achar as fontes, não como fonte final.
- A Hemeroteca bloqueia acesso automatizado (erro 403, inclusive no navegador embutido). Não insista: use fontes que citam os jornais com data e ponha a conferência na Hemeroteca no "Confira você". Blogs que listam jornais de época com data (ex.: pmig96.wordpress.com) ajudam a achar a edição certa.
- Afirmação que só aparece num blog é nível B, mesmo que o blog cite jornal de época. Detalhes muito específicos (datas de promoção, falas em entrevistas de TV, respostas de órgãos públicos) tendem a vir de uma fonte só: confira antes de usar. Quando existir livro de quem esteve no caso (ex.: Vallée), procure o trecho literal.
- Monte a ficha como tabela: `F#` | afirmação | fonte (título + link ou referência exata) | nível.
- Níveis: **A** = confirmado em 2+ fontes independentes · **B** = 1 fonte confiável · **C** = versões conflitantes (anote as versões) · **L** = lenda/boato (só entra como "conta-se que").
- Anote à parte: pessoas citadas que podem estar vivas, ou ter família identificável, e o que a Justiça decidiu de fato.
- Se você não achar uma fonte, a afirmação **não entra** na ficha. Nunca invente fonte, livro, link ou edição de jornal.

## 2. Rascunho (v1)

- Só pode usar o que está na ficha. Cada afirmação factual leva o marcador do fato: `...foram encontrados no Morro do Vintém [F3].`
- Estrutura: gancho nos primeiros 30 s (a pergunta central do caso, sem prometer o que o caso não entrega) → contexto → os fatos em ordem → as hipóteses (claramente rotuladas como hipóteses) → o que se sabe hoje → fechamento com a pergunta em aberto.
- Duração-alvo: 10–12 min ≈ 1.400–1.700 palavras.
- Dramatização permitida só na forma (ritmo, pausa, ordem de revelação). Nada de inventar clima, pensamento, diálogo ou detalhe sensorial que não esteja numa fonte.
- Proponha também 3 títulos e 1 ideia de thumbnail, que entram na revisão.

## 3. Revisão 1: todas as afirmações

Releia o rascunho **frase por frase** e extraia toda afirmação verificável, inclusive as que parecem óbvias. Para cada uma, registre em `03-revisao-1.md`:

`frase` | tipo (data, número, nome, lugar, citação, causa, superlativo, conclusão oficial, outro) | F# | a fonte diz exatamente isso? | ação (ok / corrigir / suavizar / cortar)

- Confira contra a fonte **de novo**, abrindo a fonte. Não confie na ficha nem na memória.
- Afirmação sem F#, ou com F# que não sustenta a frase como escrita, é corrigida ou cortada.
- Nível C vira "há versões diferentes..."; nível L vira "conta-se que...", ou sai.
- Passe o checklist-erros.md inteiro e registre o resultado de cada item.
- Gere o `roteiro-v2` dentro do próprio arquivo da revisão, com as correções aplicadas.

## 4. Revisão 2: funil nos pontos críticos

A revisão 2 não repete a 1. Ela **afunila**: pega só o que mais machuca se estiver errado e tenta derrubar.

1. **Selecione os pontos críticos** do roteiro-v2:
   - qualquer frase que atribua culpa, crime, doença ou conduta a uma pessoa identificável;
   - o fato central do vídeo (a "revelação" ou o mistério em si) e tudo o que o título e a thumbnail prometem;
   - números, datas e nomes que aparecem no gancho, no título ou no fechamento;
   - toda citação entre aspas;
   - todo superlativo ("o maior", "o primeiro", "o único", "nunca");
   - o que a polícia, a Justiça ou o governo concluíram;
   - tudo que ficou nível B ou C na revisão 1.
2. **Verificação independente:** delegue a checagem dos pontos críticos a um subagente revisor, que não viu a sua pesquisa. Passe para ele só a lista de afirmações (sem as fontes da ficha) e a instrução: "Tente provar que cada afirmação está errada ou imprecisa. Para cada uma, busque fontes por conta própria e responda: confirmada (com fonte), imprecisa (o que diz a fonte) ou não encontrada". Ele deve achar as próprias fontes.
3. **Compare:** onde o revisor discordar ou não achar fonte, a frase é corrigida, suavizada ou cortada. Na dúvida, corte. Um vídeo um pouco menos dramático é melhor que um vídeo errado.
4. **Checagens de risco** (registre cada uma como ok/ajustado):
   - difamação: pessoa viva ou família identificável só aparece com o que a Justiça decidiu, com "acusado", "segundo a denúncia", "foi absolvido";
   - políticas do YouTube: sem descrição gráfica de violência, sem detalhe de ferimento, sem sexualização, cuidado com menores (evita anúncio limitado);
   - título e thumbnail não prometem nada que o roteiro não entrega;
   - desinformação: hipótese sobrenatural ou conspiratória aparece como hipótese, nunca como conclusão.
5. Se a revisão 2 mudou algo central (o fato principal, uma acusação, o título), rode a revisão 2 de novo só nesses pontos.

## 5. Texto final para narração

Gere `05-roteiro-final.md` só com o texto falado, sem marcadores:
- números, datas e siglas por extenso, do jeito que devem ser lidos ("mil novecentos e sessenta e seis"; sigla na primeira vez por extenso, como "Força Aérea Brasileira");
- frases curtas, uma ideia por frase; quebra de parágrafo onde a voz deve pausar;
- confira a pronúncia de nomes estrangeiros e regionais e, se preciso, escreva-os foneticamente.

## 6. Relatório para o Victor

`06-relatorio.md`, curto:
- quantas afirmações foram checadas, quantas foram corrigidas e quantas cortadas, com as 3–5 mudanças mais importantes;
- **"Confira você"**: os itens que ficaram com uma fonte só ou dependem de documento que você não conseguiu abrir, com o link para o Victor olhar;
- as fontes usadas, prontas para colar na descrição do vídeo;
- títulos e thumbnail finais.

Depois, atualize o status da pauta para "Roteiro" com:
`python status_pauta.py <nº> Roteiro` (rodado na pasta do canal)

Na resposta ao Victor, diga em poucas linhas o que mudou nas revisões e o que ele precisa conferir. Não diga que está "100% checado": diga o que foi checado e o que ficou com fonte única.
