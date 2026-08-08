# Cenários de atributos de qualidade

Cada cenário usa a estrutura: fonte, estímulo, ambiente, artefato, resposta e medida. Os valores são propostas de negociação.

## CQ-01 — Concorrência pela última vaga

| Elemento | Descrição |
|---|---|
| Fonte | Múltiplos participantes |
| Estímulo | Tentativas simultâneas de confirmar a última vaga |
| Ambiente | Pico de abertura de inscrições |
| Artefato | Serviço de inscrição e controle de capacidade |
| Resposta | Serializar ou coordenar a alocação e rejeitar/promover excedentes de forma coerente |
| Medida proposta | Nenhum excesso de capacidade; todas as tentativas recebem situação inequívoca e auditável |

## CQ-02 — Tempo de resposta

| Elemento | Descrição |
|---|---|
| Fonte | Participante ou organizador |
| Estímulo | Consulta catálogo, evento ou painel |
| Ambiente | Carga normal e pico acordado |
| Artefato | Aplicação web e serviços |
| Resposta | Processar e apresentar dados atualizados |
| Medida proposta | 95% das consultas em até 2 s; transações em até 3 s |

## CQ-03 — Disponibilidade

| Elemento | Descrição |
|---|---|
| Fonte | Falha de componente |
| Estímulo | Interrupção inesperada durante período de inscrição |
| Ambiente | Produção |
| Artefato | Plataforma de eventos |
| Resposta | Detectar falha, alertar suporte e restaurar serviço preservando transações confirmadas |
| Medida proposta | 99,5% ao mês; RTO 2 h; RPO 15 min |

## CQ-04 — Acesso indevido a dados

| Elemento | Descrição |
|---|---|
| Fonte | Usuário autenticado sem autorização |
| Estímulo | Tentativa de acessar participantes de atividade alheia |
| Ambiente | Produção |
| Artefato | Controle de acesso e consulta de participantes |
| Resposta | Negar acesso, não revelar dados e registrar tentativa conforme política |
| Medida proposta | 100% dos testes negativos bloqueados; evento de segurança auditável |

## CQ-05 — Privacidade por minimização

| Elemento | Descrição |
|---|---|
| Fonte | Palestrante autorizado |
| Estímulo | Consulta à lista de sua atividade |
| Ambiente | Produção |
| Artefato | Tela ou exportação de participantes |
| Resposta | Exibir somente campos aprovados para a finalidade e período válidos |
| Medida proposta | Nenhum campo fora da matriz de permissão; acesso expira no prazo definido |

## CQ-06 — Acessibilidade

| Elemento | Descrição |
|---|---|
| Fonte | Pessoa que utiliza teclado ou leitor de tela |
| Estímulo | Executar consulta, inscrição, cancelamento e emissão de certificado |
| Ambiente | Navegador suportado |
| Artefato | Interface web |
| Resposta | Permitir concluir o fluxo com foco visível, rótulos e mensagens compreensíveis |
| Medida proposta | Conformidade WCAG 2.2 AA nos fluxos críticos e sucesso nos testes assistivos definidos |

## CQ-07 — Falha de notificação

| Elemento | Descrição |
|---|---|
| Fonte | Serviço externo de notificação |
| Estímulo | Falha ou atraso na entrega de comprovante |
| Ambiente | Produção |
| Artefato | Módulo de comunicação |
| Resposta | Registrar falha, repetir conforme política e manter comprovante consultável na área do usuário |
| Medida proposta | Nenhuma perda silenciosa; alerta após tentativas definidas; histórico consultável |

## CQ-08 — Auditabilidade financeira

| Elemento | Descrição |
|---|---|
| Fonte | Equipe financeira ou integração |
| Estímulo | Confirmação, estorno ou reembolso |
| Ambiente | Produção |
| Artefato | Pagamento, reembolso e inscrição |
| Resposta | Registrar identidade/origem, data, valor, estado anterior e novo estado |
| Medida proposta | 100% das mudanças críticas rastreáveis e conciliáveis |

## Validação necessária

Negócio e TI devem revisar volumes, percentis, disponibilidade, recuperação, navegadores, tecnologias assistivas, retenção de logs e tolerância a falhas antes de aprovar estes cenários.
