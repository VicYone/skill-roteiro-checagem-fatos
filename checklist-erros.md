# Checklist: onde o Claude mais erra em roteiro de caso real

Passe item por item na revisão 1 e registre "ok" ou o que foi ajustado. Os itens estão em ordem de frequência: os primeiros são os erros mais comuns.

## 1. Precisão inventada
Data exata, hora, idade, número de vítimas, valores, distâncias. O modelo tende a "completar" com um número plausível quando a fonte só diz "cerca de" ou nem diz.
→ Todo número precisa estar literalmente na fonte. Se a fonte diz "cerca de", o roteiro diz "cerca de".

## 2. Nomes de personagens secundários
Delegado, perito, testemunha, jornalista, o nome do navio ou do jornal. São os nomes mais fáceis de inventar ou trocar.
→ Confira a grafia e o papel de cada nome próprio. Na dúvida, use o cargo sem o nome ("o delegado do caso").

## 3. Citações
Frases entre aspas atribuídas a alguém, inclusive o texto de bilhetes, cartas e manchetes.
→ Só vai entre aspas o que está transcrito numa fonte, palavra por palavra. Sem isso, vira paráfrase sem aspas ("ele disse que...").

## 4. Lenda tratada como fato
Em casos de mistério, a versão popular costuma ser mais famosa que a documentada (ex.: detalhes que só aparecem em sites e vídeos, nunca em jornal da época).
→ Para cada detalhe marcante, pergunte: isso está numa fonte da época ou num documento oficial? Se só aparece em conteúdo recente, é nível L.

## 5. Fusão de versões
Misturar detalhes de duas versões incompatíveis do mesmo caso, ou de dois casos parecidos.
→ Se as fontes divergem, o roteiro apresenta as versões separadas, dizendo quem conta cada uma.

## 6. Superlativos e "primeiros"
"O maior", "o primeiro do mundo", "o único", "nunca mais", "até hoje ninguém".
→ Só ficam com fonte que diga isso. Senão: "um dos maiores", "pouco tempo depois", "não há registro de...".

## 7. Conclusão oficial distorcida
Dizer que alguém "matou", "confessou" ou "foi condenado" quando foi só acusado, foi absolvido, ou o inquérito foi arquivado.
→ Confira exatamente o desfecho jurídico e use os termos certos: suspeito, acusado, denunciado, condenado, absolvido, arquivado.

## 8. Cronologia e causa
Trocar a ordem dos fatos ou criar uma relação de causa ("por isso", "o que levou a...") que a fonte não estabelece.
→ Monte a linha do tempo pela ficha e confira cada "então", "depois" e "por isso".

## 9. Dramatização inventada
Clima ("noite chuvosa"), pensamentos, falas, sons e cheiros que tornam a cena mais viva, mas não estão em fonte nenhuma.
→ Corte. Se quiser atmosfera, descreva o lugar como ele é ou era, com fonte.

## 10. Fonte inexistente ou mal citada
Livro com título ou autor errado, edição de jornal que não existe, link que não abre.
→ Abra cada link e confira título, autor e data de cada referência listada na descrição.

## 11. Anacronismo
Nome atual de cidade, bairro, órgão ou moeda usado para a época do caso (ex.: chamar de "real" um valor de 1960).
→ Use o nome da época, e o atual entre parênteses se ajudar.

## 12. Pessoas vivas e famílias
Afirmação negativa sobre alguém que pode estar vivo, ou que expõe a família.
→ Só o que está documentado e é necessário para a história. Sem especulação sobre culpa.

## 13. Resumo da ferramenta tomado como fonte
O WebFetch devolve um resumo feito por outro modelo, que pode pôr interpretação nos títulos e tópicos. No piloto das máscaras de chumbo, o tópico "hipótese extraterrestre (defendida pela revista O Cruzeiro)" virou fato no roteiro, mas o artigo dizia que a revista **ironizou** a hipótese.
→ Para posição, opinião ou tom ("defendeu", "negou", "ironizou") e para qualquer frase que vá entre aspas, peça ao WebFetch a **frase literal** do texto antes de usar.
