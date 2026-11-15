---
name: obrigacoes-e-astreintes-ambientais
description: "Esta skill deve ser usada pelo advogado de qualquer polo da ACP ambiental para estruturar obrigação de fazer ou não fazer e examinar multa judicial."
---

# Obrigações e astreintes ambientais

## Entrada

Identificar representado/polo, pretensão, obrigação proposta ou imposta, título e versão, decisão/termo, intimação, possibilidade técnica de cumprir, marcos de cumprimento, prova, multa, pagamentos e cálculos. Separar obrigação judicial de termo extrajudicial, multa coercitiva, multa convencional e indenização. Não tratar multa de TAC como astreinte nem embargo administrativo como decisão judicial.

## Procedimento

1. Descrever para cada dever conduta verificável, sujeito obrigado, local, termo inicial, prazo do ato real, parâmetro de cumprimento, meio de prova e impossibilidade alegada. Para o autor, formular pedido delimitado; para o réu, testar viabilidade e propor ajuste com prova. Sem suporte técnico, marcar método, metragem e custo 🟡.
2. Ler `context/lei-7347-acp-integral.md` arts. 11 e 12 §2º e `context/cpc-tutela-prova-execucao.md` arts. 497–501 e 536–537. Arts. 497/499 priorizam tutela específica ou resultado equivalente conforme hipótese; no art. 499 parágrafo único, nas hipóteses enumeradas, conversão requerida exige primeiro faculdade de cumprimento específico. Art. 500 distingue perdas e danos da multa coercitiva.
3. Para multa judicial, conferir ato que a fixou, destinatário, valor, periodicidade, prazo razoável, ciência e prova de descumprimento. Construir tabela `base do ato → início comprovado → unidades de incidência → valor por unidade → abatimentos → total provisório`. Art. 537 §§1º–4º exige examinar alteração de multa vincenda, depósito no cumprimento provisório e início da incidência; ACP 12 §2º disciplina exigibilidade da multa cominada liminarmente. Não anunciar levantamento, exigibilidade ou total sem confrontar os dois textos e o estado do processo.
4. Art. 536 §4º remete ao CPC 525 ausente 🟡. Impugnação executiva completa, contagem e rito local dependem de captura. Se o pedido for de execução de sentença, encaminhar a `cumprimento-sentenca-ambiental`; se for execução de TAC, a `execucao-tac-ambiental`, sem fabricar peça pronta.

## Saída

Entregar pedido/contraproposta, matriz por obrigação e memória de cálculo reexecutável ou lacuna calculatória. Explicitar objeção do outro polo, prova necessária e estado `MINUTA PARA REVISÃO HUMANA`, `PENDENTE DE PROVA`, `PENDENTE DE FONTE` ou `BLOQUEADO`.

Fundamentar só após leitura verbatim e conferência de versão em `context/`; artigo faltante = 🟡. Documentos privados por cliente/matéria fora do source; serviço externo só com autorização específica. Suporte: suporte@iapx.pro. **Guidance only:** não há decisão judicial ou cobrança automática.

Ao final, inclusive em saída bloqueada ou chamada direta, chamar nesta ordem `anti-alucinacao-ambiental-judicial` → `validador-ambiental-judicial` → `suprema-corte-ambiental-judicial` (R1→R4). Registrar achados, corrigir e repetir a cadeia; dependência indisponível impede liberar minuta dependente.
