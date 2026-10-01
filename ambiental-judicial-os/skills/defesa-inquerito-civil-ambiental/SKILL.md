---
name: defesa-inquerito-civil-ambiental
description: "Esta skill deve ser usada pelo advogado do investigado para organizar a defesa em inquérito civil ambiental e distinguir a investigação de TAC rural de APP, RL ou PRA."
---

# Defesa no inquérito civil ambiental

## Entrada e rota

Exigir notificação integral, órgão/expediente, cliente e posição, objeto da investigação, requisição concreta, data e meio de ciência, documentos acessíveis, restrições de acesso fundamentadas, objetivo da defesa e desfecho proposto. Imóvel rural começa sempre no `agrario-adv-os`; o inquérito civil, inclusive com TAC proposto para APP/RL/PRA rural, segue ao `ambiental-judicial-os` após essa triagem. TAC só com órgão ambiental, sem MP e sem ação, segue ao `ambiental-extrajudicial-os`. Se os objetos forem mistos, separar os subpedidos e não supor plugin irmão instalado nem oferecer venda cruzada. Defesa/recurso administrativo de auto e matéria penal ficam fora.

Ler `context/lei-7347-acp-integral.md`, arts. 8º §§1º–2º e 9º §§1º–2º, e `context/cf-ambiental.md`, art. 129 III. Citar texto literal, arquivo, artigo, trecho e versão/captura. A norma e o ato do órgão sobre acesso, sigilo e prazos adicionais estão 🟡.

## Execução

1. Construir linha do tempo de instauração, notificação, requisições, respostas, acesso, eventual proposta de arquivamento e sessão do Conselho Superior, cada passo com documento. Sem ato, não afirmar dever específico ou prazo final.
2. O art. 8º §1º da Lei ACP impõe ao prazo assinalado **pelo MP para sua requisição** piso de dez dias úteis; não transformá-lo em prazo geral de resposta a toda notificação. O art. 9º §1º dá três dias **ao MP para remeter autos arquivados ao Conselho Superior**, não ao investigado. O §2º admite razões escritas/documentos das associações legitimadas até a sessão do Conselho; verificar qualidade e ato da sessão antes de usar.
3. Organizar índice de documentos recebidos/faltantes, fatos admitidos/controvertidos, prova técnica a obter, versão do cliente e pergunta objetiva ao órgão. Pedido de acesso, cópia ou manifestação depende do ato real e da norma aplicável; não prometer acesso irrestrito nem criar sigilo.
4. Entregar rascunho de manifestação somente onde objeto, poder de representação, ato, fonte aplicável e documentos estejam presentes. Não redigir ato do MP, arquivamento, TAC assinado, laudo ou resposta com fatos inventados.

## Saída e controle

Entregar dossiê `ato → data/ciência → exigência → fonte → prova → resposta possível → pendência/responsável`, com estado `MINUTA PARA REVISÃO HUMANA`, `PENDENTE DE PROVA`, `BLOQUEADO` ou `FORA DO RECORTE`. Fonte/ato crítico 🟡 bloqueia afirmação dependente; súmula/tema só número e 🟡.

Chamar antes da manifestação `anti-alucinacao-ambiental-judicial` e `validador-ambiental-judicial`; fechar até a saída de pendências com `anti-alucinacao-ambiental-judicial` → `validador-ambiental-judicial` → `suprema-corte-ambiental-judicial` (R1 documentos; R2 fonte e órgão; R3 marcos; R4 fronteira/sigilo). Registrar achados e não afirmar execução de gate indisponível. Guidance only. Arquivos de caso em pasta privada externa por matéria; serviços externos só com autorização. Suporte: luis@sbroggio.io.
