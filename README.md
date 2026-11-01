# PetMove

Aplicativo de transporte e passeio de pets que conecta tutores a condutores credenciados.

Engenharia de Software II • Senac • Prof. Rafael

## Elevator pitch

Para **tutores de pets** que precisam levar o animal ao veterinário, ao banho e tosa ou passear e não têm tempo ou carro, o **PetMove** é um **aplicativo de mobilidade pet** que **agenda transporte e passeio com condutores credenciados em poucos toques**. Diferente de **combinar por WhatsApp com conhecidos ou usar apps de corrida que recusam animais**, o nosso diferencial é que **todo condutor passa por credenciamento com documentos e o serviço é pensado para o pet**.

## Problema

Tutores têm dificuldade para transportar pets: apps de corrida comuns muitas vezes recusam animais, táxis cobram taxa extra e não há garantia de que o motorista sabe lidar com o pet. Para passeios, o tutor depende de indicações informais, sem saber quem é a pessoa nem acompanhar o serviço. A dor é de quem trabalha fora, não tem carro ou tem pet idoso/doente.

## Público (papéis de usuário)

| Papel | Quem é |
|---|---|
| **Tutor** | Dono do pet; cadastra os animais e solicita transporte ou passeio |
| **Condutor** | Prestador credenciado; aceita e executa transportes e passeios |
| **Administrador** | Equipe PetMove; aprova o credenciamento dos condutores |

## Proposta de valor

O tutor resolve o deslocamento ou o passeio do pet pelo celular, com um condutor verificado, sem precisar negociar caso a caso.

## Funcionalidades essenciais (Must)

1. Cadastro e login do tutor com seus pets
2. Solicitação de **transporte** e de **passeio** pelo tutor
3. Aceite e execução do serviço pelo condutor

## Fora de escopo (Won't, neste semestre)

- Pagamento real dentro do app (cartão, Pix) — o valor é só exibido
- Rastreamento GPS em tempo real com mapa
- Backend em nuvem — o protótipo usa persistência local no dispositivo
- Chat entre tutor e condutor
- Publicação nas lojas (App Store / Play Store)

## Indicadores de sucesso

- Um tutor novo consegue cadastrar um pet e solicitar um transporte em **menos de 3 minutos** no protótipo
- **100%** das histórias Must aceitas na Sprint Review com critérios de aceite cumpridos

## Equipe

| Integrante | Papel Scrum |
|---|---|
| Bruno Augusto | Product Owner |
| Fernando Canario | Scrum Master e Developer |
| Gabriel Frigo | Developer |

## Matriz RACI

R = Responsável · A = Aprovador · C = Consultado · I = Informado

| Atividade | Product Owner (Bruno) | Scrum Master (Fernando) | Developers (Fernando, Gabriel) | Professor |
|---|---|---|---|---|
| Definir visão e objetivo do produto | A / R | C | C | I |
| Escrever e ordenar o Product Backlog | A / R | C | C | I |
| Escrever critérios de aceite | A | I | R | I |
| Estimar itens (Planning Poker) | C | R (facilita) | A / R | I |
| Definir o escopo da sprint | C | C | A / R | I |
| Implementar e testar | I | I | A / R | I |
| Revisar pull requests | I | I | A / R | C |
| Aceitar o incremento na Review | A | I | R | C |
| Avaliar a entrega (nota A2/A3) | I | I | I | A / R |

Como a equipe tem três pessoas, o Scrum Master também atua como Developer. Ele facilita o Planning Poker, mas vota como Developer.

## Definition of Done

- Critérios de aceite da história cumpridos e demonstráveis no protótipo
- Código revisado em pull request por outro Developer
- Testes da funcionalidade passando
- Sem bugs críticos abertos
- Issue movida para **Concluído** no quadro

## Backlog e quadro

- Histórias: aba **Issues** (label `tipo:história`)
- Prioridade: labels `prioridade:must`, `prioridade:should`, `prioridade:could`
- Estimativa: labels `pontos:N` (Planning Poker, escala de Fibonacci modificada)
- Quadro **Projects**: Backlog → Pronto para sprint → Em andamento → Em revisão → Concluído

Protótipo: [FeCanario/petmove](https://github.com/FeCanario/petmove) (web app com persistência local).
