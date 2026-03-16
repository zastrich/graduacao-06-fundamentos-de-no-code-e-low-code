# **Graduação IA e Automação Digital - 1º Semestre**
## *Trabalho para a disciplina de Fundamentos de No-code e Low-code*

O **TeamFlow** é uma aplicação web funcional construída com Bubble (No-code) para resolver problemas reais de gestão de tarefas e comunicação em equipes. O sistema permite que times colaborem em tempo real, organizando fluxos de trabalho através de um quadro Kanban intuitivo.

Este projeto foi desenvolvido como parte do trabalho final da disciplina **Fundamentos de No-code e Low-code**.

# Vídeo de demonstração (Pitch):
[![Watch the video](https://img.youtube.com/vi/-DsExJu9A5U/maxresdefault.jpg)](https://youtu.be/-DsExJu9A5U)

## 🚀 Funcionalidades Principais
- **Autenticação de Usuários**: Sistema completo de Login e Signup.
- **Dashboard Kanban**: Visualização de tarefas divididas em três colunas (To Do, In Progress, Done).
- **Gestão de Tarefas**: Criação, edição e exclusão de tarefas com campos de prioridade, responsável e data limite.
- **Colaboração em Equipe**: Gerenciamento de equipes e atribuição de tarefas a membros específicos.
- **Notificações In-app**: Alertas para novas atribuições e atualizações de status.
- **Comentários**: Espaço para discussão interna em cada tarefa.
- **Filtros e Busca**: Busca por palavras-chave e filtros por responsável ou prioridade.

## 🔗 Links Úteis
- **Aplicação Publicada (Preview)**: [Acesse aqui](https://teamflow-27948.bubbleapps.io/version-test/)
- **Trabalho Teórico**: [Link](src/trabalho-final/teorico/Disciplina%20de%20Fundamentos%20de%20No-code%20e%20Low-code%20-%20Trabalho%20Teórico.md)

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

## 📸 Screenshots

### Tela principal
![Tela principal](src/trabalho-final/screens/home.png)

### Tela principal - Modais de ação
![alt text](src/trabalho-final/screens/home/image.png)
![alt text](src/trabalho-final/screens/home/image-1.png)
![alt text](src/trabalho-final/screens/home/image-2.png)
![alt text](src/trabalho-final/screens/home/image-3.png)

### Workflows
![Workflows](src/trabalho-final/screens/workflows.png)

![Workflows 2](src/trabalho-final/screens/workflows-2.png)

### Estrutura do Banco de Dados
![alt text](src/trabalho-final/screens/data/image.png)
![alt text](src/trabalho-final/screens/data/image-1.png)
![alt text](src/trabalho-final/screens/data/image-2.png)
![alt text](src/trabalho-final/screens/data/image-3.png)
![alt text](src/trabalho-final/screens/data/image-4.png)
![alt text](src/trabalho-final/screens/data/image-5.png)

### Aplicação em uso
![alt text](src/trabalho-final/screens/aplicacao/image.png)
![alt text](src/trabalho-final/screens/aplicacao/image-1.png)
![alt text](src/trabalho-final/screens/aplicacao/image-2.png)
![alt text](src/trabalho-final/screens/aplicacao/image-3.png)
![alt text](src/trabalho-final/screens/aplicacao/image-4.png)
![alt text](src/trabalho-final/screens/aplicacao/image-5.png)
![alt text](src/trabalho-final/screens/aplicacao/image-6.png)
![alt text](src/trabalho-final/screens/aplicacao/image-7.png)
![alt text](src/trabalho-final/screens/aplicacao/image-8.png)