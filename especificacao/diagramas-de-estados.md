# Diagramas de estados

Os diagramas mostram ciclos de vida candidatos. Estados e transições marcados como dependentes de política devem ser validados antes da implementação.

## Inscrição

```mermaid
stateDiagram-v2
    [*] --> Solicitada
    Solicitada --> PendentePagamento: evento pago
    Solicitada --> Confirmada: gratuita e com vaga
    Solicitada --> EmEspera: sem vaga
    PendentePagamento --> Confirmada: pagamento confirmado e vaga válida
    PendentePagamento --> Expirada: prazo encerrado
    Confirmada --> Cancelada: cancelamento autorizado
    Confirmada --> Concluida: evento encerrado
    EmEspera --> Confirmada: promoção aceita
    EmEspera --> Expirada: prazo ou lista encerrada
    Cancelada --> [*]
    Expirada --> [*]
    Concluida --> [*]
```

## Pagamento

```mermaid
stateDiagram-v2
    [*] --> Pendente
    Pendente --> Confirmado: confirmação válida
    Pendente --> Recusado: falha ou recusa
    Pendente --> Expirado: limite atingido
    Confirmado --> ReembolsoPendente: cancelamento elegível
    ReembolsoPendente --> Reembolsado: devolução concluída
    ReembolsoPendente --> FalhaReembolso: falha
    Recusado --> [*]
    Expirado --> [*]
    Reembolsado --> [*]
```

## Entrada na lista de espera

```mermaid
stateDiagram-v2
    [*] --> Aguardando
    Aguardando --> OfertaEnviada: vaga liberada
    OfertaEnviada --> Promovida: aceite e condições cumpridas
    OfertaEnviada --> Expirada: prazo encerrado
    OfertaEnviada --> Recusada: participante recusa
    Aguardando --> Cancelada: saída voluntária
    Promovida --> [*]
    Expirada --> [*]
    Recusada --> [*]
    Cancelada --> [*]
```

## Certificado

```mermaid
stateDiagram-v2
    [*] --> NaoElegivel
    NaoElegivel --> Elegivel: critérios satisfeitos
    Elegivel --> Emitido: geração concluída
    Emitido --> Revogado: correção ou invalidação
    Revogado --> Emitido: reemissão autorizada
    Emitido --> [*]
```

## Transições que exigem decisão

| Transição | Decisão necessária |
|---|---|
| Pendente de pagamento → Confirmada | Se a vaga permanece reservada e como tratar confirmação tardia. |
| Solicitada → Em espera | Se a entrada é automática ou depende de aceite. |
| Oferta enviada → Promovida | Prazo, pagamento e tratamento de conflitos. |
| Confirmada → Cancelada | Prazo e autoridade para exceções. |
| Confirmado → Reembolso pendente | Elegibilidade e cálculo do valor. |
| Não elegível → Elegível | Presença mínima e demais critérios de certificação. |
