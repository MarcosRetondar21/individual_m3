Projeto individual Marcos da Costa Retondar

Quais são as entidades necessárias?

As entidades necessárias são: Empresa_Parceira, Tecnologia, Tecnologias_Utilizadas e Colaborador.

Quais são os principais campos e seus respectivos tipos?

Empresa_Parceira:

id: int
nome: varchar
endereco: varchar
telefone: varchar
email: varchar



Tecnologia:

id: int
nome: varchar
area: varchar



Tecnologias_Utilizadas:

id: int
empresa_parceira_id: int (chave estrangeira)
tecnologia_id: int (chave estrangeira)




Colaborador:

id: int
nome: varchar
cargo: varchar
empresa_parceira_id: int (chave estrangeira)



Como essas entidades estão relacionadas?

A entidade Tecnologias_Utilizadas tem uma relação muitos-para-um com a entidade Empresa_Parceira através do campo empresa_parceira_id.
A entidade Tecnologias_Utilizadas tem uma relação muitos-para-um com a entidade Tecnologia através do campo tecnologia_id.
A entidade Colaborador tem uma relação muitos-para-um com a entidade Empresa_Parceira através do campo empresa_parceira_id.



Simule 2 registros para cada entidade:

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

ID: 1
ID da Empresa Parceira: 1
ID da Tecnologia: 1

ID: 2
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