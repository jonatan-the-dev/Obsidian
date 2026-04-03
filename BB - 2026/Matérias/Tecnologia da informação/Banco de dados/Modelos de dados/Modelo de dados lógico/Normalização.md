Tags: [[Banco de dados]] | [[Modelo de dados lógico]]

A normalização serve para evitar redundância de dados e anomalias de atualização.

Um banco de dados está em determinada forma normal quando ele atende às regras necessárias.

Dependência funcional:
	- Uma coluna C1 depende funcionalmente de C2 quando C2 determina C1 (C2 -> C1);
	- Para cada valor de C2 aparece o mesmo valor de C1.

1 FN - Primeira Forma Normal
	- Todos os atributos devem conter apenas valores atômicos (simples, indivisível);
	- Não deve haver atributos com mais de um valor;
	- Passo a passo de como fazer a transformação para a 1 FN:
		- Remover colunas com dados repetidos;
		- Criar nova tabela para armazenas o dado repetido;
		- Criar relação entre as tabelas;

2 FN - Segunda Forma Normal
	- A relação tem que estar na 1 FN e não conter dependência parcial;
	- Dependência parcial: coluna que depende de uma parte de uma chave primária composta;
	- Passo a passo de como fazer a transformação para a 2 FN:
		- Identificar coluna com dependência parcial;
		- Criar nova tabela para essa coluna;

3 FN - Terceira Forma Normal
	- A relação tem que estar an 2 FN e nenhum atributo não chave for transitivamente dependente da chave primária;
	- Dependência transitiva: quando uma coluna, além de depender da chave primária, depende de outra coluna;
	- Passo a passo de como fazer a transformação para a 3 FN:
		- Identificar colunas que são funcionalmente dependentes de outras colunas não chave e criar tabelas à parte;