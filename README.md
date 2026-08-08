# Engenharia de Requisitos com apoio de GenAI

## Sistema de Gestão de Eventos — Eventus

Este repositório reúne a análise e a especificação inicial dos requisitos do Sistema de Gestão de Eventos da empresa Eventus. O ponto de partida foi o documento de elicitação fornecido na atividade, com entrevistas de participantes, organizadores, equipe financeira e palestrantes.

> **Estado da especificação:** versão inicial para validação. Questões sobre pagamento, cancelamento, reembolso, lista de espera, certificados, notificações, conflitos de horário, acesso de palestrantes e atributos de qualidade ainda precisam ser decididas com os stakeholders.

## Estrutura

```text
.
├── README.md
├── analise/
│   ├── requisitos-funcionais.md
│   ├── requisitos-nao-funcionais.md
│   ├── regras-de-negocio.md
│   └── duvidas-e-lacunas.md
└── especificacao/
    ├── catalogo-de-requisitos.md
    ├── casos-de-uso.md
    ├── modelo-conceitual-de-dominio.md
    ├── diagramas-de-estados.md
    ├── tabelas-de-decisao.md
    ├── cenarios-de-atributos-de-qualidade.md
    ├── prototipos-de-baixa-fidelidade.md
    └── matriz-de-rastreabilidade.md
```

## Ferramenta de GenAI utilizada

Foi utilizado o **ChatGPT, por meio do Codex da OpenAI**, como ferramenta de apoio. A decisão final sobre a classificação dos requisitos, o grau de certeza de cada item e a seleção dos artefatos permaneceu sob responsabilidade humana.

## Como a IA apoiou a atividade

1. Organizou as falas dos stakeholders e as observações do documento de elicitação.
2. Propôs uma classificação inicial em requisitos funcionais, requisitos não funcionais, regras de negócio e lacunas.
3. Detectou conflitos e decisões ainda não tomadas, evitando transformar suposições em requisitos aprovados.
4. Sugeriu artefatos de especificação compatíveis com um sistema orientado por fluxos, estados e políticas configuráveis.
5. Gerou versões iniciais dos artefatos, posteriormente revisadas quanto à coerência, rastreabilidade, redundância e nível de detalhe.

## Critério de certeza adotado

| Classificação | Significado |
|---|---|
| Evidenciado | Decorre diretamente das entrevistas ou do contexto fornecido. |
| Derivado | Necessário para viabilizar ou administrar uma necessidade evidenciada, mas não foi declarado literalmente. |
| Proposto | Sugestão de especificação que exige validação dos stakeholders. |

## Sugestões de artefatos apresentadas pela IA

A IA sugeriu: histórias de usuário com critérios de aceitação, catálogo de requisitos e glossário, casos de uso, modelo conceitual de domínio, diagramas de estados, tabelas de decisão, cenários de atributos de qualidade, protótipos, matriz de rastreabilidade, BPMN, modelo lógico de dados, contrato de API e uma especificação SRS monolítica.

## Análise crítica e artefatos selecionados

| Artefato selecionado | Justificativa |
|---|---|
| Catálogo de requisitos e glossário | Cria vocabulário comum, registra prioridade, origem e grau de certeza e reduz interpretações diferentes. |
| Casos de uso textuais e visão de atores | Representam as interações dos quatro perfis principais e deixam explícitos fluxos alternativos e pontos pendentes. |
| Modelo conceitual de domínio | Esclarece relações entre evento, atividade, inscrição, pagamento, lista de espera, presença e certificado sem antecipar o banco de dados. |
| Diagramas de estados | São adequados porque inscrição, pagamento, espera, cancelamento e certificado mudam de estado ao longo do tempo. |
| Tabelas de decisão | Tornam auditáveis as combinações de capacidade, pagamento, cancelamento, reembolso e presença. |
| Cenários de atributos de qualidade | Convertem temas vagos como segurança, desempenho e disponibilidade em propostas mensuráveis para negociação. |
| Protótipos de baixa fidelidade | Permitem validar navegação, informações e permissões antes de investir em design visual e implementação. |
| Matriz de rastreabilidade | Relaciona falas e lacunas da elicitação aos requisitos e casos de uso, apoiando validação e controle de mudanças. |

Esses artefatos foram escolhidos porque se complementam: o catálogo define **o que** é necessário; os casos de uso mostram **como os atores interagem**; os modelos de domínio e de estados explicam **conceitos e ciclos de vida**; as tabelas registram **decisões condicionais**; os cenários tratam **qualidade**; os protótipos permitem **validar a experiência**; e a matriz demonstra **a origem de cada requisito**.

## Sugestões descartadas ou modificadas

| Sugestão | Decisão e justificativa |
|---|---|
| Histórias de usuário como artefato principal | Incorporadas apenas como perspectiva de necessidade no catálogo. Isoladamente, seriam insuficientes para representar regras financeiras, estados e permissões entre vários perfis. |
| BPMN detalhado | Adiado. Os processos de pagamento, cancelamento, reembolso e lista de espera ainda não possuem decisões suficientes para um fluxo estável. |
| Modelo lógico de dados | Adiado por pertencer à etapa de projeto. Nesta fase, o modelo conceitual é suficiente e evita definir tabelas prematuramente. |
| Contrato de API | Descartado nesta etapa, pois depende de decisões arquiteturais e de integrações de pagamento/notificação ainda não levantadas. |
| Protótipo de alta fidelidade | Reduzido para baixa fidelidade, adequado para validar conteúdo e fluxo antes da identidade visual. |
| Documento SRS único | Substituído por arquivos Markdown modulares, mais fáceis de revisar, versionar e rastrear no GitHub. |

## Premissas e limites

- O material de elicitação é a única fonte de requisitos desta versão.
- Valores numéricos de desempenho, disponibilidade, recuperação e retenção são propostas de negociação, não acordos já aprovados.
- O sistema deverá tratar políticas configuráveis por evento, mas os limites e responsáveis por essas configurações precisam ser confirmados.
- Nenhum ponto listado em `analise/duvidas-e-lacunas.md` deve ser implementado sem validação ou decisão formal.

## Próximos passos recomendados

1. Realizar uma sessão de validação conjunta com representantes dos quatro grupos de stakeholders.
2. Resolver primeiro as questões marcadas como críticas em `analise/duvidas-e-lacunas.md`.
3. Atualizar tabelas de decisão e diagramas de estados com as decisões aprovadas.
4. Transformar propostas aceitas em requisitos verificáveis e critérios de aceitação.
5. Registrar mudanças na matriz de rastreabilidade.
