# Ambiental Judicial OS

`ambiental-judicial-os` · versão 0.1.0 · Luis Sbroggio.

Plugin para o **advogado de qualquer dos polos**, conforme legitimidade, representação e via comprovadas: réu em ação civil pública ambiental; autor, associação ou atingido. O produto contém manifestos, licença, hook, corpus local, **29 skills e 19 comandos**.

## Estado da entrega

As portas `/ambiental-judicial-install` e `/ambiental-judicial-master` estão presentes. As skills orientam a triagem, a seleção de rota e a revisão R1→R4; sua presença e os gates estruturais não comprovam a execução de um caso real nem dispensam conferência jurídica humana.

## Recorte

O desenho cobre ACP e responsabilidade civil ambiental para ambos os lados, da triagem à prova, tutela, reparação e execução. Inclui agravo de instrumento contra liminar ou tutela interlocutória da ACP, apelação e respectivas contrarrazões, conforme a posição processual. Inclui também a ação judicial anulatória de auto de infração ambiental pelo autuado, sujeita às bases ainda pendentes.

Defesa e recurso administrativos, embargo administrativo, CAR/PRA, dimensionamento agrário especializado, licenciamento agropecuário e matéria penal ambiental ficam fora do recorte. Em conflito entre vias, separar o pedido judicial do procedimento administrativo; uma peça tem uma única rota de produção. A atuação para polos diferentes não autoriza representar interesses opostos no mesmo caso ou usar acervo adversário.

## Corpus e limites

`context/` contém cópia dos 15 textos normativos capturados, índice, manifesto e marcadores de conclusão da captura anterior. Os arquivos normativos foram copiados sem edição. O índice foi ajustado para descrever o pacote autônomo; scripts de captura, validação e estado de operador não foram incluídos. Cada fundamento futuro deve usar o texto literal local com localizador, alcance e versão; artigo sem texto fica **🟡 pendente** e não pode ser completado por memória. Não usar Jusbrasil ou Escavador. Súmula e tema ficam apenas como número e 🟡 até conferência oficial.

A base crítica da anulatória segue 🟡: Decreto 6.514/2008, Leis 9.873/1999 e 9.784/1999, regras processuais aplicáveis e normas do órgão do caso não estão neste corpus. A CF 5º XXXV/LIV/LV não basta para concluir nulidade, prazo ou suspensão da multa. Minuta dependente desses fundamentos permanece bloqueada. Vigência, remissões e alcance de precedentes também exigem conferência antes do uso.

As skills de mérito instruem o uso dos três controles locais: anti-alucinação, validador normativo e Suprema Corte R1→R4. Cada pasta de skill contém apenas `SKILL.md`; os comandos diretos também instruem os mesmos controles. O hook `SessionStart` apenas exibe uma mensagem; não executa validação jurídica.

Casos, documentos e dados de clientes devem ficar em pasta privada externa, separados por cliente e matéria, fora do source e do pacote distribuível. O plugin não pressupõe conector, pesquisa externa ou plugin irmão instalado.

Suporte: **luis@sbroggio.io**. Uso sujeito à [LICENCA](LICENCA).
