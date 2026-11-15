---
name: prescricao-pretensoes-ambientais
description: "Separa pretensões civis ambientais e organiza marcos e fontes para análise de prescrição do autor ou do réu, sem tese ou prazo material presumido."
---

# Prescrição das pretensões ambientais

## Entrada e enquadramento

Receba cliente e polo, pretensão específica, titulares, pedido, título e sua natureza, fatos, datas e comprovantes de ciência, ajuizamento, trânsito e eventuais atos interruptivos/suspensivos alegados. Separe reparação coletiva, indenização individual, multa judicial, multa do TAC e execução de título. Defesa/recurso administrativo e prescrição da sanção administrativa ficam fora desta skill; anulatória judicial do auto segue `anulatoria-auto-infracao-ambiental` com fontes próprias 🟡. Não transportar o regime de uma pretensão para outra.

## Fonte e trabalho

O corpus `context/` ainda **não contém âncora material suficiente** para afirmar regime ou prazo prescricional civil. `Tema 999/STF 🟡` é apenas número pendente; não atribuir assunto, tese ou efeito. CC 189/202/205/206 🟡 são alvos sem texto local: não citar seu conteúdo nem preencher de memória. Eventual dispositivo processual sobre prescrição não resolve por si a duração material da pretensão. Nunca chamar multa, execução ou pretensão individual de imprescritível por analogia.

1. Entregue matriz `pretensão → titular/polo → fato/ato comprovado → data e prova → fonte literal disponível → fonte crítica 🟡 → hipótese concorrente → risco/medida de pesquisa`.
2. Ordene os marcos cronológicos sem criar termo inicial, interrupção, suspensão ou data final. Se parte alegar esses efeitos, registre como alegação e peça texto crítico e prova do ato.
3. Só formule conclusão material ou peça dependente após capturar **neste** corpus o regime pertinente, conferir redação/versão e aplicar a fatos reais. Sem isso, estado `PENDENTE DE FONTE`; o mapa de investigação é entregável, mas tese prescricional conclusiva e minuta fundada nela ficam bloqueadas.

## Saída e revisão

Entregue posições possíveis do autor e réu separadas, evidências faltantes e próxima providência, sem prognóstico. Use dados somente na pasta privada externa por cliente/matéria, nunca no source ou serviço externo sem autorização.

Ao final, inclusive se bloquear, chamar `anti-alucinacao-ambiental-judicial` → `validador-ambiental-judicial` → `suprema-corte-ambiental-judicial`, R1 fatos/provas, R2 fontes/alcance, R3 marcos, R4 via/polo/sigilo. Controle indisponível significa revisão pendente, sem liberar peça. Guidance only; não é enforcement por hook. Suporte: suporte@iapx.pro.
