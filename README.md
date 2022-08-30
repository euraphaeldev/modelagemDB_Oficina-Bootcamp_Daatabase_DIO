# ModelagemDB-Ecommerce-BootcampDIO - ⚠️ Projeto de estudos
### Desafio de Projeto do Bootcamp Database Experience da DIO

#### Contextualizando a situação do negócio para melhor entendimento da modelagem.

O desafio nos pede para modelar um projeto conceitual de uma oficina.

####  Cliente

* A tabela cliente tem relacionamento n:m com as tabelas veiculos, cartao_de_credito e OS para que consigamos rastrear uma maior quantidade de informações possíveis através de um cliente.
* Um cliente poderá ter várias OS e uma OS só poderá ter um cliente.
* Um cliente pode ter vários cartões de crédito cadastrados.

#### Veículo

* A tabela veículo tem relacionamento N:M com a tabela cliente e com a tablea OS.
* A tabela veículo irá guardar as informações de todos os veículos cadastrados.
* Um veículo pode está registrado em várias OS e uma OS pode ter vários veículos.

#### Mecânico

* A tabela mecânico tem relacionamento n:m com a tabela OS.
* Todas as informações relacionados aos mecânicos da oficina estão nessa tabela.
* Uma OS pode ter mais de um mecânico e um mecânico pode ter mais de uma OS.

#### Serviços

* A tabela serviço tem um relacionamento n:m com a tabela OS.
* A tabela serviço registra todas as informações sobre os tipos de serviços oferecidos e seus valores.
* Uma OS pode ter vários tipos de serviço e um serviço pode está em várias OS.

#### Fornecedor

* A tabela fornecedor tem relacionamento n:m com a tabela suprimentos.
* A tabela fornecedor registra todas as informações de identificação de cada fornecedor cadastrado.
* Em seu relacionamento com a tabela suprimentos é definida a quantidade.
* Um fornecedor pode fornecer vários suprimentos e um suprimento pode ser fornecido por vários fornecedores.

#### Estoque

* A tabela estoque tem relacionamento n:m com a tabela suprimentos.
* A tabela estoque registra informações de identificação de cada estoque cadastrado.
* Em seu relacionamento com a tabela suprimentos é definida a quantidade de suprimentos em cada estoque.
* Um estoque pode conter vários suprimentos e um suprimento pode está em vários estoques.

#### Suprimentos

* A tabela suprimentos tem relacionamento n:m com as seguintes tabelas, estoque e fornecedor.
* A tabela suprimentos registra todas as informações referentes a cada suprimento utilizado na oficina, incluindo o valor de cada um.
* Um suprimento pode ser usado em várias OS e uma OS pode conter vários suprimentos.
* Em seu relacionamento com as tabelas estoque, fornecedor e OS, é definida a quantidade de suprimentos relacionadas a cada uma delas.

#### OS

* A tabela OS tem relacionamento N:M com as tabelas veiculos, forma_pgto, mecanico, serviço e suprimentos.
* É obrigatório que cada OS tenha um número identificador único, além do ID.

#### Pagamento e Cartões de Crédito

* A aplicação irá determinar a forma escolhida.
* A Tabela cartao_de_credito irá salvar as informações do cartão ou cartões utilizados e o ID irá identificar cada um.
* Um cartão pode ser cadastrado por vários clientes.
* Uma OS pode ter várias formas de pagamento e várias formas de pagamento podem ser usadas em várias OS.




### ⚠️ Este foi meu primeiro projeto conceitual de um Database, ainda preciso refiná-lo mais para deixar ele com a melhor desempenho possível.
