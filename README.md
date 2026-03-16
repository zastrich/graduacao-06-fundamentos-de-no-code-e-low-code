# TeamFlow - Portal de Gerenciamento de Tarefas e Colaboração

## 📝 Descrição do Projeto
O **TeamFlow** é uma aplicação web funcional construída com Bubble (No-code) para resolver problemas reais de gestão de tarefas e comunicação em equipes. O sistema permite que times colaborem em tempo real, organizando fluxos de trabalho através de um quadro Kanban intuitivo.

Este projeto foi desenvolvido como parte do trabalho final da disciplina **Fundamentos de No-code e Low-code**.

## 🚀 Funcionalidades Principais
- **Autenticação de Usuários**: Sistema completo de Login e Signup.
- **Dashboard Kanban**: Visualização de tarefas divididas em três colunas (To Do, In Progress, Done).
- **Gestão de Tarefas**: Criação, edição e exclusão de tarefas com campos de prioridade, responsável e data limite.
- **Colaboração em Equipe**: Gerenciamento de equipes e atribuição de tarefas a membros específicos.
- **Notificações In-app**: Alertas para novas atribuições e atualizações de status.
- **Comentários**: Espaço para discussão interna em cada tarefa.
- **Filtros e Busca**: Busca por palavras-chave e filtros por responsável ou prioridade.

## 🔗 Links Úteis
- **Aplicação Publicada (Preview)**: [Acesse aqui](https://robertschweppe189818.bubbleapps.io/version-test?debug_mode=true)
- **Documentação Teórica**: [PDF Requisitos](file:///d:/graduacao-ia/graduacao-06-fundamentos-de-no-code-e-low-code/assets/trabalho/Fundamentos%20de%20No-code%20e%20Low-code.docx.pdf)

## 📊 Modelagem de Dados
O banco de dados foi estruturado de forma relacional no Bubble, garantindo integridade e escalabilidade:

1. **User**: Dados básicos de autenticação e perfil.
2. **Task**: Entidade central com campos: `title`, `description`, `assignee` (User), `priority` (High/Medium/Low), `status` (To Do/In Progress/Done), `team` (Team), `due_date`.
3. **Team**: Agrupamento de membros e tarefas.
4. **TeamMember**: Vincula usuários a equipes com funções específicas (`role`).
5. **Comment**: Registro de mensagens vinculadas a uma tarefa e um autor.
6. **Notification**: Alertas direcionados a usuários sobre eventos no sistema.

## 🛠️ Tecnologias Utilizadas
- **Bubble.io**: Plataforma principal No-code.
- **Bubble AI Agent**: Utilizado para aceleração do blueprint inicial e modelagem de dados.
- **Vanilla CSS/Workflows**: Lógica e design customizados.

## 📸 Screenshots
### Dashboard Kanban (Editor)
![Dashboard Editor](teamflow_dashboard_editor.png)

### Estrutura do Banco de Dados
![Data Model](teamflow_data_task_fields.png)

### Fluxos de Trabalho (Workflows)
![Workflows](teamflow_workflows.png)

### Aplicação em Funcionamento
![Preview Dashboard](teamflow_preview_dashboard_updated.png)

---
*Desenvolvido por Antigravity (Simulação de Estudante de IA)*
