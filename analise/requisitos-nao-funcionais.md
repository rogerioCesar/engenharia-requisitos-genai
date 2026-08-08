# Requisitos não funcionais

O documento de elicitação informa expressamente que segurança, desempenho, disponibilidade, acessibilidade e privacidade não foram levantados. Portanto, todos os itens desta versão são **candidatos para negociação**, e não requisitos aprovados.

| ID | Atributo | Proposta verificável para validação | Situação |
|---|---|---|---|
| RNF-01 | Desempenho | Em condições de carga acordadas, 95% das consultas ao catálogo e painel devem responder em até 2 segundos e 95% das operações transacionais em até 3 segundos. | Proposto; carga ainda não estimada |
| RNF-02 | Concorrência | O sistema deve preservar a integridade da capacidade mesmo quando múltiplos participantes tentarem ocupar a última vaga simultaneamente. | Proposto |
| RNF-03 | Disponibilidade | O serviço deve alcançar disponibilidade mensal de 99,5%, excluídas janelas de manutenção previamente comunicadas. | Proposto; meta a negociar |
| RNF-04 | Segurança | Todo tráfego deve ser protegido por TLS; credenciais devem ser armazenadas por mecanismo de hash apropriado; sessões e tentativas de acesso devem ser protegidas contra ataques comuns. | Proposto |
| RNF-05 | Controle de acesso | O sistema deve aplicar controle de acesso por papéis e exigir autenticação reforçada para perfis privilegiados, conforme análise de risco. | Proposto |
| RNF-06 | Privacidade | O tratamento de dados deve observar finalidade, minimização, transparência, retenção definida e atendimento aos direitos dos titulares, em conformidade com a LGPD. | Proposto; bases legais e prazos a definir |
| RNF-07 | Acessibilidade | As interfaces devem buscar conformidade com WCAG 2.2 nível AA e ser testadas com teclado, leitor de tela, contraste e ampliação. | Proposto; nível a validar |
| RNF-08 | Compatibilidade e usabilidade | As funções essenciais devem operar em navegadores atuais e em telas móveis, sem exigir planilhas ou processos paralelos para tarefas rotineiras. | Proposto |
| RNF-09 | Escalabilidade | A solução deve suportar crescimento de eventos e acessos sem perda das metas acordadas; volume de referência e sazonalidade devem ser levantados. | Proposto |
| RNF-10 | Auditabilidade | Alterações críticas devem registrar autor, data, ação e resultado, com acesso restrito e período de retenção definido. | Proposto |
| RNF-11 | Recuperação | Backups e procedimentos de recuperação devem atender a RPO de 15 minutos e RTO de 2 horas. | Proposto; metas a negociar |
| RNF-12 | Observabilidade | A equipe de TI deve dispor de logs, métricas e alertas para falhas em inscrição, pagamento, notificação e emissão de certificados, sem expor dados pessoais indevidamente. | Proposto |

## Informações necessárias para fechar os RNFs

- Quantidade média e máxima de eventos, atividades, participantes e acessos simultâneos.
- Períodos de pico, especialmente abertura de inscrições e emissão de certificados.
- Horário de operação, tolerância a indisponibilidade e janelas de manutenção.
- Dados pessoais coletados, finalidades, bases legais, compartilhamentos e prazos de retenção.
- Requisitos legais, contratuais e internos de auditoria.
- Tecnologias assistivas e perfis de usuários a incluir nos testes.
- Riscos aceitáveis, autenticação exigida e necessidade de segregação de funções.
- Metas de recuperação, backup, suporte e monitoramento.

## Critério de aceitação desta etapa

Nenhum valor numérico acima deve ser incorporado ao contrato ou à implementação antes de ser validado pela Eventus e pela equipe de TI. Após a validação, cada item deve receber responsável, método de medição e ambiente de teste.
