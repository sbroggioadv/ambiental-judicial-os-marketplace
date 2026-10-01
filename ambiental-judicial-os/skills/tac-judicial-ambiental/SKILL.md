---
name: tac-judicial-ambiental
description: "Esta skill deve ser usada pelo advogado de qualquer polo da ACP ambiental para negociar ajuste em processo e analisar pedido ou ato de homologação."
---

# TAC judicial ambiental

## Entrada

Receber processo, polo, partes e poderes, texto integral da proposta/termo, documentos técnicos, obrigações, pedido de homologação e decisão real, se houver. Identificar se é negociação no curso da ação, termo já assinado, pedido pendente ou acordo efetivamente homologado. A existência da ação não prova assinatura nem homologação; não chamar toda proposta de título judicial.

## Rota obrigatória

Aplicar `triagem-ambiental-judicial`: imóvel rural começa no `agrario-adv-os`. TAC com MP, inquérito civil ou ACP segue neste plugin; se já houver ação, esta skill trata o ajuste judicial. TAC só com órgão ambiental, sem MP e sem ação, segue ao `ambiental-extrajudicial-os`. Na falta desses dados, `PENDENTE DE ENQUADRAMENTO` antes da minuta.

## Procedimento

1. Montar tabela por cláusula: sujeito/poder, objeto, conduta e modo, prazo, prova de cumprimento, cominação, destinação, interesse protegido e objeção. Separar reparação específica, compensação e indenização para evitar duplicidade. Se a prova técnica faltar, pedir avaliação externa; não gerar medidas ou valores fictícios.
2. Conferir `context/resolucao-cnmp-179-tac-integral.md` arts. 1º, 3º e 6º §1º quando o MP for tomador; os dispositivos não são regra geral de homologação de todo acordo. Art. 3º exige olhar poderes do signatário e contém a ressalva “salvo peculiaridades do caso concreto” para obrigações certas, líquidas e exigíveis. Participação de associação/terceiros no §6º não os converte em tomadores públicos.
3. Conferir `context/cpc-tutela-prova-execucao.md` art. 139 V e art. 373 §3º I. O último impede convenção sobre ônus da prova que recaia em direito indisponível. A convenção concreta exige exame do direito, das partes e da cláusula; não usar negociação para presumir renúncia coletiva. O CPC 515, procedimento de homologação e efeitos recursais não estão no corpus 🟡: bloquear classificação definitiva de título/efeito que dependa deles.
4. Para análise de decisão, citar dispositivo e data do ato recebido, alcance homologado e cláusulas excluídas; se não houver ato, elaborar somente pedido condicional e pendências. Execução/cumprimento depende da classificação do título e da camada C5; eficácia penal não é prometida (CNMP 1º §3º).

## Entrega

Entregar minuta de ajuste ou de pedido sujeita à revisão humana, ou análise do ato existente, com quadro `proposta → prova → poderes → fundamento/localizador → estado`. Registrar `MINUTA PARA REVISÃO HUMANA`, `PENDENTE DE PROVA`, `PENDENTE DE FONTE` ou `BLOQUEADO`. Não produzir homologação fictícia.

Norma só após leitura verbatim e conferência de versão em `context/`; artigo faltante = 🟡. Documentos por cliente/matéria em pasta privada externa e sem envio a serviço externo sem autorização específica. Suporte: luis@sbroggio.io. **Guidance only:** o plugin não celebra ou homologa acordo.

Ao final, inclusive em saída bloqueada ou chamada direta, chamar nesta ordem `anti-alucinacao-ambiental-judicial` → `validador-ambiental-judicial` → `suprema-corte-ambiental-judicial` (R1→R4). Registrar achados, corrigir e repetir a cadeia; dependência indisponível impede liberar minuta dependente.
