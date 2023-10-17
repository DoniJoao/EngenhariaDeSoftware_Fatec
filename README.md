# EngenhariaDeSoftwareII-2.2023-Prof_AnaCelia
Repositorio destinado a entrega das atividades desenvolvidas em sala de aula

``` mermaid
classDiagram
  class Usuario{
    - nome: String
    - endereço: String
    - numeroCell: int
    - chavePix: String
    + criarConta(): void
    + inserir(): void
    + alterar(): void
    + deletar(): void
    + encerrarConta(): void
  }

  class Entrega {
    - endereçoRetirada: String
    - horarioColeta: datetime
    - endereçoEntrega: String
    - tamanhoProduto: float
    - pesoProduto: float
    + solicitarEntrega(): void
    + inserir(): void
    + alterar(): void
    + deletar(): void
    + encerrarEntrega(): void
  }

  Usuario "1" -- "1..*" Entrega : tem

```
``` mermaid

graph TD
    subgraph RegistrarCliente
    A[Download do Aplicativo "RapidLogística"]
    B[Registro no Aplicativo]
    C[Fornecer Informações Pessoais]
    D[Fornecer Informações de Pagamento]
    end

    subgraph SolicitarServico
    E[Iniciar o Aplicativo]
    F[Selecionar "Solicitar Serviço"]
    G[Fornecer Detalhes da Entrega]
    end

    subgraph AlocarEntregador
    H[Usar Dados para Encontrar Entregador Disponível]
    I[Alocar Entregador]
    J[Enviar Detalhes para o Entregador]
    end

    subgraph CalcularValor
    K[Calcular Custo com Base em Distância, Tamanho e Peso]
    L[Revisar o Custo]
    end

    subgraph ConfirmarPagamento
    M[Confirmar Solicitação]
    N[Pagamento via Transferência Bancária (Pix)]
    end

    subgraph AcompanharTempoReal
    O[Acompanhar Entregador em Tempo Real]
    P[Visualizar no Mapa]
    Q[Estimativa de Tempo Restante]
    end

    subgraph NotificacaoConclusao
    R[Notificação de Conclusão]
    S[Classificar Entrega e Deixar Feedback]
    end

    subgraph HistoricoEntregas
    T[Manter Histórico de Entregas]
    U[Detalhes e Recibos das Entregas Anteriores]
    end
```
