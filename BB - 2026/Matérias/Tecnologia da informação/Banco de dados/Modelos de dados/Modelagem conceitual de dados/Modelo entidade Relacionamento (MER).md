Tags: [[Banco de dados]] | [[Modelagem conceitual de dados]] | [[Superclasse]] | [[Subclasse]] | [[Teoria dos conjuntos]]

![[Pasted image 20260222160732.png]]
![[Pasted image 20260222162546.png]]

Superclasse (Entidade de Alto Nível): Entidade mais generalista.
Subclasse (Entidade de Baixo Nível): Entidade mais específica.

Uma entidade pode ter atributos multivalorados (que podem ter mais de um valor), para esses atributos deve ser criada uma tabela separada que contenha a chave da entidade e o valor do atributo.

Cardinalidade se lê considerando o relacionamento por exemplo:
"Cliente: (1,1) Pedido: (0,n)" Significa que cada cliente pode ter 0 até n pedidos e cada pedido pode ter no mínimo 1 e no máximo 1 cliente.
Quando na cardinalidade só tiver um dos 2 valores (mínimo e máximo) esse único valor é o máximo (nesse caso o mínimo não está sendo informado).
Quando tem uma cardinalidade N:N é necessário que seja criado uma tabela extra.

Entidade Associativa (ou Agregação) significa que um relacionamento está sendo tratado como uma entidade. É representado por um losango dentro de um retângulo.
	Situações onde a Entidade Associativa é usada:
		- Quando o relacionamento possui atributos próprios.
		- Quando o relacionamento precisa se ligar a outra entidade.

Quando há um auto relacionamento é necessário descrever os papeis que cada entidade pode exercer.

Função é uma relação entre dois conjuntos A e B, não vazios, de forma que todo elemento de A tem um elemento correspondente em B e um elemento de A só possui um único correspondente no conjunto B.

Uma entidade fraca (ligada através de uma linha dupla ou uma linha mais grossa) tem identificador composto por seu próprio atributo chave e os atributos chave da entidade à qual está associada.

Em um relacionamento ternário é necessário formar duplas:![[Pasted image 20260225200052.png]]
Por exemplo nesse diagrama está sendo dito que um distribuidor distribui algum produto em n cidades, ou que um distribuidor distribui em uma cidade n produtos, ou que um produto numa cidade é distribuído por n distribuidores.

Hierarquias IS-A
	- representam o conceito de especialização e generalização ("IS-A" vem do inglês "is a" ou em português "é um") e servem para representar dados que compartilham características comuns (é o equivalente à herança na Programação Orientada a Objetos). 
		- Por exemplo temos a Superclasse "Funcionário" e a Subclasse "Secretário". Isso é útil para não termos muitos campos vazios na tabela de funcionários.
	- Pode ser parcial (representado pela letra "p") que permite que uma Superclasse não necessariamente precisa estar atrelada a alguma Subclasse (resumidamente nem todo elemento da SuperClasse precisa estar na subClasse, até mesmo nenhum é possível). Também pode ser total (representado pela letra "t") que diz que uma Superclasse necessariamente precisa estar atrelada a alguma Subclasse (resumidamente todo elemento da Superclasse precisa estar na Subclasse).
	- Pode ser exclusiva (a Superclasse só pode estar atrelada a no máximo uma das Subclasses) resumidamente isso quer dizer que um elemento da Superclasse só pode estar em uma de suas Subclasses. Também pode ser não exclusiva (a Superclasse pode estar relacionada a "n" subclasses) resumidamente isso quer dizer que um elemento da Superclasse pode estar em várias Subclasses.
	- ![[Pasted image 20260209204906.png]]


