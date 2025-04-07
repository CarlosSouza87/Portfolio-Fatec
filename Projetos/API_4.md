<html>
<body>
 <h1 align="center"> API 4º Semestre - 02/2022</h1>
<h1 align="center"> 
<a href="https://github.com/Doc-Docker/APISubiter"><img src="https://img.shields.io/badge/GitHub-Repositório Projeto-181717?style=for-the-badge&logo=github"></a>
</h1>
 
 <h2> Parceiro Acadêmico: <a href="https://www.subiter.com/">Subiter</a></h2>
 
<img src="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/images/logosubiter.png" height="150" width="250"/>
  
  <h2 style="font-family:roboto;"> Resumo do Projeto :clipboard:</h2>
  
  <p align="justify" style="font-family:roboto;"> O projeto tem como objetivo solucionar o desafio de sincronização dos dados administrativos, financeiros e operacionais relacionados aos serviços prestados pela empresa. A falta de organização desses dados resulta em lentidão para atender chamados e dificuldades na interpretação dos indicadores comerciais e financeiros. Implementamos um sistema de gerenciamento integrado que centralizou informações relevantes por meio de um banco de dados robusto. Isso permitiu uma análise precisa dos indicadores comerciais e financeiros, facilitando a tomada de decisões estratégicas.

<h2 style="font-family:roboto;"> Tecnologias Adotadas :computer:</h2>
 
 <div style="display: inline_block"><br> 
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/oracle/oracle-original.svg" width="100"    height="100" />	 
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/java/java-original-wordmark.svg" width="100"    height="100" />
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/vuejs/vuejs-original.svg" width="100" height="100" />
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/docker/docker-original-wordmark.svg" width="100" height="100" />
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/bootstrap/bootstrap-original-wordmark.svg" width="100" height="100" />
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/intellij/intellij-original.svg" width="100" height="100" />
</div>
 
<br>
 
  <ul>
  <li><a href="https://www.oracle.com/br/cloud/">Oracle Cloud</a>: É uma plataforma de nuvem que oferece serviços abrangentes de armazenamento, computação e aplicativos, além de ser altamente escalável e segura.</p></li>
  </li>	  
  <li><a href="https://www.java.com/pt-BR/">Java</a>: É uma linguagem de programação de alto nível, multiplataforma e orientada a objetos, conhecida por sua portabilidade e segurança, amplamente usada no desenvolvimento de aplicativos e sistemas corporativos.</p></li>
  </li>
   <li><a href="https://vuejs.org/">Vue.js</a>: É um framework JavaScript progressivo e de código aberto para construção de interfaces de usuário interativas e dinâmicas. Ele oferece uma abordagem simples e flexível para o desenvolvimento de aplicações web modernas.</p></li>
  </li>
   <li><a href="https://www.docker.com/">Docker</a>: É uma plataforma de virtualização leve e portátil que permite empacotar, distribuir e executar aplicativos de forma isolada, garantindo a portabilidade e consistência do ambiente de desenvolvimento e produção.</p></li>
  </li>
   <li><a href="https://getbootstrap.com/">Bootstrap</a>: É um framework front-end de código aberto que facilita o desenvolvimento de interfaces responsivas e estilizadas, fornecendo um conjunto de estilos predefinidos e componentes reutilizáveis, agilizando o processo de criação de páginas web modernas e atraentes.</p></li>
  </li>
  <li><a href="https://www.jetbrains.com/idea/">IntelliJ IDEA</a>: É um ambiente de desenvolvimento integrado (IDE) altamente produtivo para programação em diversas linguagens.</p></li>
  </li>

  </ul>
  
  <h2 style="font-family:roboto;"> Contribuições Individuais :dart:</h2>
  
  <h3> Atribuições como Desenvolvedor</h3>

### ☁️ Oracle Cloud

Tive um papel fundamental na criação da modelagem do banco de dados no Oracle Cloud, ajustando as tabelas conforme a necessidade do cliente. Ajustei as tabelas conforme as necessidades do cliente, realizando modificações e refinamentos na estrutura do banco de dados. Isso envolveu a adição de novas colunas, a definição de índices para otimização de consultas e a criação de visões personalizadas para facilitar a interpretação dos dados pelos usuários.

<details>
      <summary>Modelo Lógico</summary>
<h1 align="center"> <img src = "https://github.com/Doc-Docker/APISubiter/blob/main/docs/Imagens/modelagem_sprint3.jpg" /></h1>
 
 </details> 

A centralização dos dados administrativos, financeiros e operacionais proporcionou uma análise mais precisa dos indicadores comerciais e financeiros, facilitando a geração de relatórios e métricas atualizados em tempo real. Essa visão mais clara dos dados contribuiu significativamente para a interpretação dos dados e para a tomada de decisões estratégicas.

### 🐳 Docker

Desempenhei um papel importante na criação dos containers e no processo de implantação das imagens no Docker para o front-end da aplicação. Comecei estudando as necessidades e requisitos técnicos do projeto, entendendo a arquitetura de cada componente do sistema. Com base nisso, trabalhei em conjunto com a equipe de desenvolvimento para definir a melhor estratégia de containerização.

 <details>
      <summary>Código em Dockerfile - Front-end</summary>

 ```docker
 
FROM node:lts-alpine
RUN npm install -g http-server
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
RUN npm run build
EXPOSE 4200
CMD [ "http-server", "dist" ]
 
 ```
 
 </details> 

No front-end, ajudei a criar o container Docker para a aplicação, garantindo que todos os recursos e dependências necessários estivessem configurados corretamente. Isso incluiu a seleção da imagem base apropriada, a configuração dos arquivos Dockerfile e o gerenciamento das variáveis de ambiente.
  
<h3> Atribuições como Product Owner</h3>
  <p align="justify" style="font-family:roboto;"> Como Product Owner nesse projeto, minha principal responsabilidade foi alinhar o backlog de produto, as tarefas do time de desenvolvimento e garantir que todas as etapas do projeto estivessem em conformidade com os objetivos definidos. Trabalhei em estreita colaboração com as partes interessadas para entender suas necessidades e traduzi-las em requisitos claros e priorizados.
 
Para começar, realizei uma análise abrangente dos desafios enfrentados pela empresa em relação à sincronização dos dados administrativos, financeiros e operacionais. Com base nessa análise, elaborei o backlog de produto, identificando as funcionalidades e melhorias necessárias para resolver o problema central. Priorizei as histórias de usuário de acordo com o valor agregado e o impacto nos indicadores comerciais e financeiros.

 <details>
      <summary>Sprint Backlog</summary>
<h1 align="center"> <img src = "https://github.com/Doc-Docker/APISubiter/blob/main/docs/Imagens/Backlog_Sprints3.PNG" /></h1>
 
 </details> 
 
Durante o desenvolvimento, mantive uma comunicação constante com o time de desenvolvimento, esclarecendo dúvidas, fornecendo orientações e garantindo que todos estivessem alinhados com os objetivos do projeto. Realizei reuniões de planejamento de sprint para revisar e refinar o backlog, além de definir as metas para cada interação, em colaboração com a equipe de desenvolvimento para dividir as histórias de usuário em tarefas específicas e acionáveis. Isso permitiu que o time trabalhasse de forma mais eficiente, com um fluxo contínuo de trabalho e uma melhor compreensão das expectativas e prazos.</p>
 
<h2 style="font-family:roboto;"> Aprendizados Efetivos :book:</h2>  

Neste projeto pude aprimorar minha habilidade em trabalhar com o Oracle Cloud como banco de dados, adquirindo conhecimentos específicos dessa tecnologia. Aprendi sobre a configuração do ambiente, criação de instâncias, modelagem de dados e ajustes necessários para atender às necessidades do cliente.

Ajudar na criação dos containers e no processo de implantação das imagens no Docker foi uma experiência valiosa. Compreendi como configurar e otimizar os ambientes de desenvolvimento e produção usando containers. Isso me permitiu compreender melhor os benefícios da containerização, como a portabilidade e a escalabilidade.

Além disso, o projeto me ensinou a importância da organização e centralização dos dados, assim como a sincronização e integração de informações entre diferentes áreas de uma empresa. Compreendi a relevância de ter um sistema capaz de disponibilizar os dados de forma rápida e organizada, permitindo melhorias significativas no atendimento ao cliente e na análise dos indicadores comerciais e financeiros. Também aprendi a importância da comunicação clara, priorização baseada em valor, flexibilidade, empatia com os usuários e análise contínua como Product Owner.

  <h3 align="center"> Hard Skills </h3>
  <table align="center">
    <tr>
      <th width="290px">Tecnologia/Metodologia</th>
      <th width="85px">Nota</th>
      <th width="240px">Classificação</th>
    </tr>
    <tr>
      <td>Metodologia Scrum - Product Owner</td>
      <td>★★★★☆</td>
      <td>Sei fazer com ajuda</td>
    </tr>
    <tr>
      <td>Oracle Cloud</td>
      <td>★★★☆☆</td>
      <td>Entendi</td>
    </tr>	
    <tr>
      <td>Java</td>
      <td>★★★☆☆</td>
      <td>Entendi</td>
    </tr>
    <tr>
      <td>Vue.js</td>
      <td>★★★☆☆</td>
      <td>Entendi</td>
    </tr>
   <tr>
      <td>Docker</td>
      <td>★★★★☆</td>
      <td>Sei fazer com ajuda</td>
    </tr>
   <tr>
      <td>Bootstrap</td>
      <td>★★★★★</td>
      <td>Sei fazer com autonomia</td>
    </tr>
    <tr>
      <td>IntelliJ IDEA</td>
      <td>★★★☆☆</td>
      <td>Entendi</td>
    </tr>
  </table>
  
  <h3 align="center">Soft Skills</h3>
  <table align="center">
    <tr>
      <th width="270px">Habilidade</th>
      <th width="290px">Descrição</th>
    </tr>
    <tr>
      <td>Responsabilidade</td>
      <td>Assumi o cargo de Product Owner pela primeira vez.</td>
    </tr>
    <tr>
      <td>Visão de Negócio</td>
      <td>Compreendi melhor os problemas e expectativas do cliente, aplicando o Product Backlog Building.</td>
    </tr>
    <tr>
      <td>Comunicação</td>
      <td>Precisei me comunicar com o cliente com resiliência, e transmitir os requisitos para equipe dev.</td>
    </tr>
    <tr>
      <td>Organização</td>
      <td>Precisei organizar as tarefas do time e definir as prioridades.</td>
    </tr>
    <tr>
      <td>Planejamento</td>
      <td>Precisei planejar o escopo do projeto e construir o Product Backlog de uma forma prática.</td>
    </tr>
  </table>
  
---

 <h2 align="center"> Git do Projeto link:</h2>

   
   <p align="justify" style="font-family:roboto;"><li>4° Semestre: Subiter - Aplicação Web para sincronização dos dados administrativos, financeiros e operacionais.</a></li></p>
   
</body>
</html>
