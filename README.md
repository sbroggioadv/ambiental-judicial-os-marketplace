# Ambiental Judicial OS — Marketplace

Apoio documental ao advogado de qualquer polo na ação civil pública ambiental, conforme legitimidade e representação comprovadas: réu, autor, associação ou atingido. Inclui agravo, apelação e anulatória judicial do auto de infração ambiental, com revisão humana.

## Qual plugin usar — confira antes de iniciar

| Situação | Primeiro destino |
| --- | --- |
| Imóvel **rural**, inclusive com auto de infração | `agrario-adv-os` primeiro; se houver **ação anulatória do auto rural**, a peça judicial segue ao `ambiental-judicial-os` após a triagem agrária. |
| TAC com **Ministério Público**, **inquérito civil** ou **ACP** | `ambiental-judicial-os`, inclusive quando o imóvel for rural, após a triagem inicial no `agrario-adv-os`. |
| TAC apenas com **órgão ambiental**, sem MP e sem ação | `ambiental-extrajudicial-os`, após a triagem inicial no `agrario-adv-os` se o imóvel for rural. |
| Anulatória de auto **não rural**, com defesa administrativa feita no `ambiental-extrajudicial-os` e **sem ação conexa** | `ambiental-extrajudicial-os` como continuidade. |
| Demais anulatórias judiciais de auto | `ambiental-judicial-os`; para imóvel rural, começar pela triagem do `agrario-adv-os`. |

Se faltar dado sobre imóvel, tomador do TAC, inquérito, ACP, defesa prévia ou ação conexa, registrar `PENDENTE DE ENQUADRAMENTO` e pedir os documentos antes de produzir peça. O encaminhamento não pressupõe outro plugin instalado.

## Instalação no Cowork

No Claude Desktop, abra a área de plugins do Cowork, escolha adicionar um marketplace e informe `https://github.com/sbroggioadv/ambiental-judicial-os-marketplace`. Instale **ambiental-judicial-os**, abra uma conversa e execute `/ambiental-judicial-install` para configurar; use `/ambiental-judicial-master` para conduzir o caso.

## Escopo e limites

O plugin oferece 29 skills e 19 comandos. O advogado confere a legitimidade, as provas, as fontes e os prazos antes do uso. A anulatória judicial do auto depende de bases normativas e documentos ainda pendentes no corpus; sem eles, a minuta fica bloqueada. O plugin não cobre defesa ou recurso administrativo, CAR/PRA ou matéria penal ambiental. Consulte o [README do plugin](ambiental-judicial-os/README.md).

## Licenças

O marketplace e o plugin seguem a licença comercial de uso em [LICENSE](LICENSE), reproduzida em [LICENCA](ambiental-judicial-os/LICENCA).
