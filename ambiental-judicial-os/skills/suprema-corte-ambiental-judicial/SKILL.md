---
name: suprema-corte-ambiental-judicial
description: "Esta skill deve ser usada para auditar toda entrega ambiental judicial em R1→R4 após guard e validador, inclusive comandos diretos e saídas bloqueadas. Libera apenas minuta para revisão humana ou registra impedimento."
---

# Suprema Corte ambiental judicial

Receber versão efetiva da saída, matriz de documentos e fundamentos, cálculos, pendências e resultados de `anti-alucinacao-ambiental-judicial` e `validador-ambiental-judicial`. Se algum controle não rodou, executá-lo antes; se indisponível, registrar revisão não realizada e impedir liberação. Sem minuta, revisar apenas o mapa recebido. Revisão **default-on**, R1→R4 em ordem, inclusive chamada direta ou pedido para pular gate. Não simular revisores independentes ou decisão judicial. **Guidance only:** a skill não é tribunal nem mecanismo de enforcement.

## R1 — Fatos e atores

Conferir cliente, polo, representação/mandato, legitimidade, interesse, cronologia, dano alegado, conduta versus titularidade, área, documentos, laudo e contraprova. Distinguir relato, fato provado e inferência. Exigir ato real para decisão, ciência, TAC, homologação, título e cumprimento. Atingido não se torna autor de ACP automaticamente; réu e autor não compartilham peça ou acervo.

## R2 — Fundamentos

Revisar cada selo do validador com dispositivo/trecho literal em `context/`, versão/captura, alcance e alterações. 🟡 não sustenta conclusão dependente. Remissão não capturada, veto/revogação, jurisprudência só numerada e texto vindo de outro plugin não viram regra. Preservar distinção entre PNMA, Código Florestal, LACP, CDC, CPC e Resolução CNMP 179; não criar tese de solidariedade, prescrição, nexo ou efeito coletivo por memória.

## R3 — Marcos e cálculos

Checar decisão/publicação/intimação/ciência nos autos e calendário antes de qualquer prazo final. Separar prazo processual, prazo textual CDC 104, cronograma TAC, multa, prescrição material e administrativa. Agravo de instrumento da tutela interlocutória, agravo do ACP 12 §1º contra suspensão pelo Presidente e apelação têm objetos distintos. Cálculos exigem valor, unidade, fórmula e documento; inexistindo dados, deixar pendente. Tema 999/STF permanece número + 🟡.

## R4 — Via, forma e sigilo

Conferir legitimidade, competência e poderes; ACP versus ação individual; inquérito versus TAC; TAC rural extrajudicial versus pedido judicial; anulatória judicial versus recurso administrativo; título judicial versus extrajudicial; pedido principal/subsidiário, prova/contraprova e revisão humana. Recurso fora do rol não é produzido por analogia. Não protocolar, assinar, julgar, homologar, certificar reparação ou substituir perito/MP/juízo. Dados ficam na pasta privada externa por matéria; envio externo só com autorização específica.

## Resultado

Para cada rodada registrar `objeto → achado → prova/arquivo/trecho → gravidade → correção → residual` e `PASS`, `CONCERNS` ou `FAIL` no alcance revisado. Continuar as rodadas para diagnóstico mesmo após impedimento; após correção, repetir rodadas afetadas sobre a nova versão. Resultado global não supera impedimento residual. Encerrar com `MINUTA PARA REVISÃO HUMANA` somente se não houver falta crítica no alcance entregue; senão `PENDENTE DE PROVA`, `PENDENTE DE FONTE`, `PENDENTE DE ENQUADRAMENTO`, `FORA DO RECORTE` ou `BLOQUEADO`, com próximo passo e responsável. Instrução escrita e hook echo não provam revisão executada nem prontidão do produto. Suporte: suporte@iapx.pro.
