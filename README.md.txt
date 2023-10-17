classDiagram
  class Usuario{
    - nome: String
    - endereço: String
    - numeroCell: int
    - chavePix: String
    + criarConta: void
    + inserir(): void
    + alterar(): void
    + deletar(): void
    + encerrarConta: void
  }

  class Entrega {
    - endereçoRetirada: String
    - horarioColeta: datetime
    - endereçoEntrega: String
    - tamanhoProduto: float
    - pesoProduto: float
    + solicitarEntrega: void
    + inserir(): void
    + alterar(): void
    + deletar(): void
    + encerrarEntrega: void
  }

  Usuario "1" -- "1..*" Entrega : tem