<h1 align="center"> API -  2º Semestre</h1>
<h2 align="center">:office: EMPRESA - NECTO SYSTEMS</h2>


----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# :clipboard: Desafio/Projeto
Neste projeto foi proposto a construção de uma integração para a coleta de informações diretamente dos servidores, visando a criação de uma série histórica de dados. A concepção por trás disso era criar uma aplicação que pudesse realizar a coleta regular de métricas de um ou mais Sistemas Gerenciadores de Banco de Dados remotos. Essa ferramenta é projetada para fornecer informações valiosas ao usuário, permitindo que tomem decisões informadas em relação à manutenção, balanceamento, escalabilidade e melhorias necessárias nos seus SGBDs, bancos de dados e infraestrutura de servidores.
Ao realizar essa integração, o objetivo é capacitar os usuários a monitorar de perto o desempenho de seus sistemas, identificar tendências ao longo do tempo e agir de forma proativa para otimizar e manter a estabilidade de suas operações. Ao fornecer uma visão holística das métricas do sistema, essa aplicação permite que os usuários tomem decisões fundamentadas sobre ajustes necessários, sejam eles relacionados a melhorias na eficiência dos bancos de dados, balanceamento de carga ou mesmo escalonamento da infraestrutura para atender às demandas crescentes.
Essa iniciativa reflete um entendimento avançado das necessidades de gestão de banco de dados e infraestrutura, demonstrando a capacidade de criar soluções práticas para otimizar a operação dos sistemas e garantir sua confiabilidade e eficácia contínuas.
<br></br>
## :desktop_computer: Tecnologias Utilizadas
<ul>
<div style="display: inline_block"><br> 
 <img src="https://github.com/devicons/devicon/blob/master/icons/postgresql/postgresql-original-wordmark.svg" width="100" height="100"/>
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/java/java-original-wordmark.svg" width="100"    height="100" />
 <img src="https://github.com/devicons/devicon/blob/master/icons/spring/spring-original-wordmark.svg" width="100" height="100" />
 
</div>
</ul>


 <br></br>
 <a href="https://github.com">Github</a>: Esta plataforma foi utilizado como repositorio do projeto. O Github é uma plataforma de gerenciamento de código fonte que permite hospedar, gerenciar e colaborar em projetos de desenvolvimento de software usando o sistema de controle de versão Git.
<br></br>
<a href="https://www.postgresql.org">PostgreSQL</a>: Este sistema foi utilizado como Sistema Gerenciador de Banco de Dados (SGBD) do projeto. O PostgreSQL é um sistema de gerenciamento de banco de dados relacional de código aberto que oferece um alto grau de confiabilidade e flexibilidade.
<br></br>
<a href="https://www.java.com">Java</a>:Esta Linguagem foi utilizada para a descompactação dos dados. Java é uma linguagem de programação versátil e amplamente utilizada, conhecida por sua portabilidade e capacidade de criar aplicativos de alta performance.
<br></br>
<a href="https://www.pgadmin.org">pgAdmin</a>: Esta plataforma foi utilizada como interface gráfica para administrar dados no PostgreSQL. O pgAdmin é uma ferramenta de administração de banco de dados que facilita a administração e a manipulação de dados no PostgreSQL por meio de uma interface gráfica amigável.



-------------------------------------------------------------------------------------------------------------------------------------------------------------

 ## :dart: Contribuições Individuais: 

 **1° Sprint**
- Instalação do Banco de dados Postgres;
- Criação e modelagem do banco de dados;
- Criação das tabelas e colunas definidas.

 **2° Sprint**  
- Apoio na criação da conexão da aplicação ao Banco de dados;
- Gerenciamento do Banco de dados atraves do seu SGBD.

 **3° Sprint**
 - Auxilio com a montagem do readme e inserção dos dados da Aplicação;
 - Criação das consultas (queries) necessárias para recuperar os dados e desenvolver procedimentos armazenados (procedures) para a execução eficiente dessas operações;
 - Ajustes em tabelas e colunas do banco de dados.

 **4° Sprint**
 - Apresentação final da aplicação ao cliente.
		  
</details>

<br></br>

<h3 align="center"> Hard Skills </h3>
  <table align="center">
    <tr>
      <th width="300px">Tecnologia/Metodologia</th>
      <th width="300px">Classificação</th>
    </tr>
    <tr>
      <td>POSTGRESQL</td>
      <td>★★★★☆</td>
    </tr>	
   <tr>
      <td>JAVA</td>
      <td>★☆☆☆☆</td>
    </tr>
    <tr>
      <td>GITHUB</td>
      <td>★★☆☆☆</td>
    </tr>
  </table>

 <h3 align="center">Soft Skills</h3>
  <table align="center">
    <tr>
      <th width="300px">Habilidade</th>
      <th width="300px">Descrição</th>
    </tr>
    <tr>
      <td>Comunicação</td>
      <td>Utilizei minha boa comunicação com a equipe para juntos compreender o que deveria ser e implementado na escrita do projeto.</td>
    </tr>
    <tr>
      <td>Adaptabilidade</td>
      <td>Precisei aprender a me adaptar nas diversas tecnologias do projeto para a compreensão e realização de minhas atividades.</td>
    </tr>
    <tr>
      <td>Trabalho em Equipe</td>
      <td>Desenvolvi bastante esta Soft Skills para sanar todas as duvidas no decorrer do projeto e, além disso, a comunicação entre o grupo para imediatamente instruir sobre o que estava sendo feito e no que deverimos nos aprimorar.</td>
  </table>

</table>
  <h2 align="center">  Comandos Utilizados  na aplicação </h2>
  <table align="center">
 select * from pg_stat_statements

/*10 Consultas mais demoradas*/
SELECT total_exec_time, query
FROM pg_stat_statements
ORDER BY total_exec_time
DESC LIMIT 10;

/*Consultas mais demoradas em média*/
SELECT mean_exec_time, query
FROM pg_stat_statements
ORDER BY mean_exec_time
DESC LIMIT 10;

/*Chamadas mais de 1000 vezes*/
SELECT calls, query, total_exec_time
FROM pg_stat_statements
where calls > 1000;

/*Tamanho banco dos bancos de dados excluindo os bancos do sistema, possibilidade de inserir só o banco em que estou logado*/
SELECT
	datname                                   AS banco,
	pg_database_size(datname)                 AS tamanho,
	pg_size_pretty(pg_database_size(datname)) AS tamanho_pretty
FROM pg_database
WHERE datname NOT IN ('template0', 'template1', 'postgres') /*Inserir o banco que estou logado*/
ORDER BY tamanho DESC, banco ASC

/*Tamanho banco dos bancos de dados excluindo os bancos do sistema*/
(SELECT
	datname                                   AS banco,
	pg_database_size(datname)                 AS tamanho,
	pg_size_pretty(pg_database_size(datname)) AS tamanho_pretty
FROM pg_database
WHERE datname NOT IN ('template0', 'template1', 'postgres') 
ORDER BY tamanho DESC, banco ASC)

UNION ALL

(SELECT
	'TOTAL'                                        AS banco,
	sum(pg_database_size(datname))                 AS tamanho,
	pg_size_pretty(sum(pg_database_size(datname))) AS tamanho_pretty
FROM pg_database
WHERE datname NOT IN ('template0', 'template1', 'postgres'));


/*Tamanhos de tabelas*/
SELECT esquema, tabela,
       pg_size_pretty(pg_relation_size(esq_tab)) AS tamanho,
       pg_size_pretty(pg_total_relation_size(esq_tab)) AS tamanho_total
  FROM (SELECT tablename AS tabela,
               schemaname AS esquema,
               schemaname||'.'||tablename AS esq_tab
          FROM pg_catalog.pg_tables
         WHERE schemaname NOT
            IN ('pg_catalog', 'information_schema', 'pg_toast') ) AS x
 ORDER BY pg_total_relation_size(esq_tab) DESC;
 

   
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<h2 align="center"> GITHUB DO PROJETO</h2>

 <h3 align="center">https://github.com/apibanco/Vigilant</h3>
 
