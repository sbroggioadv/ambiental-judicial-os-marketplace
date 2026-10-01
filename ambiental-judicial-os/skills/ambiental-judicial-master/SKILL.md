---
name: ambiental-judicial-master
description: "Esta skill deve ser usada para conduzir pedido civil ambiental judicial de advogado de qualquer polo, da triagem à skill pertinente e à revisão local obrigatória. Não presume legitimidade, decisão, prova ou capacidade instalada."
---

# Master ambiental judicial

## Entrada e rota

Receber pedido, cliente, polo, representado e poderes, interesse/pretensão, via, fase, instrumento, fatos, área, autos, atos de ciência, decisões, documentos, objetivo e urgência. Perguntar **quem tem legitimidade para este ato** e **se há ato urgente/decisão real** antes de produzir. Não fixar polo pelo perfil da instalação. Não misturar acervo de clientes ou matérias.

Executar `triagem-ambiental-judicial` e registrar fronteira e pendências. Encaminhar a uma ou mais skills conforme objeto confirmado: `legitimidade-acp-ambiental`, `competencia-acp-ambiental`, `defesa-inquerito-civil-ambiental`, `inicial-acp-ambiental` ou `contestacao-acp-ambiental`; `responsabilidade-civil-ambiental-objetiva`, `obrigacoes-ambientais-propter-rem`, `nexo-causal-ambiental`, `solidariedade-ambiental`, `onus-e-inversao-prova-ambiental`, `pericia-ambiental-judicial`, `tutela-urgencia-ambiental` ou `obrigacoes-e-astreintes-ambientais`; `tac-extrajudicial-ambiental`, `tac-judicial-ambiental`, `reparacao-integral-ambiental` ou `dano-moral-coletivo-ambiental`; `prescricao-pretensoes-ambientais`, `cumprimento-sentenca-ambiental` ou `execucao-tac-ambiental`; `agravo-liminar-ambiental` ou `apelacao-acp-ambiental`; `anulatoria-auto-infracao-ambiental` para a ação judicial específica do autuado. Escolher **uma rota de peça por polo e ato**. Recurso administrativo, CAR/PRA e crime ambiental saem do recorte. Se a skill de destino não existir em `skills/`, declarar capacidade indisponível e entregar apenas mapa de requisitos; não improvisar a peça.

## Contrato de trabalho

Ler norma somente no `context/` local, conferir dispositivo literal e registrar arquivo, trecho, versão e limite. Artigo sem texto, atualização/alcance não conferidos e remissão não capturada recebem 🟡; tema/súmula só número e 🟡, sem tese. Usar documentos recebidos com autorização; fato alegado não é prova. Não inventar processo, decisão, laudo, prazo final, valor ou ato externo. Suporte: luis@sbroggio.io.

Cada entrega identifica cliente/polo/destinatário, via/fase/ato e quadro `alegação → prova/arquivo/trecho → contraprova/lacuna → dispositivo/versão/localizador → situação`. Separar fato e inferência, pedidos e limites, argumento adversário e cálculo com dados/fórmula quando cabível. A minuta, se permitida, traz `MINUTA PARA REVISÃO HUMANA`; sem base crítica, entregar pendências e próxima providência.

## Fechamento obrigatório

Executar, nesta ordem, `anti-alucinacao-ambiental-judicial` sobre a versão efetiva, `validador-ambiental-judicial` por fundamento e `suprema-corte-ambiental-judicial` R1→R4. Se correção alterar conteúdo, repetir os controles afetados. Uma rota direta passa pelos mesmos controles. Se um controle não estiver disponível ou não for executado, registrar revisão não realizada e impedir liberação de minuta. Hook de orientação não é prova de execução. Não chamar controle recursivamente.

Fechar com achados, alcance e um estado: `MINUTA PARA REVISÃO HUMANA`, `PENDENTE DE PROVA`, `PENDENTE DE FONTE`, `PENDENTE DE ENQUADRAMENTO`, `FORA DO RECORTE` ou `BLOQUEADO`. Falta crítica bloqueia somente a conclusão/peça dependente. Não declarar liminar concedida, TAC celebrado ou homologado, dano comprovado, processo encerrado ou dívida quitada sem ato real. Não protocolar, assinar ou substituir perito, MP ou juízo. Dados ficam na pasta privada externa por matéria; serviço externo exige autorização específica. **Guidance only:** estas chamadas são instruções, não enforcement mecânico.
