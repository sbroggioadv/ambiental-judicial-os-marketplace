---
name: anulatoria-auto-infracao-ambiental
description: "Organiza ação anulatória judicial de auto ambiental pelo autuado; entrega matriz documental e bloqueia minuta até capturar normas críticas."
---

# Anulatória judicial do auto de infração ambiental

## Entrada e rota única

Receba autuado/mandato, auto integral, órgão/ente autuante, processo e defesa administrativos completos, notificações e atos de ciência, decisão final/estado do processo, provas, local e fato, objetivo judicial, urgência e pedidos. Confirme que a atuação é **anulatória judicial do auto**, não defesa/recurso administrativo, embargo administrativo, CAR/PRA, ACP ou matéria penal. Rota obrigatória: imóvel rural começa sempre no `agrario-adv-os`, mas a **peça anulatória judicial do auto rural só é produzida neste `ambiental-judicial-os`**. Se o imóvel não for rural, a defesa administrativa tiver sido feita no `ambiental-extrajudicial-os` e não houver ação conexa, encaminhar a continuidade ao `ambiental-extrajudicial-os`. Nos demais casos, esta skill é a rota da anulatória judicial. Se ruralidade, histórico administrativo ou ação conexa não estiverem documentados, `PENDENTE DE ENQUADRAMENTO` e nenhuma peça. Escolher e registrar uma rota por peça; não pressupor plugin irmão instalado nem importar seu corpus. Se houver interesses adversos do mesmo caso, interrompa e peça análise humana de conflito.

## Fonte disponível e bloqueio

Leia `context/cf-ambiental.md`, art. 5º XXXV/LIV/LV, linhas 15–21: acesso à Justiça, devido processo, contraditório e ampla defesa no alcance literal. Essa base **não prova** vício do auto, nulidade, prazo, competência, efeito suspensivo nem procedência. Decreto 6.514/2008, Leis 9.873/1999 e 9.784/1999, CPC sobre competência/rito/tutela e normas/atos do órgão competente estão 🟡 **ausentes deste corpus**. Normas federais não regem automaticamente auto estadual ou municipal. Não buscar agregadores (Jusbrasil/Escavador), não importar texto de outro plugin ou de memória.

## Procedimento permitido

1. Entregue matriz `ato/etapa → data e prova de ciência → vício alegado pela parte → documento/trecho → norma necessária 🟡 → resposta do órgão → prova contrária/lacuna → providência de captura`. Distinguir alegação do autuado de nulidade constatada.
2. Preserve cronologia administrativa e escolha do pedido judicial como hipótese a examinar. Peça versão oficial e recorte aplicável da norma do ente/órgão, mais base processual, para captura **neste** corpus com proveniência. A existência de arquivo em outra pasta não vale como captura aqui.
3. Até fonte crítica e prova do caso estarem conferidas, emitir somente `PENDENTE DE FONTE`/`PENDENTE DE PROVA` e mapa documental. **Bloquear petição inicial, pedido de tutela, prazo final, tese de prescrição/decadência e conclusão de nulidade**. Não prometer suspensão da multa ou reversão da autuação. Após eventual captura, exigir nova validação jurídica antes de mudar esse estado.

Guarde dados na pasta privada externa por cliente/matéria; não faça protocolo nem envio externo sem autorização. Ao final, mesmo bloqueada, chamar `anti-alucinacao-ambiental-judicial` → `validador-ambiental-judicial` → `suprema-corte-ambiental-judicial`, R1 atos/provas, R2 texto/versão, R3 marcos, R4 via/polo/sigilo. Controle indisponível não pode ser declarado executado; mantém bloqueio. Guidance only. Suporte: suporte@iapx.pro.
