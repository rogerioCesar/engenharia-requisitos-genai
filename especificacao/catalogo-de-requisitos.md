# Catálogo de requisitos e glossário

## Visão do produto

Centralizar o ciclo de gestão de eventos da Eventus — publicação, inscrição, capacidade, pagamento, cancelamento, espera, presença e certificação — reduzindo controles paralelos por formulários e planilhas e oferecendo informações consistentes a participantes, organizadores, equipe financeira e palestrantes.

## Escopo funcional inicial

| Épico | Capacidades relacionadas | Requisitos |
|---|---|---|
| Catálogo e programação | Listar eventos, consultar detalhes e programação | RF-01, RF-02 |
| Administração de eventos | Criar, configurar, publicar e acompanhar evento e atividades | RF-04, RF-05, RF-18, RF-19 |
| Inscrição e capacidade | Solicitar inscrição, controlar vagas, consultar situação, tratar conflitos | RF-06 a RF-13, RF-25 |
| Financeiro | Classificar gratuidade, confirmar pagamento e tratar reembolso | RF-14 a RF-17 |
| Palestrantes | Consultar programação e lista limitada de participantes | RF-20, RF-21 |
| Presença e certificado | Registrar presença e emitir certificado | RF-22, RF-23 |
| Comunicação e controle | Notificar e preservar trilha de alterações | RF-24, RF-26 |

O detalhamento e a situação de cada item estão em [`../analise/requisitos-funcionais.md`](../analise/requisitos-funcionais.md). As propostas de qualidade estão em [`../analise/requisitos-nao-funcionais.md`](../analise/requisitos-nao-funcionais.md).

## Atores

| Ator | Responsabilidade no sistema |
|---|---|
| Participante | Consultar oferta, solicitar e acompanhar inscrição, pagar, cancelar quando permitido e obter certificado. |
| Organizador | Configurar evento, programação, capacidade e políticas; acompanhar e administrar inscrições. |
| Equipe financeira | Confirmar pagamentos e controlar reembolsos. |
| Palestrante | Consultar suas atividades e informações autorizadas dos respectivos participantes. |
| Serviço de pagamento | Ator externo candidato para autorizar ou confirmar transações, caso haja integração. |
| Serviço de notificação | Ator externo candidato para entrega de e-mail, SMS ou outro canal aprovado. |

## Glossário

| Termo | Definição de trabalho |
|---|---|
| Evento | Congresso, workshop ou evento corporativo administrado pela Eventus. |
| Atividade | Unidade da programação de um evento, como palestra ou workshop, com horário, responsável e possivelmente capacidade próprios. |
| Solicitação de inscrição | Pedido do participante ainda sujeito a capacidade, pagamento ou outra validação. |
| Inscrição confirmada | Inscrição que cumpriu as condições vigentes e ocupa uma vaga. |
| Reserva de vaga | Bloqueio temporário candidato durante pagamento ou aceite; duração ainda não definida. |
| Lista de espera | Fila de interessados acionada quando não há vaga, segundo política ainda a aprovar. |
| Promoção | Oferta de uma vaga a uma pessoa da lista de espera. |
| Cancelamento | Encerramento da participação por solicitação autorizada ou por ação administrativa. |
| Reembolso | Devolução total ou parcial de valor segundo política aplicável. |
| Presença | Evidência de participação utilizada caso seja adotada como requisito de certificação. |
| Certificado | Documento emitido após o evento para participante que cumprir os critérios definidos. |
| Política do evento | Conjunto configurável de regras sobre inscrição, pagamento, cancelamento, reembolso, espera e certificação. |

## Fora do escopo confirmado nesta versão

Não há evidência suficiente para incluir hospedagem, transporte, submissão de trabalhos científicos, credenciamento físico, transmissão de vídeo, gestão de fornecedores, contabilidade completa, marketing ou rede social do evento.

## Critério de evolução da baseline

Um item proposto passa a aprovado apenas quando houver decisão registrada, responsável, regra verificável e atualização da matriz de rastreabilidade.
