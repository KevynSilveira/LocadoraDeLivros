# Camadas da Arquitetura

1. **Camada de Apresentação (Frontend)**
2. **Camada de Aplicação (Backend)**
3. **Camada de Dados (Banco de Dados)**
4. **Camada de Segurança**
5. **Camada de Infraestrutura**

---

## Descrição Detalhada dos Componentes

### 1. Camada de Apresentação (Frontend)

#### Componentes:

- **Interface de Usuário (UI):**
  - Implementada em HTML, CSS e JavaScript.
  - Frameworks como React, Angular ou Vue.js podem ser usados.
  - Segue diretrizes de acessibilidade WCAG 2.1.
- **Gerenciamento de Sessão:**
  - Lida com a manutenção de sessões de usuário.
  - Usa cookies e tokens JWT (JSON Web Tokens) para autenticação.
- **Módulo de Feedback:**
  - Proporciona feedback em tempo real.
  - Exibe mensagens de sucesso, erro ou informações.

#### Fluxos de Dados:

- Usuário -> Interface de Usuário (UI): Interações do usuário (cadastro, login, pesquisa, locação).
- Interface de Usuário (UI) -> Backend (APIs REST): Requisições de operação.

### 2. Camada de Aplicação (Backend)

#### Componentes:

- **Controladores (Controllers):**
  - Implementam endpoints de API.
  - Processam requisições do frontend.
- **Serviço de Autenticação:**
  - Gerencia login e recuperação de senha.
  - Valida credenciais de usuário.
- **Serviço de Controle de Acesso (RBAC):**
  - Gerencia permissões baseadas em funções de usuário.
- **Serviço de Criptografia:**
  - Criptografa senhas e outros dados sensíveis.
  - Usa algoritmos robustos como bcrypt.
- **Serviço de Locação de Livros:**
  - Gerencia a locação e a devolução de livros.
- **Serviço de Pesquisa:**
  - Executa consultas de pesquisa de livros.
- **Serviço de Histórico de Locação:**
  - Recupera e gerencia o histórico de locações dos usuários.

#### Tecnologias:

- Frameworks de desenvolvimento web - Node.js com Express.

#### Fluxos de Dados:

- Frontend -> Controladores: Envio de requisições (dados de cadastro/login, termos de pesquisa, pedidos de locação).
- Controladores -> Serviços Backend: Invocação de lógica de negócios.
- Serviços Backend -> Banco de Dados: Realizam operações de leitura/escrita no banco de dados.

### 3. Camada de Dados (Banco de Dados)

#### Componentes:

- **Tabela de Usuários:**
  - Armazena informações dos usuários (nome, CPF, e-mail, senha criptografada).
- **Tabela de Livros:**
  - Armazena informações dos livros (título, autor, tópico, capa, disponibilidade).
- **Tabela de Locação:**
  - Armazena informações de locação de livros (usuário, livro, data de locação, data de devolução).
- **Tabela de Histórico:**
  - Armazena o histórico de locações (usuário, livro, data de locação e devolução).

#### Tecnologias:

- Banco de dados relacional como MySQL ou PostgreSQL.

### 4. Camada de Segurança

#### Componentes:

- **Criptografia:**
  - Senhas criptografadas usando bcrypt.
- **Controle de Acesso (RBAC):**
  - Implementação de níveis de acesso para diferentes funções de usuário.
- **Proteção contra Ataques:**
  - Middleware para prevenção de SQL Injection, XSS e CSRF.
  - Implementação de CORS (Cross-Origin Resource Sharing).

#### Tecnologias:

- Bibliotecas de segurança e criptografia, como bcrypt, helmet (para Express), etc.

### 5. Camada de Infraestrutura

#### Componentes:

- **Servidores:**
  - Servidores web e de aplicação.
  - Balanceadores de carga para distribuir requisições.
- **Backup e Recuperação:**
  - Mecanismos automáticos de backup e recuperação de dados.
- **Monitoramento e Logging:**
  - Ferramentas de monitoramento de desempenho e logs de aplicação.

#### Tecnologias:

- Servidores Nginx ou Apache.
- Ferramentas de CI/CD como Jenkins.
- Sistemas de monitoramento como Prometheus e Grafana.
