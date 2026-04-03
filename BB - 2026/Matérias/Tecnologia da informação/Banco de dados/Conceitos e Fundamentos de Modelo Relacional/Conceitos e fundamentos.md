Tags: [[Comandos SQL]] | [[Banco de dados]]

Cláusulas:
	- CHECK = Garante que os valores presentes em uma coluna satisfazem uma condição;
	- NOT NULL = Garante que os valores inseridos em uma coluna não serão nulos;
	- UNIQUE = Garante que os valores em uma coluna são únicos (não se repetem);
	- PRIMARY KEY = Restrição que combina as restrições NOT NULL e UNIQUE. Ou seja, identifica unicamente uma linha de uma tabela;
	- FOREIGN KEY - Possibilita a criação de relacionamentos entre tabelas;
	- DEFAULT - Cria um valor padrão (default) para uma coluna se ela não respeitar um valor específico.

O nível de isolamento de uma transação pode ser definido com o comando "SET TRANSACTION ISOLATION LEVEL" e existem 4 níveis possíveis, do menos restritivo (mais performático, porém mais suscetível a erros) ao mais restritivo (mais seguro, porém com menor concorrência). Além de que tem três fenômenos de leitura (anomalias) que eles buscam evitar:
	- Leitura Suja (Dirty Read): Ocorre quando uma transação lê dados que foram alterados por outra transação que ainda não foi concluída (não sofreu commit);
	- Leitura não repetível (Non-Repeatable Read): Acontece quando uma transação lê a mesma linha duas vezes durante sua execução e, entre essas leituras, outra transação altera e comita essa dado;
	- Leitura Fantasma (Phantom Read): Semelhante à leitura não repetível, mas afeta um conjunto de linhas.
![[Pasted image 20260308163216.png]]

Domínio são "regras de aceitação" de uma coluna na sua tabela. O domínio geralmente engloba duas coisas:
	- O tipo do Dado (Data Type);
	- As restrições (Constraints);
