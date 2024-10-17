# programacao-orientada-a-objeto-projeto-de-java

feito por: HILCCER ROCHA DE ARAUJO MELO

resumo:
ATENCAO: se so quiser saber sobre o que o codigo fara, olhe embaixo, que mostrara as classes usadas caso contrario o senhor queira saber sobre prossiga para a leitura

Neste projeto por ter feito sozinho acabei olhando ao redor em torno de cenarios parecidos, pois eu ja tinha o que foi pedido, e tambem sabia que deveria pegar algo diferente, o que levou a ser algo mais simples de se fazer os 3 primeiros menus, porem se dificulto, no momento que tinha que criar um do inicio,o que me levou a ir para varios cantinhos, um deles sendo o google, em que perguntei o que um restaurante fazia em eventos, sem sucesso pois no final so falou de eventos de promoção o mesmo foi com hospital. 
Isso levou eu a ser mais "criativo" por asim dizer no que eu poderia fazer para dar um diferencial, o que me fez ter a ideiua no final  de um evento beneficiente, que seria um menu que pegaria ambos os menus juntos, e como sera mostrado na apresentação, o codigo em si, abaixo tem exatamente o que cada menu tera que fazer, e os codigos usados... tenha em mente claro, que o codigo foi pego em boparte, de varios exemplos da enternet, e das minhas aulas privadas, que me ajudaram.





1. Sistema de Clínica Médica
Classe Paciente: Armazena informações sobre pacientes, como nome e CPF.
Classe Medico: Armazena informações sobre médicos, como nome, especialidade e disponibilidade. Permite alterar a disponibilidade do médico.
Classe Consulta: Representa uma consulta médica entre um paciente e um médico, armazenando a data da consulta. Ao criar uma consulta, o médico é marcado como indisponível.
Classe ClinicaMedica: Gerencia listas de pacientes, médicos e consultas, além de fornecer métodos para cadastrar médicos e buscar médicos disponíveis.



Classe Paciente:
Tokens: Paciente, nome, cpf, getNome(), getCpf()
Classe Medico:
Tokens: Medico, nome, especialidade, disponivel, isDisponivel(), setDisponivel(boolean), getNome(), getEspecialidade()
Classe Consulta:
Tokens: Consulta, paciente, medico, data, getPaciente(), getMedico(), getData(), medico.setDisponivel(false)
Classe ClinicaMedica:
Tokens: ClinicaMedica, medicos, pacientes, consultas, cadastrarMedico(), buscarMedicoDisponivel()



2. Sistema de Eventos

Classe Evento: Gerencia eventos, permitindo adicionar participantes e verificar a lotação com base nos ingressos vendidos.

Classe Evento:
Tokens: Evento, participantes, ingressos, verificarLotacao()




3. Sistema de Restaurante
Classe ItemDoPedido: Representa um prato do cardápio com nome e valor. Fornece detalhes do item.
Classe Pedido: Armazena uma lista de itens do pedido e calcula o valor total. Permite listar todos os itens e o total do pedido.
Classe SistemaDeRestaurante: Gerencia os pratos do cardápio e associa pedidos às mesas.


Classe ItemDoPedido:
Tokens: ItemDoPedido, nome, valor, getNome(), getValor(), detalhes()
Classe Pedido:
Tokens: Pedido, itens, adicionarItem(ItemDoPedido), calcularTotal(), listarItens(), itens.stream()
Classe SistemaDeRestaurante:
Tokens: SistemaDeRestaurante, pratos, pedidos, getItemDoCardapio(int)

4. Sistema de Evento Beneficente
Classe EventoBeneficente: Integra os três sistemas (Clínica Médica, Eventos, Restaurante). Gerencia a doação de marmitas, o médico presente e o prato escolhido para o evento, além de calcular o valor total da doação. Exibe os detalhes do evento.

Classe EventoBeneficente:
Tokens: EventoBeneficente, nome, quantidadeMarmitas, medicoPresente, pratoEscolhido, valorTotalDoacao, getNome(), getValor(), mostrarDetalhes()

5. Menu Principal
Main: Interface principal que conecta todos os sistemas, permitindo ao usuário escolher qual sistema acessar (Clínica Médica, Restaurante ou Evento Beneficente).
Método gerenciarEventoBeneficente: Gera um evento beneficente, solicitando ao usuário o nome do evento e a quantidade de marmitas. Escolhe um médico e um prato para o evento e exibe os detalhes.

Main:
Tokens: Main, menu principal, scanner, ClinicaMedica, SistemaDeRestaurante, gerenciarEventoBeneficente(), opcao, break, switch(opcao)
Método gerenciarEventoBeneficente:

Tokens: gerenciarEventoBeneficente, nomeEvento, quantidade, Medico, ItemDoPedido, EventoBeneficente, mostrarDetalhes()
