## Requisitos Funcionais

1. **Cadastro**
   - O sistema deve permitir o cadastro de novos usuários.
   - O sistema deve validar as informações de cadastro: nome completo, CPF, e-mail, senha e confirmação de senha.
   - A tela de cadastro deve conter os seguintes elementos:

     | Campo            | Tipo   |
     |------------------|--------|
     | Nome Completo    | Texto  |
     | CPF              | Texto  |
     | E-mail           | Texto  |
     | Senha            | Senha  |
     | Confirmar Senha  | Senha  |
     | Botão Cadastrar  | Botão  |

2. **Login**
   - O sistema deve permitir que os usuários façam login usando suas credenciais (e-mail e senha).
   - O sistema deve verificar a autenticidade das credenciais fornecidas.
   - A tela de login deve conter os seguintes elementos:

     | Campo            | Tipo   |
     |------------------|--------|
     | E-mail           | Texto  |
     | Senha            | Senha  |
     | Botão Entrar     | Botão  |
     | Label Cadastro   | Link   |

   - O sistema deve permitir a recuperação de senha.

3. **Painel Principal**
   - O sistema deve exibir a logo da empresa no canto superior direito em todas as telas.
   - O menu principal deve estar localizado na lateral esquerda, contendo os seguintes módulos:

     | Módulo       | Ação                                               |
     |--------------|----------------------------------------------------|
     | Home         | Redireciona para a página inicial                  |
     | Disponíveis  | Exibe a lista de livros disponíveis para locação   |
     | Locar        | Redireciona para a página de locação de livros     |
     | Locados      | Exibe a lista de livros locados                    |
     | Histórico    | Exibe o histórico de locações                      |
     | Sair         | Realiza logout do sistema                          |

   - A label do menu ativo deve ficar em laranja.

4. **Menu Disponíveis**
   - O sistema deve exibir uma lista de livros disponíveis para locação, separados por tópicos.
   - A tela deve conter uma scrollbar no canto direito para navegação.
   - O sistema deve exibir informações de cada livro:

     | Informação    | Descrição             |
     |---------------|-----------------------|
     | Título        | Texto                 |
     | Autor         | Texto                 |
     | Avaliação     | Numérico (0 a 5)      |

   - Deve haver um campo de pesquisa para filtrar os livros.
   - Deve haver um botão de atalho "Locar" no canto inferior direito, que redireciona para o menu Locar.

5. **Pesquisa de Livros**
   - O sistema deve permitir a pesquisa de livros por:

     | Critério  | Tipo  |
     |-----------|-------|
     | Título    | Texto |
     | Autor     | Texto |
     | Categoria | Texto |

   - Os resultados da pesquisa devem ser exibidos de forma clara e organizada.

6. **Locação de Livros**
   - O sistema deve permitir que o usuário selecione um livro para alugar.
   - No menu Locar, deve haver um campo de pesquisa para selecionar o livro.
   - O livro selecionado deve aparecer em um frame abaixo com a capa e informações.
   - O sistema deve permitir que o usuário escolha a data de devolução do livro, automaticamente definida para dois meses a partir da data de locação.
   - O sistema deve registrar:

     | Informação                | Descrição                    |
     |---------------------------|------------------------------|
     | Data de Locação           | Data atual                   |
     | Data Prevista Devolução   | Data dois meses após locação |

7. **Locados**
   - O sistema deve exibir as informações dos livros locados, incluindo:

     | Informação            | Descrição                  |
     |-----------------------|----------------------------|
     | Nome do Livro         | Texto                      |
     | Prazo para Devolução  | Data                       |
     | Nome do Cliente       | Texto                      |

8. **Histórico de Locações**
   - O sistema deve exibir o histórico de livros locados pelo usuário, incluindo:

     | Informação            | Descrição                  |
     |-----------------------|----------------------------|
     | Nome do Livro         | Texto                      |
     | Data de Locação       | Data                       |
     | Data de Devolução     | Data                       |
     | Status                | Pendente (azul), Devolvido (verde), Em Atraso (vermelho) |

   - A tela deve conter uma scrollbar no canto direito para navegação, se necessário.

