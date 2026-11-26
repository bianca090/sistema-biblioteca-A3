# Bibliotech — Gestão Scrum

## Objetivo do produto
Entregar em oito semanas um MVP do hub de leitura com busca, recomendações, suporte a PDF/EPUB/CBZ/TIFF, leitura online/offline e catálogo inicial de pelo menos 100 obras. Stack prevista: JavaScript, React e PostgreSQL; arquitetura em microsserviços. O projeto se relaciona ao ODS 4 — Educação de Qualidade.

## Papéis definidos no backlog
- **Product Owner:** Bianca Gomes de Lira — prioriza o Product Backlog e valida entregas.
- **Scrum Master:** Caio Rossetto Enedino Ferreira — facilita os eventos e ajuda a remover impedimentos.
- **Developer / Analista:** Luan Lucas Targino Ribeiro — desenvolvimento, testes, integração e documentação.

## Organização sugerida
O backlog prevê oito semanas e três milestones. Para acompanhamento, a equipe pode trabalhar com quatro Sprints de duas semanas. A divisão abaixo é uma proposta de planejamento; deve ser confirmada pela equipe conforme capacidade e dependências.

| Sprint | Período | Objetivo da Sprint | Itens do backlog |
|---|---|---|---|
| Sprint 1 | Semanas 1–2 | Preparar base técnica e autenticação | Issues 1, 2, 3 e 4 |
| Sprint 2 | Semanas 3–4 | Entregar catálogo, busca e início do leitor | Issues 5, 6, 7 e planejamento inicial da 8 |
| Sprint 3 | Semanas 5–6 | Leitura multi-formato, offline e checkout | Issues 8, 9, 10, 11 e 12 |
| Sprint 4 | Semanas 7–8 | Recomendações, acervo, testes e documentação | Issues 13, 14, 15 e 16 |

## Metas dos marcos (milestones do backlog original)
1. **Milestone 1 — Fundação & MVP Core (semanas 1 a 3):** arquitetura, PostgreSQL, cadastro/login, catálogo classificado e leitor online básico.
2. **Milestone 2 — Múltiplos Formatos, Offline e Checkout (semanas 4 a 6):** PDF, EPUB, CBZ, TIFF, leitura offline/remota, download, carrinho e pagamento.
3. **Milestone 3 — Recomendação, Carga de 100 Obras e Entrega A3 (semanas 7 a 8):** recomendação, seed de 100+ obras, testes de segurança/desempenho/E2E e documentação.

## Eventos
- **Sprint Planning:** início de cada Sprint; selecionar Issues e definir objetivo.
- **Daily Scrum:** diariamente, até 15 minutos; avanço, próximo passo e impedimentos.
- **Sprint Review:** final da Sprint; demonstrar o incremento e recolher feedback.
- **Sprint Retrospective:** após a Review; registrar o que funcionou e uma melhoria concreta.
- **Refinamento:** durante a Sprint; esclarecer critérios, dependências e estimativas.

## Definition of Ready (DoR)
Uma Issue está pronta quando tem objetivo claro, critérios de aceite verificáveis, prioridade, tamanho, dependências e camada técnica identificados.

## Definition of Done (DoD)
Uma Issue só deve ser concluída quando os critérios de aceite forem atendidos, os testes pertinentes passarem, revisão e integração estiverem concluídas, não houver defeito bloqueador conhecido e a documentação necessária estiver atualizada.

## Como configurar a visão Scrum no GitHub Project
Crie um Project separado chamado **Bibliotech — Scrum** e adicione o repositório `bianca090/sistema-biblioteca-A3`.
- Visualização **Table**: backlog completo, ordenado por prioridade.
- Campo **Sprint** (Single select): Sprint 1, Sprint 2, Sprint 3, Sprint 4, Sem Sprint.
- Campo **Prioridade** (Single select): P0 - Crítica, P1 - Alta, P2 - Média, P3 - Baixa.
- Campo **Tamanho / Esforço** (Single select): P, M, G.
- Campo **Microsserviço / Camada** (Single select): Auth Service, Catalog & Search Service, Reader & Media Service, Order & Payment Service, Recommendation Service, Frontend React, Infra / QA.
- Crie uma visualização **Board por Sprint**, agrupada pelo campo Sprint, se a interface permitir.
- Não marcar tarefas como concluídas antes da validação real.

## Transparência do planejamento
As quatro Sprints são uma organização operacional sugerida para o prazo de oito semanas; os três milestones são os marcos apresentados no backlog original. A equipe deve registrar ajustes decididos nas reuniões.
