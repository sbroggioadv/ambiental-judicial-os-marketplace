---
description: "Roteia TAC ambiental extrajudicial ou ajuste no processo, verificando instrumento e poderes."
argument-hint: "[instrumento, fase, tomador, representado, proposta e documentos]"
---

# /ambiental-judicial-tac

Receber $ARGUMENTS. Aplicar `triagem-ambiental-judicial` e identificar objeto, meio rural, ação em curso, tomador, compromissário, poderes, assinaturas e ato judicial. Imóvel rural começa no `agrario-adv-os`. TAC com MP, inquérito civil ou ACP segue a este plugin após essa triagem; TAC só com órgão ambiental, sem MP e sem ação, segue ao `ambiental-extrajudicial-os`. Para TAC extrajudicial que permanecer neste plugin usar `tac-extrajudicial-ambiental` (20); para ajuste em ação/pedido de homologação usar `tac-judicial-ambiental` (21). Não produzir duas peças para o mesmo instrumento.

Entregar auditoria, minuta/contraproposta ou análise do ato real, cláusulas e pendências. Separar proposta, assinatura e homologação; associação/atingido não vira tomador público. Usar somente corpus `context/` e marcar norma ausente 🟡. Ao final chamar `anti-alucinacao-ambiental-judicial` → `validador-ambiental-judicial` → `suprema-corte-ambiental-judicial` (R1→R4), inclusive se bloqueado. Sem cadeia disponível, não liberar minuta. Dados por matéria em pasta privada externa; sem envio externo não autorizado. **Guidance only.** Suporte: luis@sbroggio.io.
