# Refinamento das histórias sem critérios de aceite

Responsável: Bruno Augusto (Product Owner)

**Status: proposta.** Pela matriz RACI, os critérios de aceite são escritos pelos Developers e aprovados pelo PO. Este texto serve de ponto de partida para validar com Fernando e Gabriel antes de passar para as issues.

As histórias partem das notas de refinamento de cada issue. Os itens marcados com *(a validar)* são sugestões novas que não estão nessas notas.

## #5: Agendar passeio (Must)

- [ ] O tutor escolhe um pet já cadastrado
- [ ] A duração pode ser de 30, 45 ou 60 minutos
- [ ] O ponto de encontro é o endereço do tutor
- [ ] Não é possível escolher data e horário no passado
- [ ] O app mostra um valor estimado antes de confirmar *(a validar)*
- [ ] Após confirmar, a solicitação aparece com status "Aguardando condutor"

**Dado** que sou um tutor logado com um pet cadastrado
**Quando** escolho o pet, a duração de 30 minutos e um horário futuro e confirmo
**Então** vejo a solicitação de passeio com status "Aguardando condutor"

## #6: Cadastro do condutor com documentos (Should)

- [ ] O condutor envia foto do RG ou da CNH e do comprovante de residência
- [ ] Para prestar transporte, a CNH e os dados do veículo são obrigatórios
- [ ] Não é possível concluir o cadastro sem os documentos obrigatórios *(a validar)*
- [ ] Após o envio, o status do cadastro fica "Em análise"

**Dado** que sou um condutor sem cadastro
**Quando** envio os documentos obrigatórios
**Então** meu cadastro fica com status "Em análise"

## #7: Aprovar credenciamento (Should)

- [ ] O administrador vê os cadastros com status "Em análise" *(a validar)*
- [ ] O administrador pode aprovar ou reprovar cada cadastro
- [ ] A reprovação exige um motivo, e o condutor consegue vê-lo
- [ ] O condutor reprovado pode reenviar os documentos
- [ ] Só o condutor aprovado passa a ver as solicitações (ver #3)

**Dado** que existe um condutor com status "Em análise"
**Quando** o administrador reprova o cadastro informando um motivo
**Então** o condutor vê o motivo e pode reenviar os documentos

## #8: Acompanhar status do serviço (Should)

- [ ] O status segue a sequência: Aguardando condutor → Condutor a caminho → Em andamento → Concluído
- [ ] O condutor atualiza o status manualmente
- [ ] O tutor vê o status atual na tela do serviço
- [ ] Não há rastreamento por GPS, que está fora de escopo

**Dado** que um condutor aceitou meu serviço
**Quando** ele marca o serviço como "Em andamento"
**Então** vejo o novo status na tela do serviço

## #9: Histórico de serviços (Could)

- [ ] A lista vai do serviço mais recente para o mais antigo
- [ ] Cada item mostra data, tipo e valor *(a validar)*
- [ ] O tutor pode filtrar por transporte ou passeio

**Dado** que contratei um transporte e um passeio
**Quando** filtro o histórico por passeio
**Então** vejo apenas o passeio

## #10: Avaliar condutor (Could)

- [ ] A nota vai de 1 a 5 estrelas, com comentário opcional
- [ ] Só é possível avaliar serviços concluídos
- [ ] Cada serviço pode ser avaliado uma única vez

**Dado** que tenho um serviço concluído e ainda não avaliado
**Quando** dou nota 5 e confirmo
**Então** a avaliação fica registrada e não posso avaliar esse serviço de novo
