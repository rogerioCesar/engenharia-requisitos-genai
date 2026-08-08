# Ambiguidades, inconsistências e lacunas

## Conflitos e ambiguidades identificados

| ID | Evidências em tensão | Análise | Esclarecimento necessário |
|---|---|---|---|
| DL-01 | Participante deseja cancelar sem contato; organizadores afirmam que nem todos os eventos permitem cancelamento. | Não é necessariamente contradição: pode haver política configurável por evento. Faltam parâmetros e comunicação da política. | Quem define a política, até quando é permitido cancelar e o que ocorre depois do prazo? |
| DL-02 | Eventos pagos exigem confirmação; não se sabe quando a vaga é reservada. | Sem uma regra atômica, podem ocorrer excesso de capacidade ou bloqueio prolongado de vagas. | A vaga é reservada ao iniciar pagamento? Por quanto tempo? O que ocorre em falha ou abandono? |
| DL-03 | Há reembolso em alguns casos e em outros não. | A regra está incompleta e pode afetar cancelamento, finanças e comunicação. | Quais eventos, prazos, percentuais, taxas, responsáveis e prazos de processamento se aplicam? |
| DL-04 | Desejo de múltiplos workshops no mesmo dia; atividades podem ser simultâneas; conflitos não foram tratados. | “Mesmo dia” não implica “mesmo horário”. É preciso decidir se o sistema bloqueia, alerta ou permite sobreposição. | Como considerar início, término, intervalos e atividades on-line? |
| DL-05 | Lista de espera desejada; funcionamento não definido. | Ordem e promoção interferem em capacidade, pagamento e notificações. | A ordem é cronológica? A promoção é automática? Há prazo para aceitar ou pagar? |
| DL-06 | Certificado desejado; emissão automática ou condicionada à presença não definida. | Emitir sem critério pode comprometer a validade do certificado. | Quem registra presença, qual frequência mínima e quem pode corrigir registros? |
| DL-07 | Comprovante deve ser recebido “logo após a inscrição”. | “Inscrição” pode significar solicitação, reserva, pagamento pendente ou confirmação. | Qual documento é emitido em cada estado e por qual canal? |
| DL-08 | Organizador quer dados em “tempo real”. | A expressão não possui tolerância mensurável. | Atualização deve ser instantânea, em segundos ou por atualização manual? |
| DL-09 | Palestrante quer lista de participantes; dados permitidos não foram definidos. | Exibir dados excessivos cria risco de privacidade e uso incompatível. | Quais campos, por quanto tempo e com possibilidade de exportação? |

## Perguntas priorizadas para os stakeholders

### Críticas — bloqueiam o núcleo da solução

1. **Organizadores e financeiro:** em evento pago, em que momento a vaga é ocupada e quanto tempo uma pendência de pagamento pode mantê-la reservada?
2. **Organizadores e financeiro:** quais combinações de prazo, motivo e tipo de evento permitem cancelamento e reembolso? O reembolso é integral ou parcial?
3. **Organizadores:** como funciona a lista de espera — entrada, ordenação, promoção, prazo de resposta, pagamento e expiração?
4. **Organizadores:** qual é o critério para emissão de certificado? Presença é obrigatória? Como é registrada e corrigida?
5. **Organizadores e participantes:** inscrições em atividades sobrepostas devem ser bloqueadas, apenas alertadas ou permitidas?

### Altas — afetam escopo, privacidade ou integrações

6. **Participantes e organizadores:** quais canais serão usados para comprovantes e notificações: área do usuário, e-mail, SMS ou aplicativo?
7. **Financeiro e TI:** o pagamento será confirmado manualmente, por importação ou por integração com provedor? Quais meios serão aceitos?
8. **Palestrantes e responsável por privacidade:** quais dados do participante podem ser vistos ou exportados, para qual finalidade e por quanto tempo?
9. **Organizadores:** capacidade e políticas pertencem ao evento inteiro ou podem variar por atividade?
10. **Organizadores:** é permitido alterar horário, capacidade ou política após existirem inscrições? Como os afetados serão tratados?
11. **Todos:** uma pessoa pode realizar inscrições duplicadas? Como identidade e acesso serão confirmados?

### Não funcionais — necessárias antes da aceitação

12. **TI e negócio:** quais volumes de pico, metas de resposta e atualização do painel são necessários?
13. **TI e negócio:** qual disponibilidade, janela de manutenção, RTO e RPO são aceitáveis?
14. **Responsável por privacidade:** quais dados serão coletados, por qual base legal, por quanto tempo e com quais compartilhamentos?
15. **TI e usuários:** quais requisitos de autenticação, auditoria e acessibilidade são obrigatórios?
16. **Equipe de suporte:** quais navegadores, dispositivos, idiomas e canais de atendimento devem ser suportados?

## Decisões a registrar após a validação

| Decisão | Responsáveis sugeridos | Artefatos a atualizar |
|---|---|---|
| Reserva e expiração de vaga | Organizadores, financeiro e TI | RN-05, UC-02/03, estados e tabelas |
| Cancelamento e reembolso | Organizadores e financeiro | RN-06/07, UC-04 e tabela TD-02 |
| Lista de espera | Organizadores | RN-08/10, UC-05 e estado da espera |
| Conflito de horários | Organizadores e participantes | RF-07/25 e tabela TD-04 |
| Certificação e presença | Organizadores e palestrantes | RF-22/23, UC-06 e tabela TD-03 |
| Visibilidade de dados | Palestrantes e responsável por privacidade | RF-21, UC-07 e RNF-06 |
| Notificações | Participantes, organizadores e TI | RF-24 e casos de uso relacionados |
| Metas de qualidade | Negócio e TI | RNFs e cenários de qualidade |
