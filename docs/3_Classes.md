# Modelagem de Entidades e Atributos (Dicionário de Dados)

### Entidades de Negócio

| Entidade | RF Relacionados | Atributos |
| :--- | :--- | :--- |
| **Aluno** | RF01, RF04, RF05, RF06, RF10 | `idAluno`, `nome`, `cpf`, `email`, `telefone`, `endereco`, `rfid`, `status` |
| **Plano** | RF01, RF02, RF04 | `idPlano`, `nome`, `tipo`, `valor`, `ativo` |
| **Pagamento** | RF03, RF04, RF09 | `idPagamento`, `data`, `valor`, `formaPagamento`, `status` |
| **Acesso** | RF05, RF09 | `idAcesso`, `dataHora`, `autorizado` |
| **Aula** | RF06, RF07, RF09 | `idAula`, `nome`, `horario`, `capacidadeMaxima` |
| **Agendamento** | RF06, RF10 | `idAgendamento`, `dataReserva`, `status` |
| **Presenca** | RF07 | `idPresenca`, `data`, `presente` |
| **AvaliacaoFisica** | RF08, RF10 | `idAvaliacao`, `data`, `peso`, `imc`, `percentualGordura`, `observacoes`, `anexo` |
| **Notificacao** | RF10 | `idNotificacao`, `tipo`, `dataEnvio`, `status`, `mensagem` |

---

### Atores do Sistema (Classes de Usuário)

| Classe | RF Relacionados | Atributos |
| :--- | :--- | :--- |
| **Instrutor** | RF07, RF08 | `idInstrutor`, `nome`, `especialidade` |
| **Recepcionista** | RF01, RF03 | `idRecepcionista`, `nome` |
| **Gerente** | RF02, RF09 | `idGerente`, `nome` |

---

> **Observação:** As chaves estrangeiras (FKs) para relacionamentos entre as tabelas (ex: `idAluno` em `Pagamento` ou `AvaliacaoFisica`) devem ser implementadas na fase de modelagem de banco de dados para garantir a integridade dos dados descritos nos Requisitos Funcionais.
