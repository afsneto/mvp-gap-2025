# SPRINT DE GESTÃO ÁGIL DE PROJETOS E PRODUTOS

Este repositório contém os artefatos desenvolvidos no contexto da disciplina **Gestão Ágil de Projetos e Produtos**, com a criação do MVP **SAVEINLINE**: uma plataforma web para **gestão e unificação do inventário de materiais sobressalentes** de almoxarifados em diferentes concessões de linhas de transmissão.

---

## FERRAMENTAS UTILIZADAS NO MVP

- **Miro** → Desenvolvimento da Lean Inception para ideação e delimitação do escopo do MVP.  
- **Figma** → Criação de protótipos de baixa fidelidade com base no Material Design.  
- **Jira** → Gestão do backlog do produto e acompanhamento das sprints.  

---

## DOCUMENTOS DO REPOSITÓRIO

- **MVP Canvas – Miro**: [🔗 Link para o quadro](https://miro.com/app/board/uXjVM2S9g5o=/?share_link_id=435509307429)  
- **Protótipo – Figma**: [🔗 Link para o protótipo](https://www.figma.com/design/rJMBzMc92lL4clVlIaaJT2/MVP-GAP?node-id=0-1&p=f&t=iZgeNVenkHmS6kja-0)  
- **Backlog – Jira**: [🔗 Link para o backlog](https://afsneto.atlassian.net/jira/software/projects/GAP/boards/34/backlog?epics=visible)  

---

## LEAN INCEPTION

### KICKOFF
O escopo do MVP é a ideação e o planejamento inicial do **SAVEINLINE**.  
A empresa fictícia **MYLINES** possui 5 concessões de linhas de transmissão (aproximadamente 1000 km de extensão) e cada concessão possui um almoxarifado de materiais sobressalentes (torres metálicas, isoladores, cabos, acessórios e ferragens, etc.).  
O objetivo é desenvolver uma plataforma web para gerenciar e integrar esses estoques, aumentando eficiência e reduzindo custos.

### EQUIPE
- **PO**: José  
- **Scrum Master**: Bruna  
- **Backend**: Adriano  
- **Frontend**: Roberta  

### VISION
- **PARA** responsáveis pela O&M (operação e manutenção)  
- **QUE** precisam consultar materiais sobressalentes em almoxarifados  
- **O SAVEINLINE**  
- **É** um aplicativo web  
- **QUE** auxilia na consulta e na gestão automática de materiais disponíveis  
- **DIFERENTE DE** planilhas isoladas e manuais alimentadas isoladamente pelo gestor de cada almoxarifado
- **NOSSO PRODUTO** oferece integração, automação e relatórios, otimizando tempo e custos.  

### IS-IS NOT - DOES - DOES NOT DO

#### IS
- Aplicativo web para integração de almoxarifados  
- Plataforma que fornece avisos personalizados para coordenação e gerência de O&M  

#### IS NOT
- Sistema de compra e venda de materiais  
- Calculadora de frete, impostos ou custos logísticos  

#### DOES
- Cadastro e consulta de materiais por almoxarifado  
- Acompanhamento de frequência de uso dos materiais
- Relatórios automáticos para gerência  
- Lista de materiais conforme instruções de trabalho (IT)  

#### DOES NOT DO
- Reposição automática de estoque  
- Consulta de preços históricos  
- Envio de pedidos de compra ao mercado para fornecedores  

### GOALS
- **Redução de despesas** (evitar compras duplicadas, integração de almoxarifados, negociação com fornecedores por maior volume).  
- **Agilidade em emergências** (consulta rápida, geolocalização de materiais, listas automatizadas).  
- **Melhor controle** (relatórios, planejamento de compras, compatibilização de dados técnicos).  

### PERSONAS
### PERSONAS
* **Gustavo**, "o gerente"  
    * 51 anos; engenheiro eletricista; averso a novas tecnologias.
    * Responsável pela mobilização de equipes disponíveis em campo para atendimentos emergenciais.
    * Precisa de um sistema com interface simples para consultas aos almoxarifados.
    
* **Renato**, "chefe da equipe em campo"
    * 37 anos; engenheiro eletricista; é autodisciplinado.
    * Responsável pela orientação e alinhamento da instrução de trabalho junto à equipe, conforme característica da emergência.
    * Possui certa facilidade com tecnologia, não havendo limitações no uso de aplicativos Web.
    * Necessita de um relatório incluindo a instrução de trabalho, relacionado à ocorrência, junto com a relação de materiais e ferramentas necessários à intervenção.
    
* **Rodrigo**, "chefe do almoxarifado"
    * 32 anos; técnico eletricista; conhecimento adquirido pela prática em campo.
    * Responsável pelo controle de materiais do almoxarifado.
    * Necessita de consultas simples e rápidas aos materiais disponíveis no almoxarifado, e melhor controle dos itens que entram e saem do almoxarifado.  

### USER JOURNEYS
* **Gustavo**, "o gerente"  
    * Recebe uma comunicação do centro de operações (COL) sobre a ocorrência de um sinistro.
    * Entra em comunicação com o engenheiro de campo responsável pela linha de transmissão onde foi identificada a ocorrência.
    * Acesso ao sistema SAVEINLINE, seleciona o tipo da ocorrência, nome ou sigla do engenheiro de campo responsável e registra a solicitação.
    * Após a solução da ocorrência, Gustavo verifica através do um relatório gerado pelo sistema, um resumo da ocorrência e relação dos materiais / ferramentas utilizadas no serviço.
* **Renato**, "chefe de equipe em campo" 
    * Após atendimento da ligação do Gustavo, e do COL, Renato mobiliza equipe para intervenção.
    * Renato e equipe vai até almoxarifado buscar materiais e ferramentas conforme relação fornecida pelo sistema.
    * Após solução do problema, Renato preenche um formulário do sistema indicando quais materiais foram utilizados em campo, e quais retornaram ao almoxarifado após intervenção.
* **Rodrigo**, "chefe do almoxarifado"
    * Mantém o almoxarifado em ordem.
    * Verifica diariamente os materiais e ferramentas, mantendo a relação de materiais cadastrados no sistema sempre atualizada.
    * Após intervenção em campo e submissão do relatório do Renato no sistema, Rodrigo verifica relação de materiais utilizados.
    * Rodrigo confirma as alterações indicadas pelo Renato, atualizando assim a relação dos materiais disponíveis no almoxarifado.
    * Rodrigo indica no sistema quais itens necessitam de reposição, e esta solicitação é recebida pelo Gustavo.

### FEATURE BRAINSTORMING
* Interface simples  
* Cadastro de novos materiais  
* Busca de material por Estado ou Concessão (Transmissora)
* Após localização do material nova página é aberta com as seguintes informações:
    * Código do material
    * Fabricante
    * Descrição
    * Quantidade
    * Cacterísticas Técnicas
    * Opção para anexar desenhos ou documentos técnicos
* Na página do material botão para solicitação de compra de novas unidades
* Na tela de submissão do relatório após retorno de campo, opção para realizar o upload de fotos com o registro do sinistro.
* Desenvolvimento futuro de app Android para utilização em conjunto da plataforma Web, com foco na equipe em campo.
* Definir opção para cadastramento de novos tipos de intervenção em campo (instruções de trabalho), com as informações:
    * Código da intervenção
    * Descrição
    * Relação de material necessário
    * Estimativa de tempo para solução do problema
    * Número de profissionais envolvidos
* Opção para geração de gráficos em barras para acompanhamento da utilização ao longo de um período de tempo de materiais (para determinado código ou por tipo de material empregado)

### TECHNICAL, BUSINESS AND UX REVIEW
![image](/imagens/Tech_Bus_Ux.png)  

### SEQUENCER
![image](/imagens/Sequencer.png)  

### MVP CANVAS
![image](/imagens/MVP_Canvas.png)  

---

## BACKLOG DO PRODUTO
Backlog estruturado no **Jira**, com épicos, features, histórias e estimativas.  
![image](/imagens/Backlog.png)  

---

## PRIMEIRA SPRINT

A **Sprint 1** foi planejada para entregar um protótipo navegável e validar as funcionalidades essenciais do MVP.  
![image](/imagens/Sprint.png)

**Features contempladas na Sprint 1:**
- **Listagem de materiais de todos os almoxarifados** → Permitir a visão global do estoque em todas as concessões.  
- **Busca de materiais por Estado e Concessão** → Viabilizar consultas filtradas por região, otimizando a localização de recursos.  
- **Cadastro de novos materiais** → Possibilitar a inclusão de itens recém-adquiridos, com dados técnicos padronizados.  
- **Agrupar materiais por IT (Instrução de Trabalho)** → Relacionar automaticamente materiais necessários a intervenções específicas.  

---

## INTERFACE FIGMA
Protótipo navegável desenvolvido no **Figma** (Material Design, 12 colunas, 1440px).
Todas as telas se encontram disponíveis no arquivo ![link](imagens/MVP-Figma-SaveInLine.pdf)  

🔗 [Link para o Figma](https://www.figma.com/design/rJMBzMc92lL4clVlIaaJT2/MVP-GAP?node-id=0-1&p=f&t=iZgeNVenkHmS6kja-0)  

### Tela de acesso
![image](/imagens/MVP-Figma - Tela de Acesso.jpg)

### Dashboard
![image[(/imagens/MVP-Figma - Dashboard.jpg)

### Detalhes do sinistro
![image](/imagens/MVP-Figma - Detalhes do Sinistro.jpg)

---

## VIDEO DE APRESENTAÇÃO
Demonstração do SAVEINLINE, cobrindo: visão, backlog, protótipo e resultados.  
🔗 [Assistir no YouTube](https://youtu.be/Mmtqc2CWG5w)  

