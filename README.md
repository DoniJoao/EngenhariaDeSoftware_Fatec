# EngenhariaDeSoftwareII-2.2023-Prof_AnaCelia
Repositorio destinado a entrega das atividades desenvolvidas em sala de aula


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

