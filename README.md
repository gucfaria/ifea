# IFE-A — Inventário de Funções Executivas no Adulto + escalas clínicas

Questionário clínico modular. O link define quais blocos o paciente responde.
© 2026 Gustavo Coutinho de Faria. Uso clínico.

## Blocos (`m=`)
| Código | Bloco | Itens | Período |
|---|---|---|---|
| `ife` | IFE-A (69 itens em 11 domínios, compensação, medicação, infrequência, impacto) | 82 | 4 semanas ou 6 meses (`p=6`) |
| `asrs` | ASRS-18 (versão brasileira, Mattos et al., 2006) | 18 | 6 meses |
| `phq` | PHQ-9 + pergunta de dificuldade funcional | 10 | 2 semanas |
| `gad` | GAD-7 | 7 | 2 semanas |
| `asrm` | ASRM (tradução livre, não validada) | 5 | 1 semana |
| `audc` | AUDIT-C (texto do SUPERA/SENAD) | 3 | 12 meses |

## Links
- Avaliação inicial completa: `https://gucfaria.github.io/ifea/?m=ife,asrs,phq,gad,asrm,audc`
- TDAH: `https://gucfaria.github.io/ifea/?m=ife,asrs`
- Seguimento curto: `https://gucfaria.github.io/ifea/?m=asrs,phq,gad`
- Informante (só IFE-A): `https://gucfaria.github.io/ifea/?f=i`
- Área do médico (gera os links): `https://gucfaria.github.io/ifea/#medico`

Sem `m=`, o questionário abre só com o IFE-A, então os links antigos continuam funcionando.

## Código
- **IFE3:** dígitos de base 6 agrupados em pares, num alfabeto de 36 símbolos. O código guarda formulário, período, relação do informante, a máscara dos blocos respondidos e as respostas, com dígito verificador. O tamanho varia com os blocos.
- **IFE1 e IFE2:** continuam sendo corrigidos.

## Segurança
Se o item 9 do PHQ-9 for maior que zero, a página mostra na hora a orientação de ajuda (CVV 188, SAMU 192), e o modo médico exibe um alerta.
