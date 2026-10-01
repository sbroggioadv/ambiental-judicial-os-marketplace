---
name: triagem-ambiental-judicial
description: "Esta skill deve ser usada para classificar representado, polo, interesse, instrumento e fase de ACP, inquérito, TAC ou anulatória judicial do auto ambiental. Separa a via coletiva da individual e as fronteiras agrária, administrativa e penal."
---

# Triagem ambiental judicial

## Colher e distinguir

Identificar representado, poderes, outro interessado, polo pretendido, tipo de interesse, dano/conduta alegados, área, objetivo, instrumento, ação individual existente, ACP, inquérito/TAC, auto de infração, decisões, ciência **nos autos**, prazo alegado e urgência. Pedir documento e data para cada ato; ausência é pendência, não negativa de existência. Não presumir que atingido seja legitimado à ACP nem que associação cumpra requisitos sem estatuto, constituição, finalidade e mandato.

## Roteamento

1. **ACP já ajuizada ou pedido judicial ambiental:** este plugin; separar autor coletivo habilitado, réu e atingido com pretensão própria. Conferir `context/lei-7347-acp-integral.md`, arts. 2º, 5º, 8º, 12 e 21, e `context/cdc-tutela-coletiva.md`, arts. 81–82, 103 §3º e 104, conforme a questão. Legitimidade/foro concretos dependem de documentos e fontes complementares 🟡.
2. **Anulatória judicial específica do auto pelo autuado:** rota única para `anulatoria-auto-infracao-ambiental`, se instalada. Distinguir do recurso/defesa administrativa, fora do recorte. `context/cf-ambiental.md`, art. 5º XXXV/LIV/LV, não basta para nulidade, prazo, competência, rito ou minuta; Decreto 6.514/2008, Leis 9.873/1999 e 9.784/1999, processo e norma do órgão estão 🟡 até captura local. Não gerar a mesma peça em dois plugins.
3. **TAC/termo extrajudicial rural de APP/RL/PRA sem ação, ou inquérito civil com esse TAC proposto:** encaminhar à especialidade agrária, sem pressupor outro plugin instalado. **Demais TAC e investigação visando ACP ou objeto não rural:** este plugin. ACP civil em imóvel rural permanece aqui; a mera menção de fazenda não define a rota. Execução de TAC rural sem pedido judicial tem lacuna de destino específico; registrar pendência, não simular capacidade do outro produto.
4. **Defesa/recurso/embargo administrativos, CAR/PRA, licenciamento agropecuário especializado e crime ambiental:** `FORA DO RECORTE`, com indicação da especialidade pertinente, sem impor aquisição de produto.

## Atingido e ação individual

Se houver ação individual, examinar a ciência **nos autos** do ajuizamento coletivo e o prazo textual de **30 dias** do CDC 104 (`context/cdc-tutela-coletiva.md`, art. 104). Não calcular termo final sem ciência documental, regras de contagem e calendário. Examinar CDC 103 §3º e ACP 21 conforme pretensão e título. O alcance do CDC 104 sobre transporte do 103 §3º em ACP difusa é 🟡; suspensão pode ser apontada como cautela de análise, **sem afirmá-la requisito jurídico resolvido**. Não converter ação individual em ACP própria.

## Saída e controles

Entregar `representado → polo → interesse → via/fase → documento/ato → rota → lacuna/estado`, distinguindo fato, declaração e inferência. Informar qual skill existe e qual está indisponível. Para triagem isolada, executar `anti-alucinacao-ambiental-judicial` → `validador-ambiental-judicial` → `suprema-corte-ambiental-judicial` R1→R4 sobre a saída, sem chamadas recursivas. Sem controle, declarar revisão não realizada; sem fonte crítica, `PENDENTE DE FONTE` ou `BLOQUEADO` na conclusão dependente. Dados ficam na matéria privada externa, sem envio não autorizado. **Guidance only.**
