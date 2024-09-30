## Sistema de Gerenciamento de Biblioteca
Banco de Dados em MongoDB

### Instruções
Você foi contratado para desenvolver um sistema de gerenciamento para uma biblioteca. O sistema deve gerenciar não apenas seus livros e autores, mas também usuários, empréstimos e categorias de livros.

### Requisitos do Sistema

#### Coleção de Livros:
Cada livro deve ter os seguintes atributos:

- _id: (gerado automaticamente pelo MongoDB)
- titulo: Título do livro
- autor_id: ID do autor (referência)
- categoria_id: ID da categoria (referência)
- isbn: Código ISBN do livro
- quantidade_estoque: (inteiro) Quantidade disponível na biblioteca
- data_publicacao: Data de publicação do livro

#### Coleção de Autores:
Cada autor deve ter os seguintes atributos:

- _id: (gerado automaticamente pelo MongoDB)
- nome: Nome do autor
- nacionalidade: Nacionalidade do autor
- data_nascimento: Data de nascimento do autor
- livros_publicados: (array) Lista de IDs de livros publicados pelo autor

#### Coleção de Categorias:
Cada categoria deve ter os seguintes atributos:

- _id: (gerado automaticamente pelo MongoDB)
- nome: Nome da categoria
- descricao: Descrição da categoria

#### Coleção de Usuários:
Cada usuário deve ter os seguintes atributos:

- _id: (gerado automaticamente pelo MongoDB)
- nome: Nome do usuário
- email: Endereço de e-mail do usuário
- data_cadastro: Data de cadastro do usuário
- livros_emprestados: (array de IDs de empréstimos) Lista de IDs de empréstimos realizados pelo usuário

#### Coleção de Empréstimos:
Cada empréstimo deve conter:

- _id: (gerado automaticamente pelo MongoDB)
- livro_id: ID do livro (referência)
- usuario_id: ID do usuário (referência)
- data_emprestimo: Data em que o livro foi emprestado
- data_devolucao: Data em que o livro deve ser devolvido
- status: (string: "ativo", "devolvido") Status do empréstimo

#### Tarefas
Modelo de Dados: Desenhe um modelo de dados que represente as coleções e seus relacionamentos.

#### Configuração do Banco de Dados:

1. Crie um banco de dados chamado biblioteca.
2. Crie as coleções livros, autores, categorias, usuarios e emprestimos.
3. População do Banco de Dados: Insira pelo menos 5 documentos em cada coleção, utilizando dados fictícios.

#### Consultas: Crie e execute as seguintes consultas:

1. Liste todos os livros disponíveis na biblioteca (quantidade_estoque > 0).
2. Encontre todos os livros de um autor específico.
3. Liste todos os usuários e quantos livros cada um já emprestou.
4. Liste todos os empréstimos ativos e os respectivos usuários e livros.
6. Encontre todas as categorias que possuem mais de 3 livros associados.

![image](https://github.com/user-attachments/assets/382321ab-80e6-4b4b-9a57-5784e8683ea2)

