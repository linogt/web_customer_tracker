# web_customer_tracker


## Sobre o projeto

Projeto proposto pelo professor Chad Darby dedicado a criação de uma página web que cumpra as funções de inserção, remoção e atualização de usuários de um banco de dados utilizando as tecnologias Spring MVC, Hibernate e MySQL WorkBench.

## Tecnologias Utilizadas

* Java
* SQL
* MySQL WorkBench
* Eclipse IDE
* Spring MVC
* Hibernate

## Mapa do Projeto 

Customer Controller -> Customer Service -> Customer DAO -> DataBase

## Processo

### 1º Etapa -  Criação da Tabela Usuários

Nessa etapa acontece a criação e população da tabela Usuários por meio do MySQL WorkBench. Os Atributos escolhidos foram ID, nome, sobrenome e email.

![tabelausua](https://user-images.githubusercontent.com/75547468/213825797-f1028bae-7044-4cf0-8acd-a0282e035531.png)

### 2º Etapa - Configuração do Spring + Hibernate

Nessa etapa ocorre a configuração do Spring + Hibernate no arquivo xml, definindo a conexão com o banco de dados e criando o bean 
"session factory" e "transaction manager" que serão responsáveis por fazer a conexão do banco de dados com as outras classes. 

### 3º Etapa - Criação da Classe Customer (Cliente)

Está etapa consiste na criação da Classe Cliente, onde iremos converter a tabela criada no banco de dados em uma classe Java seguindo a ordem:

* Atributos
* Getters/Setters
* toString
* Anotações

As anotações servem para definir os elementos correspondentes na tabela.

![classe cliente](https://user-images.githubusercontent.com/75547468/213828140-abeef581-0a32-46c1-9cf3-c3ecbdf6fe45.png)

### 4º Etapa - Criação da Interface CustomerDAO e a Classe de implementação 

A classe CustomerDAO (Cliente DAO) é utilizada para fazer a conexão do banco de dados com a classe Service.

### 5º Etapa - Criação da classe Controller

A classe Controller é utilizada para fazer a conexão entre a interface web com a classe Service.

### 6º Etapa - Criação da classe Service 

A classe service é utilizada para fazer a conexão entre a classe Controller e a classe DAO.

### 6º Etapa - Função Adicionar Cliente

* Adicionar Botão "Adicionar Cliente" no HTML
* Implementar a classe Controller com o método showFormForAdd
* Implementar a classe Service com o método salvar cliente
* Implementar a classe DAO com o método salvar cliente

### 7º Etapa - Função Atualizar Cliente

* Adicionar Botão "Atualizar Cliente" no HTML
* Implementar a classe Controller com o método showFormForUpdate
* Implementar a classe Service com o método get cliente
* Implementar a classe DAO com o método get cliente
* Refatorar o método salvar cliente para ter a opção de atualizar.

### 8º Etapa - Função Deletar Cliente 

* Adicionar Botão "Deletar Cliente" no HTML e o aviso para quando ocorrer uma remoção de cliente
* Implementar a classe Controller com o método deleteCustomer
* Implementar a classe Service com o método delete cliente
* Implementar a classe DAO com o método delete cliente

## Resultado em imagens

![int](https://user-images.githubusercontent.com/75547468/213869114-0a4bc353-3379-46b6-8cdd-32a31964a8d0.png)

![int](https://user-images.githubusercontent.com/75547468/213869168-89521a4b-2ce1-44e5-8eb7-8d1f5620d481.png)


## Resultado em vídeo


https://user-images.githubusercontent.com/75547468/213828726-f23a38b8-d131-43d1-b3c8-f034da510790.mp4



## Autor

Gabriel Lino Topa Garcia



