	


	Projeto individual Marcos da Costa Retondar




	Perguntas:

	1- Quais são as entidades necessárias?

	As entidades necessárias são: Empresa_Parceira, Tecnologia, Tecnologias_Utilizadas e Colaborador.

	2- Quais são os principais campos e seus respectivos tipos?

	Empresa_Parceira:

	id: int PK
	nome: varchar
	endereco: varchar
	telefone: varchar
	email: varchar



	Tecnologia:

	id: int PK
	nome: varchar
	area: varchar



	Tecnologias_Utilizadas:


	empresa_parceira_id:  FK (chave estrangeira)
	tecnologia_id: FK (chave estrangeira)




	Colaborador:

	id: int PK
	nome: varchar
	cargo: varchar
	empresa_parceira_id: int (chave estrangeira)



	3- Como essas entidades estão relacionadas?

	A entidade Empresa_parceira tem uma relação um-para-muitos com a entidade Colaborador através do campo empresa_parceira_id.

	A entidade Empresa_parceira tem uma relação um-para-muitos com a entidade Tecnologias_Utilizadas através do campo empresa_parceira_id

	A entidade Tecnologias tem uma relação um-para-muitos com a entidade Tecnologias_Utilizadas através do campo tecnologia_id.




	4- Simule 2 registros para cada entidade:

	Empresa_Parceira:

	ID: 1
	Nome: First Tecnology
	Endereço: Rua Astoufo, 123
	Telefone: (11) 1234-5678
	Email: empresafirsttecnology@example.com

	ID: 2
	Nome: Secund Tecnology
	Endereço: Rua Gilseilani, 456
	Telefone: (22) 9876-5432
	Email: empresasecundtecnology@example.com



	Tecnologia:

	ID: 1
	Nome: Python
	Área: Desenvolvimento de Dados

	ID: 2
	Nome: JavaScript
	Área: Desenvolvimento Web



	Tecnologias_Utilizadas:

	ID da Empresa Parceira: 1
	ID da Tecnologia: 1


	ID da Empresa Parceira: 2
	ID da Tecnologia: 2



	Colaborador:

	ID: 1
	Nome: Ludwig van Beethoven
	Cargo: Desenvolvedor
	ID da Empresa Parceira: 1

	ID: 2
	Nome: Johann Sebastian Bach
	Cargo: Analista de Marketing
	ID da Empresa Parceira: 2