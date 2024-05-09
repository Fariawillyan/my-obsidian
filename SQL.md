Referência Livro: **SQL para análise de dados, O'REILLY**

Linguagem usada na comunicação com banco de dados;

0. Sublinguagens do SQL:

	DQL -> SELECT.
	DDL -> CREATE, ALTER e DROP
	DCL -> GRANT e REVOKE
	DML -> INSERT, UPDATE e DELETE.

Tipos:
1. **Banco de Dados Row Store:**

	- Armazena dados por linha, onde cada linha contém todas as colunas dos registros.
	- Ótimo para operações que exigem leitura e escrita de linhas completas, como transações OLTP (Processamento de Transações On-Line).
	- Melhor desempenho em atualizações de dados individuais.
	- Pode ter desempenho inferior em análises e consultas que envolvem agregações em grandes conjuntos de dados.

2. **Banco de Dados Column Store:**

	- Armazena dados por coluna, onde cada coluna contém todos os valores para uma única propriedade ou campo.
	- Ótimo para operações analíticas e consultas que envolvem agregações em grandes conjuntos de dados.
	- Melhor desempenho em consultas que envolvem apenas algumas colunas.
	- Pode ter desempenho inferior em operações de atualização e inserção de dados.

Essencialmente, a diferença reside na forma como os dados são organizados no disco: por linha (Row Store) ou por coluna (Column Store), cada um com vantagens e desvantagens dependendo das necessidades específicas de uma aplicação.