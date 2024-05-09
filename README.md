
# Desafio de Projeto - Processando e Transformando Dados com Power BI

Link do Relátorio:
https://app.powerbi.com/links/ZFiM761SAz?ctid=d193e68c-e53f-4610-a66d-56ff300fec7a&pbi_source=linkShare

# Ferramentas
Azure, MySQL Workbench, Power BI

# Relátorio da Coleta e Limpeza de Dados
1. Criei uma instância na Azure para MySQL, e após isso me conectei ao MySQL WorkBench para criar a base de dados fornecida.

2. Integrei o banco de dados da Azure com o Power BI.

3. Alterei o nome das tabelas para melhor identificação.

4. Alterei os cabeçalhos e os tipos de dados de cada tabela, como por exemplo a alteração do tipo de salary, coloquei em Número decimal fixo.

5. Manti os valores nulos por achar que possuem relevância. Em horas de projetos, decidi remover o projeto com 0 horas trabalhadas, por não achar relevante um projeto que não teve recursos.

6. Separei a coluna de endereço em colunas mais simples, como número, rua e país.

7. Mesclei a coluna de nome e sobrenome em uma só, chamada 'nome completo'.

8. Mesclei as tabelas Employee e Departamento em uma só, mantendo a coluna do Id do departamento e o seu nome, associando-os a cada colaborador, e eliminei as colunas desnecessárias.

9. Após isso, mesclei duas consultas de funcionários, deletei as colunas e deixei apenas os Colaboradores e o Id do gerente associado, e modifiquei o id do cliente para o nome, na aba de substuir valores, assim, atribuindo o nome de gerente a cada colaborador.

10. Na tabela de localização, mesclei a tabela de departamento e a de localização, usando como base a coluna de ID, após isso, peguei o nome e o Mgr_ssn, e em seguida mesclei as colunas localização e departamento, criando um departamento-local único.

- Por que usamos apenas o mesclagem nessa situação?
Porque estamos combinando duas tabelas com base em uma coluna comum, que no caso é o Id do departamento. A atribuição apenas serveria para adicionar novas linhas, sem criar a combinação

11. Em seguida, agrupei os dados para saber quantos colaboradores existem por gerentes, usando a opção de "Agrupar por", usando a tabela gerente e a operação de contar linhas.

# Prints do Processo de Limpeza

![print01](https://github.com/devVHP/Desafio-de-Projeto---Processando-e-Transformando-Dados-com-Power-BI/blob/main/Prints/Captura%20de%20tela%202024-05-09%20174506.png?raw=true)
![print02](https://github.com/devVHP/Desafio-de-Projeto---Processando-e-Transformando-Dados-com-Power-BI/blob/main/Prints/Captura%20de%20tela%202024-05-09%20174528.png?raw=true)
![print03](https://github.com/devVHP/Desafio-de-Projeto---Processando-e-Transformando-Dados-com-Power-BI/blob/main/Prints/Captura%20de%20tela%202024-05-09%20174539.png?raw=true)
![print04](https://github.com/devVHP/Desafio-de-Projeto---Processando-e-Transformando-Dados-com-Power-BI/blob/main/Prints/Captura%20de%20tela%202024-05-09%20174449.png?raw=true)
![print05](https://github.com/devVHP/Desafio-de-Projeto---Processando-e-Transformando-Dados-com-Power-BI/blob/main/Prints/Captura%20de%20tela%202024-05-09%20174738.png?raw=true)