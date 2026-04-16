# Especificação de Requisitos Funcionais

| ID | Título | Descrição |
|:--- |:--- |:--- |
| **RF01** | **Cadastro de Alunos** | O sistema deve permitir cadastrar novos _**alunos**_ contendo dados pessoais, contato, endereço e plano contratado. |
| **RF02** | **Gerenciamento de Planos** | O sistema deve permitir criar, editar, ativar e desativar tipos de _**planos**_ (mensal, trimestral, anual, musculação, funcional etc.). |
| **RF03** | **Controle de Pagamentos** | O sistema deve registrar _**pagamentos**_ realizados na recepção (dinheiro, cartão ou PIX) e gerar boletos/cartões para pagamentos online. |
| **RF04** | **Regularidade do Aluno** | O sistema deve verificar automaticamente se o aluno está com mensalidade em dia. |
| **RF05** | **Controle de Acesso** | O sistema deve se integrar à catraca para validar a entrada do aluno por RFID. |
| **RF06** | **Agendamento de _Aulas_** | O aluno deve poder visualizar horários e reservar vagas nas aulas disponíveis. |
| **RF07** | **Lista de Presença** | _**Instrutores**_ devem registrar _**presença**_ dos alunos nas aulas. |
| **RF08** | **Avaliação Física** | Instrutores devem registrar _**avaliações físicas**_ (peso, IMC, percentual de gordura etc.) e anexar arquivos se necessário. |
| **RF09** | **Relatórios Gerenciais** | O _**gerente**_ deve poder emitir relatórios de: inadimplência, alunos ativos, histórico de acessos e ocupação das aulas. |
| **RF10** | _**Notificações**_ | O sistema deve enviar notificações sobre: vencimento de mensalidade, confirmação de agendamento e liberação de nova avaliação. |

---

### Detalhamento dos Itens

#### Relatórios (RF09)
* **Inadimplência:** Listagem de alunos com mensalidades atrasadas.
* **Alunos Ativos:** Filtro por plano e período de vigência.
* **Histórico de Acessos:** Logs gerados pela integração com a catraca (RF05).
* **Ocupação das Aulas:** Relação entre vagas ofertadas e reservas feitas (RF06).

#### Notificações (RF10)
* **Vencimento:** Alerta enviado X dias antes do prazo.
* **Agendamento:** Confirmação imediata após a reserva da vaga.
* **Avaliação Física:** Aviso de que os resultados já estão disponíveis no perfil do aluno.
