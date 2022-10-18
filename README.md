# Rebisyon Backend

REST API made in Go from the open source spaced repetition program Rebisyon.

# Arquitetura e tecnologias

O Rebisyon Backend será uma API REST open source feita em Go para que os usuários possam utilizar suas funcionalidades a partir de diferentes tipos interface, como uma interface web e/ou mobile.

A documentação das rotas será feita utilizando o Swagger.

Neste backend será utilizada a Arquitetura Hexagonal (ou de Portas e Adaptadores) afim de garantir o máximo desacoplamento do sistema.

O sistema de gerenciamento de banco de dados (SGBD) utilizado será o PostgreSQL, pois um SGBD relacional parece ser adequado para este projeto.

Também utilizaremos o docker para que quem for ajudar a desenvolver este backend não precise se preocupar com a instalação de várias ferramentas.

# Mini-mundo

O Rebisyon é um sistema que pretende facilitar a memorização e a aprendizagem de qualquer coisa (especialmente de coisas teóricas).

Inicialmente, o sistema pretende permitir a criação de flashcards apenas com textos, nos quais, na “frente” do cartão, haverá uma pergunta e, no “verso” do cartão, haverá a sua resposta. O sistema deve permitir que o usuário crie um baralho para armazenar seus cartões, para que ele possa deixar as coisas mais organizadas. Quando o usuário quiser revisar seus cartões, ele deve escolher um baralho e começar a revisar os cartões desse baralho. Durante a revisão, o usuário deve ler a pergunta de um cartão, pensar na resposta, pedir para o sistema mostrar a resposta, verificar se ele (o usuário) acertou a resposta. Caso tenha acertado, ele deve informar isso ao sistema. Caso tenha errado, ele também deve informar isso ao sistema. Dependendo do feedback do usuário (se ele acertou ou errou), o sistema deve calcular quando o usuário deve revisar aquele flashcard novamente (inicialmente, caso ele tenha acertado, só deve revisá-lo novamente amanhã, mas caso tenha errado, dede revisá-lo novamente ainda hoje).
