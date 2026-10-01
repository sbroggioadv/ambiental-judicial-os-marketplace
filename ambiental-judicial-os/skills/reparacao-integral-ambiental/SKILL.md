---
name: reparacao-integral-ambiental
description: "Esta skill deve ser usada pelo advogado de qualquer polo da ACP ambiental para estruturar medidas de reparação com prova técnica e evitar duplicidade de pedidos."
---

# Reparação integral ambiental

## Entrada

Identificar representado/polo, dano alegado, local/período, sujeitos, laudos e dados, estado do bem, medidas possíveis, custos documentados, destinatários, pagamentos e pedidos já formulados. Não usar o nome “integral” para presumir nexo, área, método, valor ou responsabilidade. Dimensionamento agrário especializado e CAR/PRA não são calculados aqui; ACP judicial sobre imóvel rural continua no recorte.

## Procedimento

1. Construir matriz `componente ambiental → condição anterior/atual documentada → medida específica → responsável alegado → indicador técnico → custo comprovado → incerteza`. Separar restauração específica, resultado equivalente, mitigação, compensação e indenização; explicitar sobreposição e pagamentos para não cobrar duas vezes o mesmo componente.
2. Conferir `context/lei-6938-pnma.md` arts. 4º VII e 14 §1º, `context/lei-7347-acp-integral.md` arts. 3º, 11 e 13 e `context/cpc-tutela-prova-execucao.md` arts. 497, 499 e 500. PNMA 14 §1º exige vincular sujeito e dano; não dispensa prova de nexo no caso. No CPC 499 parágrafo único, nas hipóteses ali enumeradas, a conversão requerida em perdas e danos exige primeiro faculdade de cumprimento específico. Art. 500 distingue indenização da multa coercitiva.
3. Se o caminho for TAC tomado pelo MP, conferir `context/resolucao-cnmp-179-tac-integral.md` arts. 1º §1º e 5º com seus parágrafos; não transportar regra de destinação do MP a todo acordo ou ao patrimônio do atingido. Conferir destinatário de cada parcela e fundamento efetivamente aplicável.
4. Para o réu, formular contraprova, impossibilidade ou alternativa com suporte técnico; para o autor, justificar alcance e fiscalização com dados. Súmula 629/STJ 🟡: só o número, sem tese ou ementa até fonte oficial. Técnica, custos, cumulação concreta e norma local faltantes permanecem 🟡 e bloqueiam quantificação dependente.

## Entrega

Entregar quadro de reparação e pedido/contraproposta com fundamento local, rubricas não sobrepostas, prova, fórmula/dados de valor quando houver e lacunas técnicas. Estado `MINUTA PARA REVISÃO HUMANA`, `PENDENTE DE PROVA`, `PENDENTE DE FONTE` ou `BLOQUEADO`. Não certificar restauração nem cumprimento por suposição.

Usar só texto verbatim em `context/`, com versão/localizador conferidos; artigo não capturado = 🟡. Documentos privados por cliente/matéria fora do source; serviço externo somente com autorização específica. Suporte: luis@sbroggio.io. **Guidance only:** a skill não substitui laudo/perito ou decisão judicial.

Ao final, inclusive em saída bloqueada ou chamada direta, chamar nesta ordem `anti-alucinacao-ambiental-judicial` → `validador-ambiental-judicial` → `suprema-corte-ambiental-judicial` (R1→R4). Registrar achados, corrigir e repetir a cadeia; dependência indisponível impede liberar minuta dependente.
