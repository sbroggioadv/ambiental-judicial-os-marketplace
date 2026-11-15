---
name: contestacao-acp-ambiental
description: "Esta skill deve ser usada pelo advogado do réu para preparar contestação de ACP ambiental com preliminares condicionadas, contraprova e pedidos subsidiários rastreáveis."
---

# Contestação da ACP ambiental

## Entrada e fontes

Receber inicial e anexos integrais, citação/intimação e prova da ciência, decisões, identificação/mandato do réu, cronologia, documentos próprios, pedidos e laudos. Se faltar inicial/citação ou prazo verificável, organizar defesa e pendências, sem prazo final ou contestação pronta. Rodar `legitimidade-acp-ambiental` e `competencia-acp-ambiental` para examinar objeções sem presumir vício.

Ler `context/lei-7347-acp-integral.md`, arts. 1º–5º; `context/cpc-litisconsorcio.md`, arts. 113–118; `context/cpc-intervencao-terceiros.md`, arts. 119–138 pertinentes; `context/cpc-ilegitimidade-passiva.md`, arts. 338–339; `context/cpc-tutela-prova-execucao.md`, arts. 369/373. Vincular afirmação a texto literal, arquivo, trecho e versão/captura. CPC 335–337/341 e contagem estão 🟡: não inventar termo inicial, prazo ou efeitos processuais dependentes.

## Execução

1. Mapear cada alegação/pedido da inicial, documento de suporte, fato admitido, fato controvertido e contraprova. Falta de prova recebida não comprova inexistência de dano ou nexo; ausência de culpa não encerra a análise de responsabilidade objetiva.
2. Examinar legitimidade, competência, interesse, identificação do réu e intervenção **conforme cabimento concreto**. CPC 113–118 não torna todo alegado poluidor litisconsorte necessário. CPC 119–138 requer hipótese própria; não pedir intervenção genérica nem importar regra de processo possessório.
3. Se houver alegação de ilegitimidade, examinar CPC 338–339 e indicar sujeito passivo **sempre que o réu tiver conhecimento**; registrar base factual do conhecimento ou sua ausência. A opção de substituição/inclusão é do autor nas condições do texto, não inclusão automática por esta skill.
4. Separar impugnação principal, objeções subsidiárias, requerimentos de prova e resposta a tutela efetivamente requerida/concedida. Prazo da defesa, ciência e ordem judicial precisam de atos e calendário reais. Não produzir sentença, laudo ou cálculo fictício.
5. Minuta revisável somente com inicial, fatos, prova, mandato e fonte crítica suficientes. Questão 🟡 permanece como pendência, sem fundamento de memória, tese de súmula ou tema não capturado.

## Saída e controle

Entregar quadro `alegação/pedido → documento adverso → posição do réu → contraprova → norma literal → pendência`, preliminares justificadas e minuta condicional ou bloqueio. Chamar antes da conclusão `anti-alucinacao-ambiental-judicial` e `validador-ambiental-judicial`; fechar, inclusive saída bloqueada, com `anti-alucinacao-ambiental-judicial` → `validador-ambiental-judicial` → `suprema-corte-ambiental-judicial` (R1 polo/fatos/prova; R2 normas; R3 ciência/calendário; R4 via/sigilo/revisão humana). Documentar achados; controle indisponível impede liberação e não pode ser declarado executado. Guidance only. Arquivos em pasta privada externa por cliente/matéria. Suporte: suporte@iapx.pro.
