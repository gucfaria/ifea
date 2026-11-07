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
| `sub` | Rastreio de substâncias (pergunta 2 do ASSIST, mais vape, medicamentos para TDAH e para emagrecer sem receita) | 11 | 3 meses |
| `beh` | Comportamentos com perda de controle (triagem própria, não validada): apostas, jogos eletrônicos, redes sociais/internet, compras, compulsão alimentar, pornografia, outros comportamentos sexuais. Frequência + perda de controle + prejuízo | 21 | 3 meses |
| `x2` | Complemento para quem respondeu IFE2 (FLE7, PLA7, TEM7, MED1) | 4 | igual ao IFE |
| `x1` | Complemento para quem respondeu IFE1 (atenção sustentada, novos itens, compensação, medicação) | 16 | igual ao IFE |

## Links
- Avaliação inicial completa: `https://gucfaria.github.io/ifea/?m=ife,asrs,phq,gad,asrm,audc,sub,beh`
- Só comportamentos: `https://gucfaria.github.io/ifea/?m=beh`
- TDAH: `https://gucfaria.github.io/ifea/?m=ife,asrs`
- Seguimento curto: `https://gucfaria.github.io/ifea/?m=asrs,phq,gad`
- Complemento IFE2: `https://gucfaria.github.io/ifea/?m=x2`
- Complemento IFE1: `https://gucfaria.github.io/ifea/?m=x1`
- Informante (só IFE-A): `https://gucfaria.github.io/ifea/?f=i`
- Área do médico (gera os links): `https://gucfaria.github.io/ifea/#medico`

Sem `m=`, o questionário abre só com o IFE-A, então os links antigos continuam funcionando.

## Código
- **IFE4:** dígitos de base 6 agrupados em pares, num alfabeto de 36 símbolos. O código guarda formulário, período, relação do informante, a máscara de 10 posições dos blocos e as respostas, com dígito verificador. O tamanho varia com os blocos.
- **Bloco `beh`:** é o último do código e começa com 7 dígitos reservados para o aprofundamento por escalas (hoje sempre 0), para que essa extensão não exija um novo formato.
- **Complementos:** no modo médico, colar o código antigo (IFE1/IFE2) junto com o do complemento soma os dois numa correção completa.
- **IFE1, IFE2 e IFE3:** continuam sendo corrigidos.

## Segurança
Se o item 9 do PHQ-9 for maior que zero, a página mostra na hora a orientação de ajuda (CVV 188, SAMU 192), e o modo médico exibe um alerta.
