# Ordenação do Product Backlog

Responsável: Bruno Augusto (Product Owner)

Este documento explica a ordem do backlog no quadro do projeto. Os pontos em aberto, no fim, ainda precisam de decisão da equipe.

## Critérios de ordenação

1. **Valor para o tutor:** primeiro o que permite contratar um serviço do início ao fim.
2. **Dependência:** uma história vem depois das histórias de que precisa para funcionar.
3. **Risco de escopo:** o que pode ficar fora do protótipo sem quebrar o fluxo principal vai para o fim.

## Ordem atual

| Ordem | Issue | História | Prioridade | Por que está nesta posição |
|---|---|---|---|---|
| 1 | #1 | Criar conta do tutor | Must | Todas as ações do tutor dependem de login |
| 2 | #2 | Cadastrar pets | Must | Não é possível solicitar serviço sem pet |
| 3 | #4 | Solicitar transporte | Must | É a principal proposta de valor do produto |
| 4 | #3 | Ver e aceitar solicitações | Must | Só faz sentido quando já existem solicitações |
| 5 | #5 | Agendar passeio | Must | Reaproveita o fluxo de aceite de #3 |
| 6 | #6 | Cadastro do condutor com documentos | Should | Base do diferencial de condutor credenciado |
| 7 | #7 | Aprovar credenciamento | Should | Depende dos cadastros de #6 |
| 8 | #8 | Acompanhar status do serviço | Should | Dá segurança ao tutor durante o serviço |
| 9 | #9 | Histórico de serviços | Could | Consulta útil, mas fora do fluxo principal |
| 10 | #10 | Avaliar condutor | Could | Depende de serviços concluídos e pode ficar para depois |

## Pontos em aberto

**1. Dependência entre Must e Should.** O critério de #3 diz que só condutores aprovados veem as solicitações, mas a aprovação está em #7 (Should). Proposta: na sprint das histórias Must, usar um condutor aprovado nos dados de demonstração, e deixar o fluxo real para #6 e #7.

**2. #5 sem detalhamento.** É Must, mas não tem estimativa nem critérios de aceite. Precisa ser refinada e estimada antes de entrar em uma sprint. Há uma proposta em [refinamento-das-historias.md](refinamento-das-historias.md).

**3. Estimativas diferentes entre README e issues.** O README agrupa as histórias e as issues têm pontos próprios, então os números não batem:

| README | Pontos no README | Issues | Pontos nas issues |
|---|---|---|---|
| Cadastro e login do tutor com seus pets | 5 | #1 e #2 | 3 + 2 = 5 |
| Solicitação de transporte e de passeio | 5 | #4 e #5 | 5 + sem estimativa |
| Aceite e execução do serviço pelo condutor | 3 | #3 | 5 |

Proposta: tratar as issues como fonte oficial e atualizar o README depois de reestimar #5.

**4. Prioridade de #8.** No README, marcar o serviço como iniciado e concluído e mostrar o status ao tutor fazem parte de uma funcionalidade Must, mas a issue #8 é Should. A equipe precisa definir se ao menos essa parte sobe para Must.

**5. Prioridade de #9.** O README coloca o histórico como Should e a issue #9 como Could. Proposta: manter Could, porque o histórico não impede a contratação de um serviço.

**6. Texto do benefício de #8.** A história promete "saber onde está meu pet", mas o rastreamento por GPS está fora de escopo. Proposta: trocar para "saber em que etapa está o serviço do meu pet".
