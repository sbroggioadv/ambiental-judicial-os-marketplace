---
name: obrigacoes-ambientais-propter-rem
description: "Esta skill deve ser usada pelo advogado de autor habilitado ou réu em ACP ajuizada ou pedido judicial ambiental para mapear deveres reais de APP ou Reserva Legal, transmissão de domínio ou posse e prova temporal; TAC rural extrajudicial sem ação segue outra rota."
---

# Obrigações ambientais de natureza real

## Entrada e fronteira

Receber cliente/polo, via/fase, imóvel e objeto exato (APP, Reserva Legal ou outro), matrículas e títulos, cadeia de domínio/posse e datas, atos de supressão e aquisição, documentos técnicos, pedidos e decisão existente. Confirmar ACP ajuizada ou pedido judicial. TAC/termo extrajudicial de APP/RL/PRA rural sem ação e inquérito civil com esse TAC proposto devem ser encaminhados ao recorte agrário, sem pressupor plugin irmão instalado; não produzir a peça duplicada. CAR/PRA, metragem ou licenciamento agropecuário especializados ficam fora.

## Procedimento

1. Construir linha do tempo por imóvel e por sujeito: `domínio/posse → período → obrigação legal invocada → situação da vegetação → ato/prova → pedido`. Separar alienante, adquirente, possuidor e ocupante; apontar intervalo e documentos ausentes.
2. Conferir `context/lei-12651-codigo-florestal.md`: art. 2º §2º atribui natureza real às **obrigações previstas nessa Lei** e as transmite ao sucessor no caso de transferência de domínio ou posse do **imóvel rural**. O art. 7º caput/§§1º–2º trata de manutenção e recomposição de vegetação em APP e transmite a obrigação do §1º no caso de transferência de domínio ou posse do **imóvel rural**. O art. 66 caput/§1º cuida da regularização da Reserva Legal na situação temporal ali descrita e transmite a obrigação do caput no caso de transferência de domínio ou posse do **imóvel rural**. Fora desse pressuposto rural, esses dispositivos não fundamentam a transmissão; marcar o dever real alegado como 🟡/`PENDENTE DE FONTE`. Aplicar só o dispositivo cujo objeto e pressupostos estejam demonstrados.
3. Examinar separadamente `dever de recompor/manter` e `imputação indenizatória por dano`. Transmissão da obrigação real não prova, por si, conduta lesiva anterior, extensão do dano ou nexo para indenização. Se a pretensão incluir indenização civil, acionar `responsabilidade-civil-ambiental-objetiva` e `nexo-causal-ambiental` com prova própria.
4. Pelo autor, indicar de quem e por qual título pede obrigação específica; pelo réu, confrontar cadeia, objeto, datas, cumprimento e alcance do pedido. Não inferir exoneração automática do alienante ou inclusão automática do adquirente além do texto e das provas.

## Âncoras e pendências

- `context/lei-12651-codigo-florestal.md`: art. 2º §2º (linha 53), art. 7º §§1º–2º (337–341), art. 66 caput/§1º (769–777): transmissão no caso de transferência de domínio ou posse do **imóvel rural**; reler texto literal no uso. O art. 2º §1º (linha 51), que remete ao rito sumário do CPC/1973, não é usado.
- `context/lei-6938-pnma.md`: arts. 3º IV e 14 §1º somente para eventual imputação civil separada.
- Tema 1204/STJ 🟡; Súmula 623/STJ 🟡, candidatas. Estes números não fornecem tese, assunto, transcrição nem resultado sem fonte oficial verificada neste corpus. Norma técnica/local, estado da área e medidas específicas também permanecem 🟡 até prova e fonte.

## Entrega e revisão obrigatória

Entregar matriz temporal `sujeito → título de domínio/posse → datas → obrigação legal delimitada → arquivo/trecho → cumprimento/contraprova → lacuna`, com posições de ambos os lados e pedido possível condicionado. Estado `PENDENTE DE PROVA`, `PENDENTE DE FONTE`, `FORA DO RECORTE` ou `MINUTA PARA REVISÃO HUMANA`, conforme o caso. Não certificar restauração, área ou custo sem medição e documento técnico reais.

Guardar documentos na pasta privada por cliente/matéria, fora do source; nenhum envio externo de dados sem autorização específica. Suporte: luis@sbroggio.io. **Guidance only:** os controles por instrução não são enforcement automático.

Ao final, inclusive para bloqueio e invocação direta, chamar `anti-alucinacao-ambiental-judicial` → `validador-ambiental-judicial` → `suprema-corte-ambiental-judicial` (R1→R4); corrigir achados e repetir a cadeia. Dependência indisponível impede liberar minuta: entregar matriz e pendências, registrando a revisão não realizada.
