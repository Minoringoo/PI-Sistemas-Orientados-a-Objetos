# DESENVOLVIMENTO DE SISTEMAS ORIENTADO A OBJETOS
O presente trabalho visa modelar os diagramas de casos de uso e o diagrama de classes, a fim de representar com base nos conceitos e fundamentos da UML o cadastro de diferentes tipos de pessoas em um sistema de gestão para o Centro Universitário Estuda com Fé Que Passa (Fictício).

## INTEGRANTES
Daiane Dias Alves

João Carlos Barbosa de Alcantara

Jonathan Bandeira de Souza

Tiago Minoru Gomes Miura

## INTRODUÇÃO
A Linguagem de Modelagem Unificada (sigla: UML; do inglês: Unified Modeling Language) nasceu em 1997, em razão da unificação dos métodos orientados a objeto de Booch, de Rumbaugh (método OOSE - Object-Oriented Software Engineering) e o método OMT (Object Modeling Technique) de Jacobson. Sendo estes três, os métodos mais populares em meados da década 1990. Posteriormente a UML foi adotada como padrão pelo Grupo de Gerenciamento de Objetos (sigla: OMG; do inglês: Object Management Group), um consórcio internacional de empresas que define e ratifica padrões na área de orientação a objetos (Fowler, 2004; Pereira, 2011).

Desde então, a UML é utilizada por profissionais da indústria de softwares para nortear a elaboração da estrutura de projetos de software e especificação de sistemas computacionais. No entanto, deve-se observar que a UML não é uma linguagem de programação, trata-se na verdade de um conjunto de notações gráficas, apoiada por um metamodelo que permite representar um sistema de forma padronizada, a fim de facilitar sua compreensão e transmitir aspectos de sua pré-implementação. Ao prover uma descrição visual o UML auxilia os desenvolvedores a definirem características como requisitos, comportamento, estrutura lógica, a dinâmica de processos e até mesmo as necessidades físicas em relação ao hardware, principalmente em sistemas projetados sobre o paradigma orientado a objetos (POO) (Fowler, 2004; Larman, 2007; Pereira, 2011, Guedes, 2018).

## DIAGRAMAS DE CASOS DE USOS
O diagrama de casos de uso apresenta uma visão geral das funcionalidades que o sistema pretende oferecer aos usuários. Ele descreve em alto nível o escopo do sistema e permite representar através de uma linguagem simples e de fácil entendimento os diferentes tipos de funções e interações para que os usuários possam ter uma ideia de como o sistema vai se comportar (Fowler, 2004; Guedes, 2018). A figura 1 apresenta o diagrama de casos de uso desenvolvido para o Centro Universitário Estuda Com Fé Que Passa (EFQP).

![diagrama_casos_de_uso](https://github.com/Minoringoo/PI-Sistemas-Orientados-a-Objetos/blob/main/Diagrama%20de%20casos%20de%20uso.png)
**Figura 1 – Diagrama de Casos de Uso:  sistema de gestão EFQP. Fonte: autores.**

## DIAGRAMA DE CLASSES
O diagrama de classes permite a visualização da parte estrutural do sistema, ou seja, de suas classes, seus atributos, métodos e os relacionamentos, auxiliando na comunicação entre a equipe de desenvolvimento e permitindo uma representação visual estática do sistema. (Pereira, 2011; Guedes 2018). Veja na figura 2 a representação gráfica do diagrama de classes de uso desenvolvido para o EFQP.

![diagrama_de_classes](https://github.com/Minoringoo/PI-Sistemas-Orientados-a-Objetos/blob/main/diagrama%20de%20classes.png)
**Figura 2 – Diagrama de Classes:  sistema de gestão EFQP. Fonte: autores.**

## DESCRIÇÃO DOS CENÁRIOS

### Caso de uso 1 - Acessar o portal:

**➢	Cenário Principal:** O usuário está na tela principal do sistema da universidade devidamente logado e tem acesso a sua página do portal.

*	**Pré-condição:** O usuário, não está em seu portal de acesso.
*	**Pós-condição:** O usuário está logado visualizando sua página no portal, com seus avisos e menu.

**➢	Cenário alternativo 1:** O usuário erra seus dados cadastrais e não acessa o portal, o site informa senha/usuário invalido, tente novamente.

* **Pré-condição:** O usuário está no portal, mas não está na sua tela de acesso.
* **Pós-condição:** O sistema solicita verificar seus dados e tente novamente.

**➢	Cenário alternativo 2:** O usuário acessa o sistema sem sucesso por erro transmissão de dados da universidade.

* **Pré-condição:** O usuário não tem acesso a sua página no portal.
* **Pós-Condição:** O usuário ainda não tem acesso seu portal, o site solicita que tente novamente, ou contate o suporte.

### Caso de Uso 2 – Visualizar avisos

**➢	Cenário Principal:** O aluno acessa sua área no portal da universidade e possui a área “avisos”. Ao clicar o aluno é direcionado aos principais avisos da universidade referente ao seu curso, onde os não lidos aparecerão em negrito.
 
* **Pré-condição:** O usuário está em sua tela do portal, logado e visualizando seus avisos.

* **Pós-condição:** O sistema mostra seus avisos, com a referente data e com a opção de expansão do aviso ao clicar.

**➢	Cenário alternativo 1:** O usuário acessa seus avisos, porém não há novos avisos a serem lidos.

*	**Pré-condição:** O usuário está em sua tela de acesso do portal.

*	**Pós-condição:** O sistema mostra os avisos, porém não há avisos em negrito

**➢	Cenário alternativo 2:** O usuário tenta acessar seus avisos, porém recebe mensagem de erro do sistema com “tente novamente”.

* **Pré-condição:** O usuário está em sua tela de acesso ao portal.

* **Pós-Condição:** O sistema informa uma mensagem de “tente novamente mais tarde”.

### Caso de uso 3 - Visualizar turma

**➢	Cenário Principal:** O aluno acessa sua área no portal da universidade e possui a área
“visualizar turma”.

* **Pré-condição:** O usuário está em sua tela do portal, logado e visualizando sua turma.

*	**Pós-condição:** O sistema mostra sua turma.

**➢	Cenário alternativo 1:** O usuário acessa seu portal, porém não está em uma turma.

* **Pré-condição:** O usuário está em sua tela de acesso do portal.

* **Pós-condição:** O sistema informa “você não está cadastrado em uma turma”.
 
**➢	Cenário alternativo 2:** O usuário está em seu portal, e o sistema informa que não está cadastrado em uma turma.

* **Pré-condição** O usuário está em sua tela de acesso ao portal.

* **Pós-Condição:** O sistema informa uma mensagem de “entre em contato com o professor”.

### Caso de Uso 4 - Enviar mensagem

**➢	Cenário Principal:** O usuário acessa sua área no portal da universidade, na matéria escolhida, possui o link “Enviar mensagem”. Ao clicar o usuário é direcionado a página com campo para escrever a mensagem.

* **Pré-condição:** O usuário está em sua tela do portal, na área de envio de mensagem.

* **Pós-condição:** O sistema mostra o campo para escrever a mensagem com campo de escolha endereço de e-mail do aluno/professor e campo de escolha de temas da mensagem

**➢	Cenário alternativo 1:** O usuário acessa a tela de envio de mensagem, porém não há e-mail no campo “Para:”.

* **Pré-condição:** O usuário está em sua tela de acesso do portal.

* **Pós-condição:** O sistema indica “Sem destinatário válido”.

**➢	Cenário alternativo 2:** O usuário tenta enviar sua mensagem, porém não consegue enviar a mensagem.

* **Pré-condição:** O usuário está em sua tela de acesso ao portal.

* **Pós-Condição:** O sistema informa uma mensagem de “indique um assunto”.
 
### Caso de uso 5 - Visualizar calendário acadêmico

**➢	Cenário Principal:** O usuário acessa sua área no portal da universidade e possui a área
“visualizar calendário acadêmico”.

* **Pré-condição:** O usuário está em sua tela do portal, logado e visualizando seu calendário

* **Pós-condição:** O sistema mostra seu calendário.

**➢	Cenário alternativo 1:** O usuário acessa seu portal, porém não está visualizando o calendário.

* **Pré-condição:** O usuário está em sua tela de acesso do portal.

* **Pós-condição:** O sistema informa “você não está cadastrado em um curso”.

**➢	Cenário alternativo 2:** O usuário está em seu portal, e o sistema informa que não está cadastrado em um curso.

* **Pré-condição:** O usuário está em sua tela de acesso ao portal.

* **Pós-Condição:** O sistema informa uma mensagem de “entre em contato com a secretaria”.

### Caso de uso 6 – Visualizar material da disciplina

**➢	Cenário Principal:** O aluno acessa sua área no portal da universidade e possui a área
“disciplinas”. Ao escolher ao acessar a disciplina escolhida, possui a opção “Material da disciplina”.

* **Pré-condição:** O usuário está em sua tela do portal, logado e visualizando suas disciplinas.

* **Pós-condição:** O sistema mostra suas disciplinas para efetuar as escolhas.

**➢	Cenário alternativo 1:** O usuário acessa seu portal, porém não possui material para a disciplina.

* **Pré-condição:** O usuário está em sua tela de acesso do portal.

* **Pós-condição:** O sistema informa “não há registro de material da disciplina”.

**➢	Cenário alternativo 2:** O usuário está em seu portal, e o sistema informa que não há Registro de material salvo na disciplina.

* **Pré-condição:** O usuário está em sua tela de acesso ao portal.

* **Pós-Condição:** O sistema informa uma mensagem de “entre em contato com o professor”.

### Caso de uso 7– Visualizar nota:

**➢	Cenário principal:** o aluno acessa o seu portal, onde possui “Visualizar Notas”. Ao clicar o aluno é direcionado a página com suas notas com suas respectivas disciplinas.

* **Pré-condição:** o usuário acessa o site da universidade e está em sua área do portal

* **Pós-condição:** o sistema mostra uma página com suas disciplinas e notas finais.

**➢	Cenário alternativo 1:** o usuário acessar a área das notas das disciplinas, porém ainda não há avaliação cadastrada.

* **Pré-condição:** o usuário acessa o site da universidade e está em sua área do portal.

* **Pós-condição:** o sistema informa “não há registros notas registradas”, caso haja um erro “entre em contato com a secretaria”.

**➢	Cenário alternativo 2:** o usuário tenta acessar o portal, mas o sistema não responde a solicitação.

* **Pré-condição:** o usuário acessa o site da universidade e está em sua área do portal.

* **Pós-condição:** o sistema informa “tente novamente mais tarde”.

## CONCLUSÃO
Os diagramas UML de casos de uso e de classes são de fundamental importância para o processo de desenvolvimento de software porque permitem aos profissionais visualizarem e compreenderem melhor o sistema que estão criando. O primeiro (casos de uso) permite que sejam identificados e definidos os requisitos e as funcionalidades que os sistemas deverão apresentar, enquanto o segundo (classes) auxilia na modelagem estrutural, apresentado as classes que constituem o sistema e como elas interagem entre si. Além disso, os diagramas proporcionam que o projeto seja bem documentado, que esteja de acordo com o que foi solicitado e que atenda às necessidades dos usuários, bem como facilita futuras manutenções e implementações (atualizações).

## REFERÊNCIAS


Fowler, Martin. **UML Essencial: Um Breve Guia para a Linguagem-Padrão de Modelagem de Objetos** – 3ª ed. Bookman, 2004.

Guedes, Gilleanes. **UML2: Uma abordagem prática**. 3ª ed. São Paulo: Novatec, 2018. 496 p.

Larman, Craig. **Utilizando UML e Padrões: Uma Introdução à Análise e ao Projeto Orientados a Objetos** – 3ª ed. Bookman, 2007.

Pereia, Luiz. **Análise e Modelagem de Sistemas com a UML**: Com Dicas e Exercícios
Resolvidos. 1ª ed. Rio de Janeiro: Edição do Autor, 2011.
