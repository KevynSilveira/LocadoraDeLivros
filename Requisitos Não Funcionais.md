## Requisitos Não Funcionais Atualizados

1. **Segurança**
   - O sistema deve criptografar as senhas dos usuários usando algoritmos de criptografia robustos.
   - O sistema deve implementar controle de acesso baseado em funções (RBAC) para proteger os dados dos usuários.
   - Deve haver proteção contra ataques comuns, como SQL Injection, Cross-Site Scripting (XSS) e Cross-Site Request Forgery (CSRF).

2. **Usabilidade**
   - O sistema deve ter uma interface amigável e intuitiva, com um design consistente em todas as telas.
   - A interface deve ser acessível e fácil de navegar para todos os tipos de usuários, seguindo as diretrizes de acessibilidade WCAG 2.1.
   - O sistema deve fornecer feedback claro e imediato para as ações do usuário.

3. **Desempenho**
   - O sistema deve ser capaz de lidar com múltiplas requisições simultâneas sem degradar o desempenho.
   - O tempo de resposta para operações críticas (como login e pesquisa) deve ser inferior a 2 segundos.
   - O sistema deve ser otimizado para minimizar o uso de recursos do servidor e da rede.

4. **Confiabilidade**
   - O sistema deve ter um uptime de 99.9%, garantindo alta disponibilidade.
   - Deve haver mecanismos de backup e recuperação de dados para garantir a integridade dos dados armazenados.
   - O sistema deve passar por testes rigorosos de qualidade e controle de versão antes de cada lançamento.

5. **Compatibilidade**
   - O sistema deve ser compatível com os principais navegadores da web (Chrome, Firefox, Safari, Edge).
   - O sistema deve ser responsivo, adaptando-se a diferentes dispositivos (desktops e notebooks) com tamanhos de tela variados.
   - Deve suportar as últimas versões dos navegadores, garantindo compatibilidade retroativa de até 2 versões anteriores.

6. **Manutenibilidade**
   - O sistema deve ser fácil de manter e atualizar, com um código modular e reutilizável.
   - O código deve ser bem documentado e seguir boas práticas de desenvolvimento, como padrões de nomenclatura, formatação e design de software.
   - Deve haver uma suíte de testes automatizados para garantir que novas alterações não introduzam bugs.

### Tabela de Compatibilidade

| Requisito                 | Detalhe                                                   |
|---------------------------|-----------------------------------------------------------|
| Navegadores Suportados    | Chrome, Firefox, Safari, Edge                             |
| Dispositivos Suportados   | Desktops e notebooks                                      |
| Versões Mínimas Suportadas| Últimas 2 versões dos navegadores principais              |

### Tabela de Segurança

| Requisito                | Detalhe                                                   |
|--------------------------|-----------------------------------------------------------|
| Criptografia de Senhas   | Uso de bcrypt                                             |
| Controle de Acesso       | Implementação de RBAC                                     |
| Proteção Contra Ataques  | SQL Injection, XSS, CSRF                                  |
| Backup e Recuperação     | Mecanismos regulares de backup e estratégias de recuperação|

### Tabela de Desempenho

| Requisito                  | Detalhe                                                   |
|----------------------------|-----------------------------------------------------------|
| Tempo de Resposta          | Inferior a 2 segundos para operações críticas             |
| Suporte a Requisições      | Capacidade de lidar com múltiplas requisições simultâneas |
| Otimização de Recursos     | Minimização do uso de recursos do servidor e da rede      |

