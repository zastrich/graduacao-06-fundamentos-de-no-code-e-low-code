# Trabalho Teórico – Fundamentos de No-code e Low-code

## 1. Parte Teórica – Análise e Discussão

### 1.1 Contextualização do Desafio
- **Descrição do problema real a ser resolvido:** Uso excessivo de planilhas e adoção de diversas plataformas fragmentadas para a execução de tarefas, disparo de alertas e comunicação de equipe. Esse cenário tradicional resulta em constante desorganização, inconsistência nas atualizações e perda sistêmica de informações no momento de transição de processos.
- **Público-alvo:** Equipes corporativas, gestores e times de rotina diária que sofrem com as falhas de comunicação e a ineficiência que a falta de uma única ferramenta integrada de apoio colaborativo gera.
- **Benefícios esperados da solução:** Através do *TeamFlow*, espera-se centralizar toda e qualquer atividade em um quadro *Kanban* dinâmico que estrutura de forma escalável atributos e status (como "A Fazer", "Em Progresso" e "Concluído"). Assim, resolve-se o gargalo da perda de dados operacionais e dá-se autonomia comunicativa à equipe.

### 1.2 Justificativa pelo Uso de No-Code/Low-Code
- **Razões estratégicas para escolher Bubble:** Diferentemente do emaranhado de softwares exigidos antes pelo problema central, o *Bubble.io* destacou-se por propiciar a estrutura para consolidação centralizada em um único local: a interface amigável unida nativamente ao ecossistema de banco relacional e regras lógicas visuais.
- **Vantagens e limitações frente ao desenvolvimento tradicional:**
  - **Vantagens:** A indiscutível velocidade de iteração. Modelar a lógica do banco de dados e aplicar automações complexas visualmente exigiu apenas uma fração do tempo que seria empregado codificando em metodologias tradicionais web.
  - **Limitações:** Um conhecido *vendor lock-in* (engessamento e dependência quanto à provedora da infraestrutura No-Code) e os limitados e complexos controles que dizem respeito às otimizações estruturais finas de um servidor dedicado se comparado a uma arquitetura nativa própria.
- **Ganhos de produtividade, custo e tempo:** Uma velocidade de entrega dramática e a facilidade em responder sem entraves técnicos geram protótipos em ritmo contínuo. Ao invés do alto custo com uma equipe vasta de programadores full-stack, a plataforma enxuta garante implementação instantânea para focar na entrega de valor e experiência do usuário (UX).

### 1.3 Modelagem de Dados
- **Explicação da estrutura de banco de dados criada no Bubble:** Estruturada via aba `Data` (*Data Types*), optando por criar bases plenamente relacionais e localizadas em sua totalidade para o Português do Brasil. Um dos méritos fundamentais dessa modelagem é a forte inclusão de `Privacy Rules` no banco, visando atender a obrigações éticas de dados corporativos (restringir sigilo na camada visual para que seja visível apenas sob condições criteriosas de função).
- **Entidades, campos, relacionamentos e regras:**
  - **Tasks (Tarefas):** Entidade atrelada fortemente de forma relacional ao conjunto de pessoas que realizam o serviço (diretamente vinculadas a `Users` e `Teams`). Campos vitais para manutenção e *drag-and-drop* no front controlam obrigatoriamente status descritivos do *Kanban*.
  - **Users (Usuários):** Mantém a identidade relacional (como "Camila Ferreira") de quem manipula e preenche atribuições gerenciais. É esse o nó que detém forte sigilo em atributos e sofre a limitação exigida pela trava imposta via `Privacy Rules`.
  - **Teams (Equipes):** Tipagem de categorização macro que congrega logicamente as tarefas dentro dos blocos e setores do fluxo da empresa.

### 1.4 Lógica e Workflows
- **Descrição da lógica de workflows definidos:** Automações (*Eventos* e *Ações*) projetadas no módulo `Workflow` do *Bubble*. Essa esteira de comandos transforma ações do visual em mutações instantâneas de registro. Quando qualquer dado é modificado nas *views* base, ele é engatilhado no banco imediatamente ("Data Sources vinculados diretamente nos campos").
- **Regras de negócio automatizadas:**
  - **Criação e Delegação Direta:** No ato da emissão de um card pelo formulário na aplicação *Preview*, associações complexas no banco (tarefa vinculada a um respectivo *User* como Responsável) operam transparentemente no arrasto em tela.
  - **Atualização de Estado de Ciclo de Vida:** Existe arquitetada uma rotina imperativa de sistema que lê uma modificação humana (como a transição de um card à instância "Concluído") e dispara no servidor a sobreposição de sistema, que atualiza a "Data de Modificação" do determinado registro automaticamente.

### 1.5 Publicação e Manutenção
- **Estratégias de publicação (ambiente de testes vs produção):** Validação técnica visual do projeto mediante modo interativo e contínuo `Preview`. Essa simulação confere toda a integridade na comunicação com os `Data Types` em área de desenvolvimento *staging* antes de confirmar por completo as edições na *live app* que impactariam a corporação usuária.
- **Plano de manutenção contínua:** Os ecossistemas do *Bubble*, baseados num padrão salvamento imediato e na edição visual de rotas ou permissões (exposição das *Privacy Rules*), tornam reparações ou manutenções orgânicas simples e diretas. Modificações para novas versões da agência fluem de modo imediato para implantação visando a preservação segura da *TeamFlow*.
