---
name: tac-extrajudicial-ambiental
description: "Esta skill deve ser usada pelo advogado de qualquer lado cabível para auditar ou negociar TAC ambiental extrajudicial com MP ou em inquérito civil, após a triagem agrária inicial quando houver imóvel rural."
---

# TAC extrajudicial ambiental

## Entrada e fronteira

Identificar representado, interesse, órgão tomador, procedimento, instrumento recebido ou proposta, poderes de representação, objeto ambiental, laudo, obrigações, valores, multas e estado das assinaturas. Aplicar a triagem antes de qualquer minuta: imóvel rural começa no `agrario-adv-os`; MP como tomador/parte, inquérito civil ou ACP mantém o TAC no `ambiental-judicial-os` após essa primeira triagem. TAC apenas com órgão ambiental, sem MP e sem ação, segue ao `ambiental-extrajudicial-os`, mesmo em imóvel rural após a triagem agrária. Se houver ação, usar `tac-judicial-ambiental`. Faltando prova do tomador, inquérito, ação ou ruralidade, `PENDENTE DE ENQUADRAMENTO` e nenhuma minuta. Associação ou atingido pode participar quando couber, mas não ganha poder de tomador público por legitimidade à ACP.

## Procedimento

1. Classificar cada cláusula: sujeito, conduta, local, modo, prazo, prova técnica, fiscalização, cominação, mitigação/compensação/indenização e destinatário. Montar `cláusula → fato/prova → fundamento literal → custo/documento → objeção/ajuste`. Para o compromissário, identificar dever inexequível ou não mensurável com prova; para o lado interessado, conferir suficiência ambiental sem inventar área ou custo.
2. Ler `context/lei-7347-acp-integral.md` art. 5º §6º e `context/resolucao-cnmp-179-tac-integral.md` arts. 1º–5º, 7º e 9º–12. A resolução disciplina TAC tomado no âmbito do MP; não generalizar seu rito a qualquer órgão. Art. 3º caput pede obrigações certas, líquidas e exigíveis, **salvo peculiaridades do caso concreto**; §§1º–4º tratam de assinatura, poderes e advogado, e §6º admite participação sem transferir a posição de tomador. Conferir representante e mandato documentalmente.
3. Art. 1º §1º não autoriza renúncia a direitos difusos/coletivos pelo MP. §3º não promete afastamento penal ou administrativo automático. Art. 4º trata de cominação do termo; distingui-la de astreinte judicial. Art. 5º e parágrafos tratam de destinação no alcance do MP; art. 7º de publicidade pelo órgão superior do MP, não obrigação geral de publicação por qualquer tomador.
4. Só marcar TAC celebrado e título extrajudicial após instrumento assinado e conferido. Conferir CPC 784 IV/XII no `context/cpc-tutela-prova-execucao.md` conforme o instrumento; esses incisos não suprem rito executivo completo 🟡. Execução segue skill 26 com exigibilidade e inadimplemento reais. Norma local do órgão, especialidade técnica e jurisprudência sem texto permanecem 🟡.

## Entrega

Entregar auditoria ou minuta/contraproposta identificada para revisão humana, matriz de obrigações, poderes, documentos, divergências e estado `MINUTA PARA REVISÃO HUMANA`, `PENDENTE DE PROVA`, `PENDENTE DE FONTE`, `PENDENTE DE ENQUADRAMENTO` ou `BLOQUEADO`. Não afirmar celebração, homologação, quitação ou eficácia penal.

Somente texto verbatim e versão conferida em `context/` fundamentam norma; artigo sem texto = 🟡. Isolar documentos por cliente/matéria em pasta privada fora do source; não enviá-los a serviços externos sem autorização específica. Suporte: suporte@iapx.pro. **Guidance only:** o plugin não toma, assina ou fiscaliza TAC.

Ao final, inclusive em saída bloqueada ou chamada direta, chamar nesta ordem `anti-alucinacao-ambiental-judicial` → `validador-ambiental-judicial` → `suprema-corte-ambiental-judicial` (R1→R4). Registrar achados, corrigir e repetir a cadeia; dependência indisponível impede liberar minuta dependente.
