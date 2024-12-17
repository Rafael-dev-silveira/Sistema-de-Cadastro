Sistema de Cadastro com Python e Django
=

Este projeto consiste em um Sistema de Cadastro de Usuários desenvolvido com Python e o framework Django. Ele permite que o usuário insira nome e idade por meio de um formulário simples, enviando esses dados a um servidor. Os dados são armazenados em um banco de dados relacional (SQLite por padrão) e exibidos em uma lista como resposta.

Funcionalidades Principais:
Interface Front-end:
=

Um formulário HTML com dois campos de entrada: nome e idade.
Um botão de envio para enviar os dados ao servidor.

Back-end com Django:
=

Models: Um modelo é definido para representar os usuários no banco de dados, com campos para nome (texto) e idade (inteiro).

Views:
Recebe os dados enviados pelo formulário.
Salva os dados no banco de dados.
Recupera a lista completa de usuários armazenados e envia essa lista de volta ao template.

URLs: Roteamento de requisições do formulário e exibição da lista de usuários.

Templates: Uso de HTML renderizado pelo Django para exibir o formulário e a lista de usuários.

Banco de Dados:
=

Armazena os dados dos usuários cadastrados.
Utiliza SQLite como banco padrão, que pode ser facilmente substituído por outros bancos como PostgreSQL ou MySQL.

Fluxo do Projeto:
=
O usuário acessa a página inicial, onde encontra um formulário com os campos nome e idade.
Após preencher os campos e clicar no botão de envio, os dados são enviados ao servidor Django.

O servidor:
=
Salva os dados no banco de dados.
Recupera todos os registros armazenados.
O servidor retorna ao usuário uma lista de registros, que aparece logo abaixo do formulário.

Tecnologias Utilizadas:
=
Linguagem: Python

Framework: Django

Banco de Dados: SQLite

Servidor: Django Development Server (para desenvolvimento local)

Resultado Final:
=
O sistema fornece uma experiência simples e funcional para cadastrar usuários, permitindo que os dados sejam persistidos em um banco de dados e visualizados em tempo real através de uma lista atualizada.
