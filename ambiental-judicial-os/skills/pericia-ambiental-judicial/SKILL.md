---
name: pericia-ambiental-judicial
description: "Esta skill deve ser usada pelo advogado de qualquer polo da ACP ambiental para organizar quesitos, examinar laudo e pedir esclarecimentos com lastro documental."
---

# Perícia ambiental judicial

## Entrada e fronteira

Identificar representado, polo, processo, objeto controvertido, decisão de produção de prova, intimação, laudos, mapas, séries de dados, método, autoria, assistente técnico e objetivo. Separar documento técnico recebido, alegação da parte e conclusão do perito. A assistência jurídica não produz ART, medição, análise laboratorial, laudo assinado ou estimativa ambiental fictícia. Sem processo ou ato real, entregar plano de prova e quesitos propostos, sem afirmar que houve nomeação ou abertura de prazo.

## Procedimento

1. Montar matriz `ponto controvertido → fato alegado → documento/trecho → dado técnico necessário → quesito → risco de contraprova`. Formular quesitos que identifiquem área, período, método, incerteza, causalidade alternativa e medidas propostas, sem preencher resultado esperado.
2. Conferir `context/cpc-tutela-prova-execucao.md` arts. 464–480. No art. 464, distinguir exame, vistoria e avaliação; examinar necessidade, substituição por prova técnica simplificada e limites da perícia. No art. 465 §1º, há 15 dias textuais da intimação do despacho de nomeação para impugnação cabível, assistente e quesitos. Prazo final exige despacho, ciência e calendário reais; art. 95, mencionado para honorários, não foi capturado 🟡.
3. Para laudo recebido, confrontar objeto, análise, método, respostas e limites com art. 473; apontar página, passagem, dado faltante, inconsistência e quesito de esclarecimento. Art. 477 §1º prevê manifestação em 15 dias textuais; §2º prevê esclarecimento pelo perito e §3º perguntas em audiência. Não afirmar deficiência apenas por discordância do resultado.
4. Registrar se há pedido de nova perícia e qual ponto ficou insuficientemente esclarecido (art. 480). Art. 479 remete ao art. 371 não capturado 🟡; não inventar regra completa de valoração. Ler também `context/lei-7347-acp-integral.md`, art. 18: nas ações dessa lei não há adiantamento de honorários periciais e outras despesas; a associação autora não será condenada em honorários de advogado, custas e despesas processuais, salvo comprovada má-fé. Isso não autoriza gratuidade universal. Custeio concreto, art. 95 do CPC, norma técnica específica e rito local permanecem 🟡 quando necessários.

## Entrega

Entregar quesitos ou crítica documental ao laudo com fundamento e contraprova, pedido de esclarecimento apenas se houver suporte, responsável técnico externo, documentos faltantes e próxima providência. Para ambos os polos, explicitar a tese oposta e a incerteza que a prova não resolveu. Registrar estado `MINUTA PARA REVISÃO HUMANA`, `PENDENTE DE PROVA`, `PENDENTE DE FONTE` ou `BLOQUEADO`.

Ler cada fundamento no `context/` do próprio plugin, verificar versão e localizador; artigo sem texto permanece 🟡. Guardar documentos de cliente por matéria em pasta privada externa ao source. Sem envio externo sem autorização específica. Suporte: suporte@iapx.pro. **Guidance only:** este texto orienta a execução; não é validação automática nem substitui perito ou advogado.

Ao final, inclusive em saída bloqueada ou chamada direta, chamar nesta ordem `anti-alucinacao-ambiental-judicial` → `validador-ambiental-judicial` → `suprema-corte-ambiental-judicial` (R1→R4). Registrar achados, corrigir e repetir a cadeia; se alguma dependência faltar, informar revisão não realizada e não liberar minuta dependente.
