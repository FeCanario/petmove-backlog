# Checklist de aceite da Sprint Review

Responsável: Bruno Augusto (Product Owner)

Roteiro para o PO aceitar ou recusar cada história na Sprint Review. Os itens vêm dos critérios de aceite das issues e da Definition of Done do README. Os campos ficam em branco até a Review acontecer.

## Antes da Review

- [ ] A demonstração roda no protótipo
- [ ] O código de cada história foi revisado em pull request por outro Developer
- [ ] Os testes das funcionalidades estão passando
- [ ] Não há bugs críticos abertos

## Roteiro de demonstração das histórias Must

| Ordem | Issue | O que demonstrar | Aceita? | Observações |
|---|---|---|---|---|
| 1 | #1 | Criar conta e entrar logado; tentar e-mail inválido e e-mail repetido; errar a senha 3 vezes | | |
| 2 | #2 | Cadastrar dois pets; fechar e reabrir o app e conferir que continuam lá | | |
| 3 | #4 | Solicitar transporte; tentar horário no passado; ver o valor antes de confirmar; cancelar uma solicitação | | |
| 4 | #3 | Como condutor aprovado, aceitar uma solicitação; conferir que outro condutor não pode aceitá-la e que o tutor vê o nome de quem aceitou | | |
| 5 | #5 | Agendar passeio escolhendo a duração, depois que a história tiver critérios de aceite aprovados | | |

## Regra de aceite

- **Aceita:** todos os critérios da issue foram demonstrados no protótipo.
- **Recusada:** algum critério falhou ou não foi demonstrado. A história volta para o backlog com o motivo registrado na issue.
- Depois de aceita, a issue vai para **Concluído** no quadro.

## Indicadores do README a medir

- [ ] Um tutor novo cadastra um pet e solicita um transporte em menos de 3 minutos. Tempo medido: ____
- [ ] 100% das histórias Must foram aceitas. Resultado: ____ de 5
