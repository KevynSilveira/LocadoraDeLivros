# Regras de Negócio

## Cadastro de Usuários

- Um usuário deve fornecer um e-mail único e válido, CPF válido, e uma senha que atenda aos requisitos mínimos de segurança.
- Senhas devem ser confirmadas antes de serem aceitas.

## Autenticação

- O sistema deve bloquear a conta do usuário após três tentativas de login falhadas consecutivas, enviando um e-mail com instruções para desbloqueio.

## Locação de Livros

- Um usuário pode alugar um máximo de 5 livros simultaneamente.
- A data de devolução padrão é dois meses a partir da data de locação, podendo ser alterada pelo administrador.

## Renovação de Locação

- Usuários podem solicitar a renovação da locação por mais um mês, desde que o livro não tenha sido reservado por outro usuário.

## Multas por Atraso

- Usuários são sujeitos a multas diárias por atrasos na devolução dos livros, calculadas com base na política da empresa.

## Controle de Acesso

- Apenas usuários autenticados podem acessar funcionalidades de locação e histórico de livros.
- Administradores têm acesso a funcionalidades adicionais, como gestão de catálogo de livros e gerenciamento de usuários.

## Backup e Recuperação

- Realizar backups diários automáticos dos dados do sistema, com retenção de backups por no mínimo 30 dias.
- Implementar procedimentos de recuperação de dados para restaurar o sistema em caso de falha.

## Monitoramento e Auditoria

- O sistema deve registrar logs de todas as atividades críticas, como login, tentativas de login falhadas, locações e devoluções de livros.
- Logs devem ser auditáveis e armazenados de forma segura.

## Atualização e Manutenção

- Implementar um ciclo regular de manutenção e atualizações do sistema, com testes rigorosos antes de cada lançamento.

## Testes Automatizados

- Desenvolver e manter um conjunto abrangente de testes automatizados para garantir que novas alterações não introduzam regressões ou bugs.
