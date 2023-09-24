# desafio-ETL-PowerBI

1) Base de dados do Azure foi conectada ao Power BI.
2) Foram retiradas todas as colunas que não seriam utilizadas de todas as tabelas.
3) Foi alterado o tipo das colunas que estavam com tipo divergente do conteúdo da mesma.
4) Foi realizado agrupamento na tabela Works_On para descobrir o número de horas por projeto.
5) Na tabela Employee foi substituído o valor "Oak-Humble" para "Oak Humble" para poder dividir a coluna de endereço.
6) Na tabela Employee foi dividida a coluna Address em 4 colunas e renomeadas para: Number, Street, City, State.
7) A tabela Employee foi mesclada como nova com a tabela Departament e esta nova consulta foi nomeada como Employee_Departament.
8) Na tabela Employee_Departament, foram retiradas as colunas que não seriam utilizadas, deixando apenas as colunas Employee.Fname, Employee.Minit, Employee.Lname, Departament.Dname.
9) A tabela Employee foi mesclada como nova com a própria tabela e esta nova consulta foi nomeada como Employee_Manager.
10) Na tabela Employee_Manager foram mantidas apenas as colunas com o nome do funcionário e o nome do seu respectivo gestor.
11) Na tabela Employee_Manager as colunas Fname, Minit e Lname foram mescladas e a nova coluna renomeada par FullNameEmployee.
12) A tabela Dpartament foi mesclada como nova com a tabela Dept_Location, sendo esta nova consulta nomeada como Departament_Location, mantendo as colunas Departament.Dname e Dept_Location.Dlocation e estas foram mescladas em uma nova coluna chamada pk_dept_location criando uma chave primária.
13) Na tabela Employee_Manager foi realizado um agrupamento para visualizar quantos funcionários há por gerente.
14) Foi aplicada a tranformação nos dados e criado dois gráficos para visualizar a quantidade de horas por projeto e a quantidade de funcionários por gerente.

Para realizar a concatenação entre as colunas Departament.Dname e Dept_Location.Dlocation só pode ser realizada através da mesclagem e não da atribuição, pois precisamos que s valores estejam emparelhados e não empilhados, ou seja, precisamos que o departamento esteja na mesma linha que a localização e não na mesma coluna.
