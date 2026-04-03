Dados são fatos brutos e que geralmelte não fazem sentido sozinhos;
Informações consistem no agrupamento de dados de forma organizada para fazer sentido;

Podemos afirmar que um banco de dados pode ter qualquer tamanho e complexidade;

Um banco de dados é que ele pode ser gerado e mantido
manualmente, ou pode ser computadorizado.

O SGBD é uma coleção de programas que facilita o processo de definição, construção, manipulação, compartilhamento, proteção e manutenção de um banco de dados.

A união do BD com SGBD é chamada de Sistema de Banco de Dados (SBD).

Antigamente os dados eram guardados em arquivos (por exemplo uma planilha do excel), mas isso gerava redundância de informações.


Os bancos de dados não contêm apenas dados - eles contêm também uma definição ou descrição completa da estrutura e restrições desses dados. Os bancos de dados possuem um catálogo com informações de cada tabela, sendo que as informações armazenadas no catálogo são chamadas de metadados, uma vez que trazem dados sobre os dados.

Abstração é a subtração de detalhes.

Uma visão (view) é um subconjunto do banco de dados.

O SGBD precisa incluir um software de controle de concorrência para garantir que vários usuários interajam simultaneamente com o banco de dados sem problemas.

Acid: Atomicidade, consistência, isolamento e durabilidade.
Atomicidade: Uma transação é uma unidade de processamento atômica que deve ser executada integralmente até o fim ou não deve ser executada de maneira alguma. Se as operações de gravação de uma transação devem ser confirmadas (commit), mas se alguma falha ocorrer a transação deve ser desfeita (rollback).

Consistência: A execução de uma transação deve levar o banco de dados de um estado consistente a um outro estado consistente.

Isolamento: Conjunto de técnicas que tentam evitar que transações paralelas interfiram umas nas outras.

Durabilidade: Os efeitos de uma transação em caso de sucesso devem persistir no banco de dados mesmo em casos de quedas de energia, travamentos ou erros.

Administrador de Banco de Dados (DBA) tem as seguintes responsabilidades: instalar o SGBD, autorizar o acesso ao banco de dados, coordenar e monitorar sua performance, adquirir recursos de software e hardware conforme a necessidade 
, por problemas (como falhas na segurança e demora na execução), assegurar-se de que os backups apropriados estão sendo feitos e estão íntegros, etc.

Administrador de dados (AD) Tem as seguintes responsabilidades: planejar, documentar, gerenciar e integrar os recursos de informação corporativos, além de entender bem o contexto da organização para que ele conheça se possível todos os dados armazenados.

A arquitetura mais comum para um SGBD é a arquitetura ANSI/SPARC (também conhecida como arquitetura de três esquemas). Seus 3 esquemas são: externo, conceitual e interno.

Um esquema de banco de dados é a descrição das estruturas, tabelas, campos, visões, índices, funções, entre outros antes dr que o banco de dados seja de fato implementado.

Uma instância (ou Estado) é o conjunto de dados armazenados no banco e um determinado momento de operação.