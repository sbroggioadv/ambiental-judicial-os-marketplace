---
description: "Enquadra ACP ambiental e encaminha o advogado do autor habilitado à inicial ou o advogado do réu à contestação."
argument-hint: "[polo, fase, objetivo e documentos]"
---

# /ambiental-judicial-acp

Usar $ARGUMENTS para identificar cliente, polo, via/fase, objetivo, autos, atos de ciência e documentos. Não presumir que a mesma peça represente ambos os lados nem aproveitar acervo do adversário. Executar `triagem-ambiental-judicial` quando disponível para fronteira: ACP ajuizada/pedido judicial aqui; anulatória específica do auto tem rota própria; TAC/termo APP/RL/PRA rural sem ação segue a especialidade agrária; defesa/recurso administrativos, CAR/PRA e penal fora. Se triagem não estiver disponível, declarar gate ausente e limitar a saída a pendências.

Executar `legitimidade-acp-ambiental` e `competencia-acp-ambiental` com o corpus literal em `context/`. Só então, conforme **polo escolhido e confirmado**, executar `inicial-acp-ambiental` para autor coletivo habilitado ou `contestacao-acp-ambiental` para réu. Atingido com pretensão individual recebe mapa de via, sem inicial coletiva automática. Não chamar duas peças como saída única.

Aplicar a cada rota `anti-alucinacao-ambiental-judicial` → `validador-ambiental-judicial` → `suprema-corte-ambiental-judicial` R1→R4, inclusive se a saída for bloqueada. Fonte, ato, documento ou controle indisponível significa pendência e revisão não realizada, sem minuta liberada. Registrar `requisito → prova → arquivo/trecho → fonte → situação`, próximo passo e revisão humana. Guidance only; hook não comprova execução. Dados do caso em pasta privada externa por matéria, sem serviço externo não autorizado. Suporte: luis@sbroggio.io.
