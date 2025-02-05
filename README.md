# DevSuperior - Java Spring Professional

## Desafio 02 - Modelo de domínio e ORM
Neste desafio trabalhamos conceitos de como trabalhar com o JPA/Hibernate para mapear as tabelas descritas no desafio.

O que utilizamos no backend:
- Java
- Framework Spring Boot

O desafio consiste em usar os conceitos de JPA com Hibernate para criar no banco de dados as tabelas requisitadas bem como suas relações.

As entidades/tabelas criadas foram:
- Atividade
- Categoria
- Participante
- Bloco

As relaçoes entre as tabelas:
- Atividade e Categoria - relação **muitos para um**
- Atividade e Bloco - relaçao **muitos para um**
- Atividade e Participante - relação **muitos para muitos**

As relações de **muitos para um** acabam refletindo em uma coluna a mais em uma das tabelas da relação.

A relação de **muitos para muitos** foi implementada com uma tabela adicional de mapeamento da associação.

Também foi criado um arquivo de seed para o banco de dados H2: `src/main/resources/import.sql`

## Como executar
Clonar este repositório, importar na IDE de preferência e executar a classe principal `Dsjsp02Application`.

O banco de dados H2 poderá ser consultado pelo client web do H2 no [link](http://localhost:8080/h2-console) e os dados de conexão ao banco H2 estão no arquivo `src/main/resources/application-test.properties`.