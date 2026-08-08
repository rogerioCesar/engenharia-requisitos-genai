# Matriz de rastreabilidade

## Fontes da elicitação

| Código | Fonte resumida |
|---|---|
| PAR-01 | Visualizar todos os eventos em um único lugar. |
| PAR-02 | Receber comprovante logo após a inscrição. |
| PAR-03 | Cancelar sem contato com a organização. |
| PAR-04 | Emitir certificado depois do evento. |
| PAR-05 | Inscrever-se em vários workshops no mesmo dia. |
| ORG-01 | Controlar automaticamente o número de vagas. |
| ORG-02 | Criar lista de espera quando lotar. |
| ORG-03 | Nem todos os eventos permitem cancelamento. |
| ORG-04 | Acompanhar inscritos em tempo real. |
| ORG-05 | Workshops no mesmo horário podem ocorrer simultaneamente. |
| FIN-01 | Existem eventos gratuitos e pagos. |
| FIN-02 | Reembolso existe apenas em alguns casos. |
| FIN-03 | Algumas inscrições dependem da confirmação do pagamento. |
| PAL-01 | Consultar lista de participantes das próprias atividades. |
| OBS-01 | Prazo de cancelamento não definido. |
| OBS-02 | Critérios de reembolso não definidos. |
| OBS-03 | Funcionamento da lista de espera não definido. |
| OBS-04 | Emissão de certificado e presença não definidas. |
| OBS-05 | Canais de comprovante/notificação não definidos. |
| OBS-06 | Momento de reserva da vaga não definido. |
| OBS-07 | Conflitos de horário não definidos. |
| OBS-08 | Dados visíveis ao palestrante não definidos. |
| OBS-09 | Atributos de qualidade não levantados. |

## Rastreabilidade das necessidades

| Fonte | Requisitos/regras relacionados | Casos de uso | Outros artefatos |
|---|---|---|---|
| PAR-01 | RF-01, RF-02 | UC-02 | P-01, P-02 |
| PAR-02 | RF-12, RN-17 | UC-02 | P-03 |
| PAR-03 + ORG-03 + OBS-01 | RF-13, RN-06 | UC-04 | DL-01, TD-02, estado da inscrição, P-04 |
| PAR-04 + OBS-04 | RF-22, RF-23, RN-15, RN-16 | UC-06 | TD-03, estado do certificado, P-04 |
| PAR-05 + ORG-05 + OBS-07 | RF-07, RF-25, RN-11, RN-12 | UC-02 | DL-04, TD-04, P-02 |
| ORG-01 | RF-08, RF-09, RN-01, RN-02 | UC-01, UC-02 | TD-01, CQ-01, P-05 |
| ORG-02 + OBS-03 | RF-10, RN-08 a RN-10 | UC-05 | DL-05, TD-05, estado da espera |
| ORG-04 | RF-18 | UC-01 | DL-08, CQ-02, P-05 |
| FIN-01 | RF-14 | UC-01, UC-02 | TD-01, P-03 |
| FIN-02 + OBS-02 | RF-17, RN-07 | UC-04 | DL-03, TD-02, estado do pagamento, P-06 |
| FIN-03 + OBS-06 | RF-15, RF-16, RN-04, RN-05 | UC-02, UC-03 | DL-02, TD-01, estados, P-03/P-06 |
| PAL-01 + OBS-08 | RF-20, RF-21, RN-13, RN-14 | UC-07 | DL-09, CQ-04/CQ-05, P-07 |
| OBS-05 | RF-24 | UC-02 a UC-06 | CQ-07, P-03/P-04 |
| OBS-09 | RNF-01 a RNF-12 | Todos | CQ-01 a CQ-08 |

## Cobertura de casos de uso por requisito funcional

| Caso de uso | Requisitos cobertos |
|---|---|
| UC-01 | RF-03 a RF-05, RF-18, RF-19 |
| UC-02 | RF-01, RF-02, RF-06 a RF-14, RF-25 |
| UC-03 | RF-15, RF-16, RF-24, RF-26 |
| UC-04 | RF-13, RF-17, RF-24, RF-26 |
| UC-05 | RF-10, RF-11, RF-24, RF-25 |
| UC-06 | RF-22, RF-23, RF-24, RF-26 |
| UC-07 | RF-20, RF-21, RF-26 |

## Controle de mudanças

Após cada sessão de validação, registrar: decisão, stakeholder responsável, data, itens alterados e impacto nos casos de uso, estados, tabelas, cenários e protótipos. Requisitos sem fonte ou decisão não devem ser promovidos à baseline aprovada.
