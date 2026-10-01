---
name: validador-ambiental-judicial
description: "Esta skill deve ser usada para validar cada fundamento de entrega civil ambiental judicial contra dispositivo literal, arquivo, versão e alcance do corpus local. Artigo sem texto, remissão não capturada e jurisprudência ficam pendentes."
---

# Validador normativo ambiental judicial

Receber minuta/matriz, resultado do guard, data dos fatos e atos, polo, via, fonte alegada e pretensão. Ler `context/INDICE.md`, manifesto e arquivo literal pertinente em `context/`; conferir **o dispositivo e a redação**, não apenas o nome do arquivo. Registrar diploma/dispositivo, trecho, arquivo/localizador, captura/versão declarada, hash se conferido, data relevante, alterações/vetos/remissões, destinatário, alcance e pendência. Integridade local não prova vigência externa nem aplicação ao caso. Se atualização ou suspensão não foi conferida, declará-la não comprovada.

Classificar por fundamento: **✅ texto local conferido no alcance descrito**, **🟡 fonte/versão/aplicação/prova pendente**, **🔴 contradição ou uso de texto vetado/revogado**. ✅ nunca é aprovação da peça ou certeza de cabimento. Artigo só numerado, trecho ausente, remissão para artigo não capturado e jurisprudência recebem 🟡. Tema 1204/STJ, Tema 999/STF e Súmulas 618/623/629 do STJ, se citados, ficam **somente como número + 🟡**; não associar assunto ou tese. Não importar selo do agrário nem consultar Jusbrasil/Escavador.

## Pontos de controle do corpus

| Tema | Texto local e limite |
|---|---|
| ACP/legitimidade/indivíduo | `lei-7347-acp-integral.md` arts. 2º, 5º, 8º, 12, 16, 19 e 21; `cdc-tutela-coletiva.md` arts. 81–82, 97–100, 103 §3º e 104. ACP 5º V `a` e `b` cumulativos; §4º não dispensa finalidade. CDC 104: ciência nos autos e 30 dias textuais; alcance na ACP difusa 🟡. ACP 16 e remissão do 19 exigem controle complementar 🟡. |
| Responsabilidade e prova | `lei-6938-pnma.md` arts. 3º IV e 14 §1º; `cf-ambiental.md` art. 225; `lei-12651-codigo-florestal.md` arts. 2º §2º, 7º §§1º–2º e 66 §1º; `cpc-tutela-prova-execucao.md` arts. 369/373/464–480. Não inferir solidariedade universal, nexo automático, qualquer obrigação propter rem ou conteúdo da Súmula 618/623/629. |
| Tutela, obrigações e TAC | `lei-7347-acp-integral.md` arts. 4º, 5º §6º, 11–14; `cpc-tutela-prova-execucao.md` arts. 300–311, 497–501, 536–537 e 784 no recorte; `resolucao-cnmp-179-tac-integral.md` no âmbito do MP. Não chamar proposta de TAC celebrado/homologado ou título exigível sem instrumento e atos. |
| Recurso | `cpc-recursos-gerais.md` arts. 994–1.008; `cpc-agravo-instrumento.md` arts. 1.015–1.020; `cpc-apelacao.md` arts. 1.009–1.014; `cpc-agravo-interno.md` art. 1.021 para distinção. ACP 12 §1º tem agravo próprio contra suspensão da liminar pelo Presidente do Tribunal; não confundir com agravo de instrumento. Prazo final depende de decisão, ciência e calendário; CPC 219/224/231 🟡. |
| Anulatória judicial do auto | `cf-ambiental.md` art. 5º XXXV/LIV/LV. Decreto 6.514/2008, Leis 9.873/1999 e 9.784/1999, competência, rito e norma do órgão 🟡; não afirmar vício, nulidade, prescrição ou prazo com base só na CF. |

Outras lacunas críticas do rol: CPC 75/103/105, 319/320, 335–337/341, 509/513/515/523–525, 771/783/786/815–821/914/917; CC 186/187/927/942 e 189/202/205/206, quando necessários, 🟡. Um artigo em outro corpus não sana o recorte local. Sem fonte crítica, bloquear a peça/conclusão dependente e entregar mapa documental possível.

Saída: `fundamento → texto/arquivo/versão → selo → alcance → lacuna → etapa impedida`, com distinção entre integridade e vigência. Passar o resultado à `suprema-corte-ambiental-judicial` R1→R4 na cadeia; se acionado isoladamente, completar guard antes e Suprema Corte depois. Não chamar recursivamente quando já integrado. **Guidance only:** nenhum hook confirma leitura ou conferência.
