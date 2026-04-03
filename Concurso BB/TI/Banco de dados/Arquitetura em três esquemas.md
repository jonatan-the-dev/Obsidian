Na arquitetura em três esquemas, há separação da lógica de apresentação, da lógica de negócio e da lógica de acesso a dados, o que proporciona flexibilidade aos sistemas. Nessa arquitetura, há três níveis:
 

- Nível interno: nível de armazenamento (forma em que os dados são armazenados dentro do sistema);
- Nível conceitual: nível lógico (intermediário entre o nível interno e o externo); descrição dos registros.
- Nível externo ou visão ou nível computacional: forma como os dados são vistos por usuários individuais.

![[Pasted image 20260119184006.png]]

Nível externo: Também conhecido como Nível de Visão ou Nível lógico do Usuário, inclui uma série de visões do usuário. Cada visão descreve a parte do banco de dados em que um grupo de usuários em
particular está interessado e oculta o restante do banco de dados do grupo de usuários. Trata-se do nível mais próximo dos usuários.

Nível conceitual: Também conhecido como Nível Lógico de comunidade (ou apenas Nível Lógico), é um nível indireto entre os níveis interno e externo. Trata-se de uma maneira de descrever a estrutura do banco de dados inteiro para uma comunidade de usuários, isto é, quais dados são armazenados em todo o banco de dados e como os dados estão inter-relacionados. Esse nível oculta os detalhes das estruturas de armazenamento físico e se concentra na descrição de entidades.

Nível interno: Também conhecido como Nível de Armazenamento ou Físico, é o meio mais próximo do meio de armazenamento físico, isto é, aquele que se ocupa com o modo como os dados estão fisicamente armazenados no banco de dados e no hardware do computador – além da definição das estruturas físicas que permitem obter um desempenho satisfatório. Ele descreve os detalhes completos do armazenamento de dados e dos caminhos de acesso para o banco de dados.

Sempre que tivermos uma arquitetura de SGBD com vários níveis, devemos pensar em como esses níveis se comunicam. Basicamente, isso é feito por meio de mapeamentos!

Quando estamos falando sobre independência de dados, estamos tratando da capacidade de modificar a definição dos esquemas de determinado nível, sem afetar o esquema de nível superior. Existem dois níveis de independência de dados: a independência física e a independência lógica.
	A independência lógica dos dados trata da capacidade de alterar o esquema conceitual sem precisar modificar os esquemas externos ou programas/aplicações. O mapeamento nível externo para o conceitual é a chave para a independência lógica de dados.
	A independência física dos dados trata da capacidade de alterar o esquema interno sem ter de	alterar o esquema conceitual. O mapeamento nível conceitual para o interno é a chave para a
	independência física de dados.


![[Pasted image 20260119184430.png]]



![[Pasted image 20260119184436.png]]

