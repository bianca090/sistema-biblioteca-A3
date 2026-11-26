# Bibliotech — Gestão Kanban

## Finalidade
Acompanhar o fluxo real das 16 tarefas do Product Backlog, tornando visíveis o estado de cada item, gargalos, revisões e entregas.

## Colunas do quadro
| Coluna | Quando usar |
|---|---|
| Backlog | Item registrado e priorizado, ainda sem refinamento suficiente para começar. |
| Ready | Critérios de aceite e dependências esclarecidos; pode ser puxado pela equipe. |
| In Progress | Há alguém trabalhando ativamente no item. |
| In Review / QA | Implementação aguardando revisão, integração ou validação de testes. |
| Done | Critérios de aceite atendidos, testes pertinentes aprovados e integração concluída. |

## Políticas de fluxo
1. Mover o cartão somente quando o estado real mudar.
2. Não colocar em Ready sem DoR.
3. Não colocar em Done apenas porque o código foi escrito.
4. Registrar impedimentos na Issue e conversar sobre eles na Daily.
5. Evitar iniciar muitos itens ao mesmo tempo; terminar o que já está em andamento antes de puxar novos itens.
6. Revisar o quadro nas reuniões da equipe.

## Campos personalizados
- **Prioridade:** P0 - Crítica; P1 - Alta; P2 - Média; P3 - Baixa.
- **Tamanho / Esforço:** P; M; G.
- **Microsserviço / Camada:** Auth Service; Catalog & Search Service; Reader & Media Service; Order & Payment Service; Recommendation Service; Frontend React; Infra / QA.

## Como configurar no GitHub Project
Crie um Project separado chamado **Bibliotech — Kanban** e adicione o repositório `bianca090/sistema-biblioteca-A3`.
- Visualização principal: **Board**.
- Agrupar por **Status**.
- Configure as opções do Status nesta ordem: Backlog, Ready, In Progress, In Review / QA, Done.
- Adicione todas as 16 Issues do repositório.
- Inicialmente, deixe os itens em Backlog; só mova os itens realmente refinados para Ready.
- Crie visualização adicional Table se quiser consultar prioridade, tamanho e camada técnica.

## Como o Kanban e o Scrum se relacionam
O Scrum organiza o trabalho em Sprints com objetivo e eventos definidos. O Kanban mostra o fluxo contínuo das tarefas e seus estados. Os dois Projects devem apontar para as mesmas Issues do repositório, evitando criar cópias diferentes das tarefas.
