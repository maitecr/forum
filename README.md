# forum

Projeto realizado a partir do curso de Sring Boot API REST da Alura, simulando o ambiente de fórum da própria Alura aplicado ao Spring Boot e ao padrão de projeto MVC (model, view, controller).

No padrão MVC, temos os eixos:

Modelo: compõe a estrutura e gerencia o comportamento dos dados através de regras de negócios, lógica, funções, etc;

View: apresenta as respostas das requisições solicitadas;

Controller: onde o usuário pode interagir com a aplicação a partir de métodos e ações já definidas, fazendo a mediação entre entrada e saída de informações.


As dependências utilizadas:
Spring Web: composto pelo Spring MVC que nos fornece a estrutura e configurações adequadas para desenvolvermos uma aplicação MVC; contém também o TomCat, um servidor web voltado para Java; atuando juntamente com o Servlet, tendo como principal função lidar com as requisições HTTPs;

Spring Dev Tools: um facilitador para o desenvolvimento de aplicações Java, onde se dispensa a necessidade de reiniciar a aplicação para testes;

Spring JPA (Java Persistence API): dependência utilizada para mapeamento e persistência de objetos relacionais através de anotações de metadados que transformavam as classes em entidades;

H2 Database: banco de dados em memória local.


A aplicação foi desenvolvida trabalhando no conceito e criação de um CRUD (creat, read, update, delete), onde a comunicação estabelecida para requisições-respostas se davam através do modelo REST (Representational State Transfer), por via dos verbos HTTPs (post, put, delete, get).
Para a comunicação entre o Controller e o Banco de Dados, foi utilizado a Interface JpaRepository, pois, nela, já constam os métodos voltados para a elaboração CRUD, onde temos embutida a query adequada para a operação e o estabelecimento comunicação com o Banco de Dados.
Dessa forma, também foi trabalhado os conceitos e aplicações de tranferências de informações entre DTOs, Forms e as entidades. Onde teremos o DTO (Data Transfer Object) atuando na conversão e transferência de dados vindos de um Entidade para retornar como resposta no módulo View os dados solicidades pelo Controller a partir do método Get. Enquanto que o modelo Form (formulário) é usado como intermediário para a transferência de dados informados pelo cliente para registro na Entidade através dos métodos Post e Put.
