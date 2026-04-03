
Projetos de banco de dados:
	Modelo Conceitual (ou Modelo de Alto Nível): Oferece conceitos que são mais próximos ao modo como muitos usuários compreendem os dados. Ele utiliza conceitos como entidades, atributos e relacionamentos. Em geral, é utilizado para envolver o cliente e discutir os aspectos do negócio e, não, da tecnologia, visto que não há limitações ou tecnologias específicas.
	Modelo lógico (ou Modelo de Implementação ou Representativo): Oferece conceitos que podem ser facilmente entendidos pelos usuários finais, mas que não está muito longe do modo como os dados são organizados e armazenados no computador. Em geral, eles ocultam muitos detalhes do armazenamento de dados em disco, mas podem ser implementados diretamente em um sistema de computador.
	Modelo físico (ou Modelo Baixo Nível): Oferece conceitos que descrevem os detalhes de como os dados são armazenados no computador. Eles costumam ser voltados para especialistas de computadores e, não,  para usuários finais. O modelo físico é a implementação concreta do projeto, sendo totalmente dependente do SGBD.

A implementação mais popular do Modelo Conceitual é o Modelo Entidade-Relacionamento (MER) que é considerado um modelo semântico, uma vez que tenta capturar o significado dos dados.
	O Modelo Entidade-Relacionamento (MER) descreve um contexto (chamado de mini-mundo) em termos de entidades, relacionamentos e atributos. Para facilitar a visualização desse modelo, foi criada uma notação gráfica conhecida como Diagrama Entidade-Relacionamento (DER).
		Entidade: qualquer objeto que exista e que pode ser distinguido de outros objetos, podendo ser concreto ou abstrato. Uma entidade é representada por meio de um retângulo com seu nome e uma ocorrência específica de uma entidade é chamada de instância. Existem três tipos de entidades:
			Entidade forte (ou Entidade Independente): Representado por um retângulo, são aquelas cuja existência independe de outras entidades, ou seja, por si só elas já possuem total sentido de existir.
			Entidade Fraca (ou Entidade Dependente): Representado por um duplo retângulo, são aquelas cuja existência depende de outra entidade e que não podem ser identificadas unicamente por seus atributos.
			Entidade Associativa: surge quando há a necessidade de associar uma entidade a um relacionamento existente ou associar dois relacionamentos entre si, é representada por um retângulo desenhado ao redor de um losango.
		Relacionamento: é a relação que existe entre entidades, isto é, a ligação lógica entre entidades que representa uma regra ou restrição de negócio, possibilitando entender como uma entidade se comporta em relação às demais, qual o seu grau de dependência de outras entidades e qual a associação de dados existentes entre elas. O relacionamento é representado por um losango.  É possível que haja um auto-relacionamento ou um relacionamento recursivo. Em complemento às entidades fracas, tem os relacionamentos fracos (que são representados por um losango duplo).
		Classificação de Relacionamentos: Os relacionamentos podem ser classificados de duas formas: quanto ao grau e quanto à cardinalidade:
			Quanto ao Grau: Representa o número de tipos de entidades que participam de um relacionamento, podendo ser binário, ternário, quaternário, entre outros.
			Quanto à Cardinalidade: Representa a quantidade de ocorrências ou instâncias de cada entidade presente no relacionamento - pode receber os seguintes valores: 1:1, 1:N, N:1 e M:N.
			Relacionamento 1:1 (UM-PARA-UM)			![[Pasted image 20260120190341.png]]
			Relacionamento 1:N (UM-PARA-MUITOS)
			![[Pasted image 20260120190425.png]]
			Relacionamento N:M (MUITOS-PARA-MUITOS)
			![[Pasted image 20260120190602.png]]
		Existem algumas restrições em relacionamentos que permitem limitar as combinações possível entre as entidades que participam de um relacionamento.
			Restrição de Participação Total: toda instância de uma Entidade A deve possuir uma ou mais instâncias de uma Entidade B associada a ela (são representadas por linhas duplas ou por uma linha mais grossa).
			Restrição de Participação Parcial: nem toda instância de uma Entidade A deve possuir uma instância de uma Entidade B associada a ela (são representadas por linhas simples).
	Atributos: São usados para descrever as propriedades ou características de uma entidade ou relacionamento, são representados graficamente através de círculos ou elipses.
		Um atributo pode ser monovalorado ou multivalorado (possuir mais de um valor) a representação gráfica de um atributo multivalorado é uma elipse dupla.

![[Pasted image 20260121203855.png]]

