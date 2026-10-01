---
name: triagem-ambiental-judicial
description: "Esta skill deve ser usada para classificar representado, polo, interesse, instrumento e fase de ACP, inquérito, TAC ou anulatória judicial do auto ambiental. Separa a via coletiva da individual e as fronteiras agrária, administrativa e penal."
---

# Triagem ambiental judicial

## Colher e distinguir

Identificar representado, poderes, outro interessado, polo pretendido, tipo de interesse, dano/conduta alegados, área, objetivo, instrumento, ação individual existente, ACP, inquérito/TAC, auto de infração, decisões, ciência **nos autos**, prazo alegado e urgência. Pedir documento e data para cada ato; ausência é pendência, não negativa de existência. Não presumir que atingido seja legitimado à ACP nem que associação cumpra requisitos sem estatuto, constituição, finalidade e mandato.

## Roteamento determinístico — primeiro destino e peça

1. Perguntar e documentar se o imóvel é rural. **Se rural, começar sempre no `agrario-adv-os`**, sem pressupor instalação. A triagem agrária é a primeira porta; a ação anulatória de auto rural é produzida somente no `ambiental-judicial-os`. ACP, inquérito civil e TAC com MP seguem para este plugin após essa primeira triagem.
2. Para TAC, verificar tomador e conexão processual. **MP como tomador/parte, inquérito civil ou ACP → `ambiental-judicial-os`**, com `tac-judicial-ambiental` se houver ação e `tac-extrajudicial-ambiental` se ainda não houver ação. **Só órgão ambiental, sem MP e sem ação → `ambiental-extrajudicial-os`**. A regra vale também para imóvel rural, respeitando a primeira porta agrária.
3. Para anulatória do auto, verificar imóvel, histórico da defesa administrativa e ação conexa. **Rural → `agrario-adv-os` primeiro e peça anulatória somente no `ambiental-judicial-os`**. **Não rural + defesa administrativa feita no `ambiental-extrajudicial-os` + ausência comprovada de ação conexa → continuidade no `ambiental-extrajudicial-os`**. Todas as demais anulatórias judiciais → `ambiental-judicial-os`, skill `anulatoria-auto-infracao-ambiental`. Nunca produzir a mesma peça em dois plugins.
4. ACP e pedido judicial ambiental, fora a exceção da continuidade de anulatória não rural acima, seguem neste plugin. Verificar legitimidade, representação, polo e ação individual com as fontes locais. Defesa/recurso administrativos, CAR/PRA, licenciamento especializado e crime ambiental ficam fora deste recorte.

Dado ausente ou contraditório sobre ruralidade, MP, inquérito/ACP, histórico da defesa ou ação conexa = `PENDENTE DE ENQUADRAMENTO`; solicitar documento e não iniciar a peça. Encaminhar ao produto nomeado sem alegar que está instalado ou copiar corpus de outro plugin.

## Atingido e ação individual

Se houver ação individual, examinar a ciência **nos autos** do ajuizamento coletivo e o prazo textual de **30 dias** do CDC 104 (`context/cdc-tutela-coletiva.md`, art. 104). Não calcular termo final sem ciência documental, regras de contagem e calendário. Examinar CDC 103 §3º e ACP 21 conforme pretensão e título. O alcance do CDC 104 sobre transporte do 103 §3º em ACP difusa é 🟡; suspensão pode ser apontada como cautela de análise, **sem afirmá-la requisito jurídico resolvido**. Não converter ação individual em ACP própria.

## Saída e controles

Entregar `representado → polo → interesse → via/fase → documento/ato → rota → lacuna/estado`, distinguindo fato, declaração e inferência. Informar qual skill existe e qual está indisponível. Para triagem isolada, executar `anti-alucinacao-ambiental-judicial` → `validador-ambiental-judicial` → `suprema-corte-ambiental-judicial` R1→R4 sobre a saída, sem chamadas recursivas. Sem controle, declarar revisão não realizada; sem fonte crítica, `PENDENTE DE FONTE` ou `BLOQUEADO` na conclusão dependente. Dados ficam na matéria privada externa, sem envio não autorizado. **Guidance only.**
