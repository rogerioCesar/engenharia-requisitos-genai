# Requisitos funcionais

Os itens abaixo foram extraídos ou derivados do documento de elicitação. A coluna **Situação** distingue necessidades evidenciadas de funcionalidades derivadas ou propostas ainda dependentes de validação.

| ID | Requisito | Origem principal | Situação | Prioridade inicial |
|---|---|---|---|---|
| RF-01 | O sistema deve permitir que participantes visualizem, em um único local, os eventos disponíveis. | Participantes | Evidenciado | Alta |
| RF-02 | O sistema deve exibir os detalhes e a programação de cada evento e de suas atividades. | Participantes e palestrantes | Derivado | Alta |
| RF-03 | O sistema deve identificar participantes, organizadores, equipe financeira e palestrantes e aplicar permissões conforme o perfil. | Todos os stakeholders | Derivado | Alta |
| RF-04 | O sistema deve permitir ao organizador criar, editar, publicar e administrar eventos e suas atividades. | Organizadores | Derivado | Alta |
| RF-05 | O sistema deve permitir configurar capacidade, horários, gratuidade, exigência de pagamento e políticas aplicáveis a cada evento ou atividade. | Organizadores e equipe financeira | Derivado | Alta |
| RF-06 | O sistema deve permitir ao participante solicitar inscrição em eventos e atividades. | Participantes | Evidenciado | Alta |
| RF-07 | O sistema deve permitir a inscrição em mais de um workshop no mesmo dia, observadas as regras de conflito de horário ainda a definir. | Participantes e observações | Evidenciado, com decisão pendente | Média |
| RF-08 | O sistema deve controlar automaticamente as vagas e impedir que inscrições confirmadas ultrapassem a capacidade configurada. | Organizadores | Evidenciado | Alta |
| RF-09 | O sistema deve informar a disponibilidade de vagas durante a inscrição. | Organizadores | Derivado | Alta |
| RF-10 | Quando a capacidade for atingida, o sistema deve oferecer lista de espera conforme política ainda a definir. | Organizadores | Evidenciado, com decisão pendente | Alta |
| RF-11 | O sistema deve permitir ao participante consultar a situação de suas inscrições. | Participantes | Derivado | Alta |
| RF-12 | O sistema deve emitir e disponibilizar comprovante após a inscrição, definindo claramente se ela está solicitada, pendente ou confirmada. | Participantes | Evidenciado | Alta |
| RF-13 | O sistema deve permitir ao participante solicitar cancelamento quando a política do evento autorizar. | Participantes e organizadores | Evidenciado | Alta |
| RF-14 | O sistema deve registrar eventos gratuitos e pagos. | Equipe financeira | Evidenciado | Alta |
| RF-15 | O sistema deve registrar o pagamento e permitir que a equipe financeira o confirme quando necessário. | Equipe financeira | Evidenciado | Alta |
| RF-16 | O sistema deve condicionar a confirmação de determinadas inscrições à confirmação do pagamento. | Equipe financeira | Evidenciado | Alta |
| RF-17 | O sistema deve permitir registrar, aprovar e acompanhar reembolsos quando previstos pela política aplicável. | Equipe financeira | Evidenciado, com decisão pendente | Alta |
| RF-18 | O sistema deve apresentar aos organizadores a quantidade de inscritos e a ocupação das atividades em tempo real ou em intervalo a validar. | Organizadores | Evidenciado | Alta |
| RF-19 | O sistema deve permitir ao organizador consultar e gerenciar participantes e suas situações de inscrição. | Organizadores | Evidenciado | Alta |
| RF-20 | O sistema deve apresentar ao palestrante a programação de suas atividades. | Palestrantes | Evidenciado | Média |
| RF-21 | O sistema deve permitir ao palestrante consultar a lista de participantes de suas próprias atividades, limitada aos dados autorizados. | Palestrantes e observações | Evidenciado, com decisão pendente | Média |
| RF-22 | O sistema deve registrar a presença dos participantes caso esse registro seja adotado como condição de certificação. | Observações | Proposto | Alta |
| RF-23 | O sistema deve gerar e permitir a emissão de certificados após o evento, conforme critérios ainda a definir. | Participantes e observações | Evidenciado, com decisão pendente | Alta |
| RF-24 | O sistema deve enviar notificações e comprovantes por canais ainda a definir e manter uma cópia consultável pelo participante. | Participantes e observações | Proposto | Média |
| RF-25 | O sistema deve detectar tentativas de inscrição em atividades com horários conflitantes e aplicar a política que vier a ser aprovada. | Observações | Proposto | Alta |
| RF-26 | O sistema deve manter histórico auditável de alterações críticas em inscrição, pagamento, reembolso, presença e certificado. | Necessidade de controle | Derivado | Média |

## Dependências de decisão

- RF-07 e RF-25 dependem da política para conflitos de horário.
- RF-10 depende da ordem, do prazo e do mecanismo de promoção da lista de espera.
- RF-13 e RF-17 dependem das políticas de cancelamento e reembolso.
- RF-15 e RF-16 dependem do meio de pagamento e da regra de reserva de vaga.
- RF-21 depende da definição dos dados visíveis ao palestrante.
- RF-22 e RF-23 dependem do critério de presença e da forma de liberação do certificado.
- RF-24 depende dos canais de comunicação e das preferências de consentimento.
