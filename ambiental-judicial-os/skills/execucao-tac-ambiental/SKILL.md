---
name: execucao-tac-ambiental
description: "Classifica título e inadimplemento de TAC ambiental e prepara mapa executivo ou defesa para o polo habilitado, com fronteira rural."
---

# Execução de TAC ambiental

## Entrada, fronteira e título

Receba termo integral assinado, celebrantes/poderes, objeto, local, existência de ação/homologação, cláusulas, vencimentos, ciência, fiscalização, pagamentos e prova técnica. Aplique `triagem-ambiental-judicial`: imóvel rural começa no `agrario-adv-os`; TAC com MP, inquérito civil ou ACP segue a este plugin após essa triagem; TAC só com órgão ambiental, sem MP e sem ação, segue ao `ambiental-extrajudicial-os`. Não presumir plugin irmão instalado ou duplicar peça. TAC judicial homologado segue `cumprimento-sentenca-ambiental` conforme título, sem rotulá-lo extrajudicial.

Leia `context/lei-7347-acp-integral.md`, art. 5º §6º; `context/resolucao-cnmp-179-tac-integral.md`, arts. 3º caput, 11 e 12; `context/cpc-tutela-prova-execucao.md`, art. 784 IV/XII. A resolução CNMP disciplina o MP no alcance lido, não qualquer celebrante. O art. 3º exige obrigações certas, líquidas e exigíveis **salvo peculiaridades do caso concreto**: examinar cláusula e caso, sem alegar nulidade automática. O art. 11 descreve atuação do órgão do MP e prazo próprio, não prazo de defesa do compromissário. Art. 12 trata hipótese de omissão de outro órgão público; não dá poder universal a particulares.

## Procedimento e saída

1. Classifique instrumento e título com assinaturas e base literal. Separe celebração, eventual homologação, fiscalização e inadimplemento comprovados. Minuta não assinada ou mera proposta não são título.
2. Para cada obrigação, faça `cláusula → sujeito → vencimento/condição → prova de execução → mora alegada e contraprova → valor/multa contratual → cálculo → lacuna`. Diferencie multa do termo de astreinte judicial e indenização; pagamentos exigem comprovantes e imputação específica.
3. Exequente: identifique cláusulas vencidas e pedido compatível com título e legitimidade. Executado: identifique pagamento, cumprimento parcial, inexigibilidade alegada e documento de suporte. Não certifique restauração por imagem isolada ou crie laudo.
4. CPC 771/783/786/815–821/914/917 e rito/defesa integral estão 🟡 sem texto local. Sem fonte crítica, título, exigibilidade ou ato comprovado, entregue mapa e bloqueie petição executiva/defesa pronta dependente. Não invente prazo ou via.

Guardar dados na pasta privada externa por cliente/matéria, sem serviço externo não autorizado. Ao final, inclusive saída bloqueada, chamar `anti-alucinacao-ambiental-judicial` → `validador-ambiental-judicial` → `suprema-corte-ambiental-judicial`, R1 termo/provas, R2 título/fonte, R3 vencimentos/cálculos, R4 via/polo/sigilo. Se controle indisponível, revisão pendente e nenhuma peça liberada. Guidance only. Suporte: luis@sbroggio.io.
