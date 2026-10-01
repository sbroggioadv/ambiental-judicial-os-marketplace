---
name: ambiental-judicial-install
description: "Esta skill deve ser usada para configurar o primeiro uso do ambiental-judicial-os por advogado de réu, autor, associação ou atingido. Define pasta privada e preferências sem receber dossiê nem presumir polo para casos futuros."
---

# Instalação do Ambiental Judicial OS

## Preparar a pasta privada

Pedir ao advogado uma pasta privada externa ao source e a qualquer repositório compartilhado. Confirmar o caminho e a permissão de acesso antes de gravar. Separar cliente e matéria em pastas próprias; não mover documentos existentes, buscar pastas sem autorização nem salvar autos ou dados identificáveis neste plugin. Sem acesso comprovado, mostrar a configuração na conversa e marcar a gravação pendente.

## Configurar

Fazer uma pergunta por vez. Para listas fechadas, usar `AskUserQuestion` com no máximo quatro opções por pergunta; texto livre deve ser digitado. Se a ferramenta não existir, oferecer opções numeradas e explicar que não são botões.

1. Colher caminho privado em texto livre. Não pedir documentos do caso na instalação.
2. Colher perfil: **advogado do réu**, **advogado do autor/associação**, **advogado de atingido**, **atua em mais de um polo**. Perfil é preferência, não autorização para representar partes em conflito; cada caso exige cliente, poderes e polo próprios. Nome/OAB são opcionais e não devem ser inventados.
3. Colher interesse inicial: **ACP**, **inquérito civil/TAC**, **anulatória judicial do auto**, **a definir**. Interesse não afirma cabimento nem disponibilidade de uma skill ainda ausente.
4. Colher tom: **objetivo**, **didático**, **técnico**. Guard, validador e R1→R4 continuam obrigatórios em todos os tons.

Resumir as escolhas e pedir confirmação **Confirmar**, **Corrigir** ou **Não salvar**. Se confirmado e permitido, ler configuração anterior e reconciliar antes de salvar somente preferências necessárias na pasta privada; não sobrescrever silenciosamente. Identificar arquivo gravado ou declarar que nada foi persistido. Não configurar conector externo nem transmitir documentos.

## Primeiro uso

Apresentar `/ambiental-judicial-master` com exemplo sem dados reais: “represento [polo] em [via/fase]; quero [objetivo]; tenho [documentos/decisão]”. O master perguntará legitimidade, representação e ato urgente, se pertinente. Suporte: luis@sbroggio.io. Instalação é operacional, sem parecer jurídico ou revisão de minuta. **Guidance only:** as instruções não provam configuração ou enforcement técnico.
