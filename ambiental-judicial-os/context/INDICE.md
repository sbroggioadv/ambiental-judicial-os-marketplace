# Índice — CAM · ambiental judicial

Captura literal em 01/10/2026, exclusivamente de fontes oficiais: sete snapshots de páginas do Planalto e um PDF do CNMP na lane CAM, mais um novo snapshot da página do CPC no Planalto na lane CAM2, todos com HTTP 200. Nenhum agregador foi usado. Os anexos registram fonte, URL, data, decodificação, SHA-256 e método; `manifesto-captura.json` contém os artigos recortados e hashes dos corpos finais. O snapshot CPC da CAM2 tem hash próprio e não altera o anexo CPC anterior.

## Anexos

| Anexo | Escopo | Caracteres do corpo |
| --- | --- | ---: |
| [cf-ambiental.md](cf-ambiental.md) | CF art. 5º XXXV/LIV/LV; 129 III e § 1º; 170 VI; 225 integral (caputs de 129/170 incluídos) | 5079 |
| [lei-7347-acp-integral.md](lei-7347-acp-integral.md) | Arts. 1º–23, diploma compilado integral | 11656 |
| [lei-6938-pnma.md](lei-6938-pnma.md) | Arts. 1º–4º, 9º, 14 e 15 integrais | 10838 |
| [lei-12651-codigo-florestal.md](lei-12651-codigo-florestal.md) | Arts. 1º-A–9º, 12–18, 29, 59–68; inclui 61-A–61-C | 91960 |
| [lei-9605-responsabilidade.md](lei-9605-responsabilidade.md) | Somente arts. 3º, 4º e 20 | 1001 |
| [cdc-tutela-coletiva.md](cdc-tutela-coletiva.md) | Arts. 81–104; exclui 104-A–104-C | 10517 |
| [cpc-tutela-prova-execucao.md](cpc-tutela-prova-execucao.md) | Arts. 18, 139, 300–311, 369, 373, 464–480, 497–501, 536–537; 784 caput e IV/XII | 25228 |
| [resolucao-cnmp-179-tac-integral.md](resolucao-cnmp-179-tac-integral.md) | Arts. 1º–15 e preâmbulo; consolidada oficialmente com Resolução 326/2026 | 13832 |
| [cpc-litisconsorcio.md](cpc-litisconsorcio.md) | Arts. 113–118 integrais | 1975 |
| [cpc-intervencao-terceiros.md](cpc-intervencao-terceiros.md) | Arts. 119–138 integrais: assistência, denunciação, chamamento, desconsideração e amicus curiae | 7481 |
| [cpc-ilegitimidade-passiva.md](cpc-ilegitimidade-passiva.md) | Arts. 338–339 integrais | 1080 |
| [cpc-recursos-gerais.md](cpc-recursos-gerais.md) | Arts. 994–1.008 integrais | 6760 |
| [cpc-apelacao.md](cpc-apelacao.md) | Arts. 1.009–1.014 integrais | 4056 |
| [cpc-agravo-instrumento.md](cpc-agravo-instrumento.md) | Arts. 1.015–1.020 integrais | 4729 |
| [cpc-agravo-interno.md](cpc-agravo-interno.md) | Art. 1.021 integral | 1169 |

## Método e limites

- Texto transferido diretamente das fontes para arquivos por scripts de captura, sem resumo, paráfrase ou correção editorial. Os scripts de captura não integram este plugin. O manifesto preserva fonte, data, método e hashes dos corpos.
- Planalto: decodificação cp1252 estrita (a tentativa UTF-8 estrita não decodificou as páginas); saída UTF-8. Entidades HTML decodificadas, espaços/quebras de layout normalizados, etiquetas/links excluídos e texto das remissões preservado. Scripts, estilos e cabeçalhos técnicos HTML excluídos. Redações históricas tachadas preservadas como `~~texto~~`; não devem ser confundidas com a redação não tachada.
- **Não foi aplicada normalização Unicode NFC nem NFD.** Não houve reparo de palavras, acentos ou pontuação. Peculiaridades literais da fonte permanecem, como a remissão ao art. 235 da Constituição no art. 1º da Lei 6.938 e `preservá- lo` no art. 225 da CF.
- Intervalos do Código Florestal incluem artigos intercalares dentro dos limites, especialmente 61-A/61-B/61-C; art. 1º fica fora, pois o recorte inicia em 1º-A. CDC termina no art. 104, sem os arts. 104-A/104-B/104-C. Na PNMA, art. 9º não implica os arts. 9º-A e seguintes. O anexo CPC original contém somente os artigos da CAM; do art. 784, preservados o caput identificador e IV/XII, sem outros incisos/parágrafos. Os sete anexos CPC da CAM2 cobrem exatamente 113–138, 338–339 e 994–1.021, sem incluir artigos entre esses intervalos. Os caputs de CF 129/170 também estão declarados; art. 5º contém só os três incisos pedidos.
- Na fonte CPC da CAM2, o art. 998 e o art. 1.003 § 6º trazem redações históricas tachadas seguidas das redações sem tachado; ambas foram transpostas literalmente. A fonte da CAM2 tem SHA-256 `2ff750558ab317c270d4f3f4541b7ea64f9f5506b3edcc6500eafc58792ac007`, diferente do snapshot CPC anterior, e seu texto inclui a remissão à Lei nº 15.484/2026, conforme exibida no Planalto em 01/10/2026.
- A Lei 7.347 foi obtida diretamente de `l7347compilada.htm`, integral, com arts. 1º–23, preâmbulo, assinaturas e nota do DOU. Links de navegação `Texto compilado`/`Mensagem de veto` e asterisco terminal excluídos. As remissões da fonte foram preservadas.
- **CNMP:** foi localizada e capturada a [versão consolidada oficial da Resolução 179/2017](https://www.cnmp.mp.br/portal/images/CALJ/resolucoes/Resoluo-179-alt-res-326.pdf), que já incorpora a alteração do art. 8º e inclusão de seu parágrafo único pela Resolução 326/2026. Não houve consolidação manual. A [ficha oficial da Resolução 326/2026](https://cnmp.mp.br/portal/atos-e-normas/norma/12619/) confirma o ato alterador. O art. 8º anterior, visualmente tachado na página 5, foi transposto como `~~texto~~`; a nova redação está íntegra e sem tachado.
- PDF CNMP: camada textual extraída por `pdftotext -layout -enc UTF-8`, sem OCR; conferência visual das páginas. Só foram removidos cabeçalhos institucionais repetidos, rodapés de paginação e separadores U+000C. Continuação de linhas/páginas reunida em parágrafos. Título, ementa, considerandos, arts. 1º–15 e assinatura preservados.
- A exclusão de tipos penais da Lei 9.605 limita-se à captura dos arts. 3º, 4º e 20, como solicitado. Referências penais nesses artigos, no art. 225 da CF, nos arts. 59–60 do Código Florestal e no art. 15 da PNMA foram preservadas literalmente por integrarem o recorte expressamente pedido. Não foram capturados outros dispositivos penais da Lei 9.605.
- Este corpus comprova a reprodução das fontes oficiais no snapshot de captura; não é auditoria autônoma de constitucionalidade, precedentes, vigência ou exaustividade de alterações posteriores. Nenhum comentário interpretativo foi inserido nos corpos legais.

## Verificação e reprodução

1. Extração HTML confrontada com extração independente por remoção de tags/decodificação de entidades e igualdade literal com espaços normalizados, nas sete fontes originais e no novo snapshot CPC. PDF confrontado por igualdade literal entre texto extraído (sem cabeçalho/rodapé) e corpo final, descontados apenas marcadores de tachado/espaços de layout.
2. Artigos iniciais/finais e conjunto de dispositivos conferidos contra os recortes solicitados, inclusive os 56 artigos da CAM2; arts. 1º–23 da ACP e 1º–15 da resolução integral verificados.
3. A cópia local preserva os 15 corpos normativos e o `manifesto-captura.json`; compare os hashes antes de usar. `DONE` e `DONE-CAM2` registram os gates das capturas originais, sem certificar vigência futura.
4. Os scripts de captura e validação ficaram fora do pacote. Revalidação de fonte, versão e remissões exige procedimento próprio antes de converter um item 🟡 em fundamento.
