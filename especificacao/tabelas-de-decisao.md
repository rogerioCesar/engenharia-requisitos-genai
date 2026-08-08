# Tabelas de decisão

As tabelas abaixo são modelos para validação. O símbolo **?** indica resultado que não pode ser decidido com a elicitação disponível.

## TD-01 — Confirmação da inscrição

| Condição/ação | R1 | R2 | R3 | R4 | R5 |
|---|---:|---:|---:|---:|---:|
| Há vaga? | Sim | Sim | Sim | Não | Não |
| Evento pago? | Não | Sim | Sim | Não | Sim |
| Pagamento confirmado? | — | Sim | Não | — | — |
| Confirmar inscrição | Sim | Sim | Não | Não | Não |
| Manter pendente/reservar vaga | Não | Não | **?** | Não | **?** |
| Oferecer lista de espera | Não | Não | Não | Sim* | Sim* |

\* Somente se a lista estiver habilitada. A reserva em R3 e o fluxo financeiro em R5 dependem de decisão.

## TD-02 — Cancelamento e reembolso

| Condição/ação | R1 | R2 | R3 | R4 |
|---|---:|---:|---:|---:|
| Política permite cancelamento? | Sim | Sim | Não | Não |
| Houve pagamento? | Não | Sim | Não | Sim |
| Dentro do prazo de reembolso? | — | Sim | — | — |
| Cancelar automaticamente | Sim | Sim | **?** | **?** |
| Gerar reembolso | Não | Sim* | Não | Não |
| Encaminhar para análise | Não | Possível | **?** | **?** |

\* O valor integral ou parcial ainda precisa ser definido.

## TD-03 — Emissão de certificado

| Condição/ação | R1 | R2 | R3 | R4 |
|---|---:|---:|---:|---:|
| Evento encerrado? | Não | Sim | Sim | Sim |
| Inscrição elegível? | — | Sim | Sim | Não |
| Presença é exigida? | — | Não | Sim | — |
| Frequência mínima atingida? | — | — | Sim | — |
| Emitir certificado | Não | Sim | Sim | Não |

O conceito de “inscrição elegível” e a frequência mínima permanecem pendentes.

## TD-04 — Conflito de horário

| Situação | Política A: bloquear | Política B: alertar | Política C: permitir |
|---|---|---|---|
| Atividades sem sobreposição | Permitir | Permitir | Permitir |
| Sobreposição parcial ou total | Impedir e explicar | Solicitar confirmação | Permitir e registrar |
| Alteração posterior cria conflito | Exigir ajuste | Notificar e solicitar decisão | Notificar |

Uma única política, ou políticas por tipo de atividade, deve ser escolhida pelos stakeholders.

## TD-05 — Promoção da lista de espera

| Condição/ação | R1 | R2 | R3 | R4 |
|---|---:|---:|---:|---:|
| Vaga liberada? | Sim | Sim | Sim | Não |
| Existe pessoa elegível aguardando? | Sim | Sim | Não | — |
| Conflito de horário? | Não | Sim | — | — |
| Oferecer vaga | Sim | **?** | Não | Não |
| Avançar para próximo candidato | Após recusa/expiração | **?** | Não | Não |

Elegibilidade, conflito e quantidade de ofertas simultâneas ainda precisam de decisão.
