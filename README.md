## LISTA COM O LINK DOS PORTFÓLIOS DOS APIs:
[API 1° SEMESTRE - **DANZO - Mapa de Criminalidade ao Redor da FATEC**](https://github.com/ZVIEWIL/portifolio1) 

[API 2° SEMESTRE - **GANTT CHART**](https://github.com/ZVIEWIL/portifolio2)

[API 3° SEMESTRE - **CADASTRO POSITIVO**](https://github.com/ZVIEWIL/portifolio3)

# API do 2° SEMESTRE - ***FATEC & NECTO - GANTT CHART***

### **RESUMO DO PROJETO**
No segundo API a FATEC trouxe o cliente NECTO com um problema a ser resolvido. O cliente buscava uma solução para gerenciar seus projetos e colaboradores, a aplicação deveria possibilitar a alocação dos recursos humanos em um gráfico de GANTT (tarefas em linhas de tempo), gerando métricas sobre a ocupação e o tempo disponível da equipe para novos projetos e contingências. 

Desenvolvemos uma API Desktop que atendeu os seguintes requisitos do cliente:
- Cadastro de Usuários: Para utilizar o sistema é necessário estar cadastrado (Usuário e Senha).
- Cadastro de Colaboradores: O sistema permite a inserção de colaboradores.
- Cadastro de Tarefas: O sistema permite inserir novos projetos e tarefas relacionando colaboradores a elas.
- Quantidade Total de Horas por Projeto: O sistema mostra a quantidade de horas alocados em cada projeto.
- Quantidade Total de Horas por Funcionário: O sistema mostra a quantidade total de horas/mês alocada por funcionário.
- Diagrama Interativo: 	O sistema gera gráficos de Gantt responsivos que ao ter a barra arrastada e depois de clicado em "salvar", refazia o calculo total de horas do projeto, total de horas das tarefa e total de horas acumuladas dos colaboradores.

Tela de Login:

![Login](https://user-images.githubusercontent.com/61089745/141656980-681987ac-1e9d-4fe9-bceb-9d83434fb975.PNG)

Tela Inicial:

![Screenshot_1](https://user-images.githubusercontent.com/54503903/142918543-6449732c-71cd-4f7d-ad51-8f8a6923cc03.png)

Tela de Cadastro de Projetos:

![CadastroProjetosII](https://user-images.githubusercontent.com/61089745/141657004-75236913-3a62-4006-990a-4f89f0475a45.PNG)

Tela de cadastro de Funcionários:

![CadastroFuncionarios](https://user-images.githubusercontent.com/61089745/141657014-8a8603a8-4cef-4aad-8837-1d5aa535aebd.PNG)

Tela de Cadastro da Tarefas:

![Screenshot_4](https://user-images.githubusercontent.com/54503903/142921705-dd120424-ecc4-4f22-a98c-2e894d0b7956.png)

Tela de Visualização das Tarefas com barras responsivas e opção de salvar a alteração:

![Screenshot_2](https://user-images.githubusercontent.com/54503903/142921293-0a2faf2e-959a-4585-bfdf-57be1982e232.png)
![Screenshot_3](https://user-images.githubusercontent.com/54503903/142921627-716dd9fb-6270-45a8-b3f7-567944a5eda0.png)

### **TECNOLOGIAS UTILIZADAS**
#### **JAVA**
![Screenshot_5](https://user-images.githubusercontent.com/54503903/142946345-bcb779b8-0c4e-4634-83cb-7325b56d761b.png)

Pensando em diminuir nossa curva de aprendizado, utilizamos a Linguagem Java que estava sendo introduzida em algumas disciplinas durante o semestre. A linguagem Java é orientada a objetos e possui muitos frameworks e bibliotecas. Utilizamos ela para desenvolver o nosso back-end.

Bibliotecas utilizadas:

-JavaFx: É uma biblioteca para desenvolvimento de programas com interfaces gráficas em Java. Optamos por utilizá-la devido ao pouco conhecimento que os integrantes do grupo tinham com o Java, estavamos com dificuldade em integrar o back end em java com o front em html. Hoje em dia olhando para trás penso que a alternativa não foi tão assertiva, pois cada vez menos vemos aplicações desktop sendo utilizadas em clientes final.

-Nebula: É uma biblioteca do Eclipse utilizada para desenvolver vários gadgets em aplicações. Encontramos ela durante as pesquisas que realizamos para desenvolver o gráfico de Gantt com a possibilidade de fazer Drag and Drop nas tarefas. 

#### **MYSQL**
![Screenshot_6](https://user-images.githubusercontent.com/54503903/142946420-93441f77-23d9-41e2-aa16-007b24d0b993.png)

Pensando da mesma forma que a tecnologia anterior, utilizamos o Banco de Dados MySql + Interface Gráfica WorkBench que também estavam sendo introduzidos na Disciplina de Arquitetura e Modelagem de Banco de Dados. Utilizamos o WorkBench para criar as Tabelas e Entidades do Nosso Banco Relacional.


#### **ECLIPSE**
![Screenshot_7](https://user-images.githubusercontent.com/54503903/142947249-51232914-04a4-413e-9821-1a520e37dd26.png)

IDE utilizada para desenvolver aplicações em Java. Utilizamos ela para desenvolver nossa aplicação.

### **CONTRIBUIÇÕES INDIVIDUAIS**
Fiz a integração do back end com a lib Nebula, foi uma tarefa bastante desafiadora, pois a quantidade de tarefas e projetos a serem inseridos no gráfico varia de acordo com o que é criado ou deletado. Para criar a classe que constrói o gráfico utilizei vetores, estruturas de repetição (For), estrutura condicional (If/Else) e conversões de variáveis (String para Date).

![Screenshot_8](https://user-images.githubusercontent.com/54503903/142952014-18f629eb-8777-44a1-87f5-c8f83ac1f8a2.png)

Dentro da classe que constrói o gráfico, criei o método para salvar as alterações feitas pelo usuário através do "drag and drop" do gráfico no banco de dados.

![Screenshot_9](https://user-images.githubusercontent.com/54503903/142952433-ee27ebf5-5c4d-4c86-b5c9-8b49106a815f.png)

Classe criada para exibir o gráfico:

![Screenshot_10](https://user-images.githubusercontent.com/54503903/142953172-d50d0ece-9c7c-471a-9476-df17abdabf01.png)

### **APRENDIZADOS EFETIVOS**

- Desenvolvi pela primeira vez uma aplicação em JAVA, aprendi a criar classes, métodos, usar vetores, estruturas de repetição, estruturas condicionais, importar bibliotecas, integrar o banco de dados com o back end e desenvolver uma aplicação desktop. Aprendi sobre as camadas utilizadas no processo de desenvolvimento (Entidade, Service, Service implements, DAO e Controller). A partir disso consegui compreender com mais clareza os conceitos de Arquitetura de Software;
- Aprendi a modelar banco de dados pelo WorkBench (Model) e criar tabelas(Comandos DDL), Aprendi a inserir, atualizar e deletar dados (Comandos DML), aprendi a fazer o CRUD de uma aplicação;
- Aprendi a configurar o Ambiente para uma aplicação Gradle e utilizar a IDE Eclipse (exportar e importar);
- Conheci e utilizei o GitHub.
- Aprendi a Utilizar uma biblioteca especifica para criar o Gráfico de Gantt, realizar testes a partir da leitura da documentação e que é possível adaptar o código de acordo com nossa necessidade.
- Aprendemos como funciona o desenvolvimento de uma aplicação na prática, tratando diretamente com o cliente, entendendo melhor sobre requisitos, desenvolvimento ágil e como agregar valor nas entregas das sprints.
- Devido a pandemia, acabamos aprendendo a trabalhar remotamente, nos comunicando pelo TEAMS, realizando as apresentações das sprints através de vídeos gravados realizando conferências para tirar dúvidas.

