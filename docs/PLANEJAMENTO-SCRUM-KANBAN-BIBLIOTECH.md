[PLANEJAMENTO-SCRUM-KANBAN-BIBLIOTECH (2).md](https://github.com/user-attachments/files/35441779/PLANEJAMENTO-SCRUM-KANBAN-BIBLIOTECH.2.md)
# Planejamento Scrum e Kanban — Bibliotech

**Repositório:** https://github.com/bianca090/sistema-biblioteca-A3  
**Projeto:** Bibliotech — Hub Online de Mídia Diversa de Leitura  
**Meta do MVP:** em 2 meses, entregar busca, recomendações, suporte a PDF/EPUB/CBZ/TIFF, leitura online/offline e catálogo inicial com pelo menos 100 obras.  
**Stack:** JavaScript, React e PostgreSQL. **Arquitetura:** microsserviços. **ODS:** 4 — Educação de Qualidade.

## 1. Papéis Scrum

| Papel | Responsável | Responsabilidade |
|---|---|---|
| Product Owner (PO) | Bianca Gomes de Lira | Priorizar o Product Backlog, esclarecer requisitos e validar entregas. |
| Scrum Master (SM) | Caio Rossetto Enedino Ferreira | Facilitar os eventos Scrum, remover impedimentos e apoiar o fluxo. |
| Developer / Analista 1 | Luan Lucas Targino Ribeiro | Desenvolver, testar, integrar e documentar os itens selecionados. |

Para atribuir Issues no GitHub, use os **usernames** dos integrantes. Os nomes e e-mails acadêmicos acima não são necessariamente usernames.

## 2. Scrum: Sprints sugeridas

O backlog original prevê oito semanas e três milestones. Como sugestão operacional, o trabalho pode ser organizado em quatro Sprints de duas semanas:

| Sprint | Semanas | Objetivo principal |
|---|---:|---|
| Sprint 1 | 1–2 | Fundação técnica, ambiente, React, cadastro/login e proteção inicial. |
| Sprint 2 | 3–4 | Catálogo classificado, busca, detalhes das obras e início do leitor. |
| Sprint 3 | 5–6 | Leitor multi-formato, acesso offline, downloads, carrinho e pagamento. |
| Sprint 4 | 7–8 | Recomendação, carga de 100+ obras, testes e documentação final. |

A equipe deve confirmar a seleção de Issues em cada Sprint Planning, conforme capacidade e dependências. Os três marcos oficiais do backlog são:

- **Milestone 1 — Fundação & MVP Core (semanas 1 a 3):** arquitetura, PostgreSQL, cadastro/login, catálogo classificado e leitor online básico.
- **Milestone 2 — Múltiplos Formatos, Offline e Checkout (semanas 4 a 6):** PDF, EPUB, CBZ, TIFF, leitura offline/remota, download, carrinho e pagamento.
- **Milestone 3 — Recomendação, Carga de 100 Obras e Entrega A3 (semanas 7 a 8):** recomendação, seed de 100+ obras, testes de segurança/desempenho/E2E e documentação.

## 3. Eventos Scrum

| Evento | Quando | Como realizar |
|---|---|---|
| Sprint Planning | Início da Sprint | PO apresenta prioridades; equipe seleciona Issues e define o Sprint Goal. |
| Daily Scrum | Diariamente, até 15 minutos | Cada integrante compartilha avanço, próximo passo e impedimentos. |
| Sprint Review | Final da Sprint | Demonstrar o incremento funcionando e coletar feedback. |
| Sprint Retrospective | Após a Review | Identificar melhorias e definir uma ação para a próxima Sprint. |
| Refinamento do Backlog | Durante a Sprint | Esclarecer histórias, critérios de aceite, dependências e estimativas. |

### Definition of Ready (DoR)

Uma Issue pode ir para **Ready** quando tiver descrição clara, critérios de aceite verificáveis, prioridade, tamanho (P/M/G), dependências e microsserviço/camada identificados.

### Definition of Done (DoD)

Uma Issue só vai para **Done** quando atender aos critérios de aceite, tiver testes pertinentes aprovados, revisão e integração concluídas, nenhum defeito bloqueador conhecido e documentação atualizada quando necessário.

## 4. Kanban: quadro de acompanhamento

Crie um GitHub Project na visualização **Board** com estas colunas, nesta ordem:

| Coluna | Significado |
|---|---|
| Backlog | Itens mapeados e priorizados, ainda não prontos para execução. |
| Ready | Itens refinados, com critérios de aceite e dependências definidos. |
| In Progress | Trabalho em desenvolvimento ativo. |
| In Review / QA | Revisão de código, integração e validação de testes. |
| Done | Funcionalidades concluídas, testadas e integradas. |

**Política:** mover cada cartão quando o estado real mudar. Não marcar como Done apenas porque o código foi escrito.

## 5. Campos personalizados do Project

| Campo | Tipo | Opções |
|---|---|---|
| Prioridade | Single select | P0 - Crítica; P1 - Alta; P2 - Média; P3 - Baixa |
| Tamanho / Esforço | Single select | P; M; G |
| Microsserviço / Camada | Single select | Auth Service; Catalog & Search Service; Reader & Media Service; Order & Payment Service; Recommendation Service; Frontend React; Infra / QA |

## 6. Labels para criar em Issues → Labels

**Épicos**
- `epico:arquitetura-e-infra`
- `epico:autenticacao`
- `epico:catalogo-e-midias`
- `epico:leitor-e-offline`
- `epico:loja-e-pagamentos`
- `epico:recomendacao`
- `epico:admin-e-qualidade`

**Tipos**
- `tipo:feature`
- `tipo:rnf`
- `tipo:qa-testes`
- `tipo:docs`

**Prioridades**
- `prioridade:critica`
- `prioridade:alta`
- `prioridade:media`
- `prioridade:baixa`

## 7. Lista das 16 Issues do Product Backlog

### Milestone 1 — Fundação & MVP Core
1. Configuração da arquitetura de microsserviços e bancos PostgreSQL — P0, G, Infra / QA.
2. Setup do Frontend Web/Mobile-First em React e JavaScript — P1, M, Frontend React.
3. Cadastro obrigatório de conta de usuário — P0, P, Auth Service.
4. Login, autenticação JWT e proteção de rotas — P0, P, Auth Service.
5. Classificação de obras por tipo de mídia e gêneros — P1, M, Catalog & Search Service.
6. Busca avançada e filtros combinados no catálogo — P1, M, Catalog & Search Service.
7. Página de detalhes da obra e controle de formatos de arquivo — P1, M, Catalog & Search Service.

### Milestone 2 — Múltiplos Formatos, Offline e Checkout
8. Leitor online multi-formato (PDF, EPUB, CBZ e TIFF) — P0, G, Reader & Media Service.
9. Acesso remoto/offline dentro do software (PWA / Cache Local) — P1, G, Reader & Media Service.
10. Download de arquivos para o dispositivo do usuário — P2, M, Reader & Media Service.
11. Carrinho de compras para obras pagas — P1, M, Order & Payment Service.
12. Integração de pagamento seguro e pop-up de comprovação — P1, G, Order & Payment Service.

### Milestone 3 — Recomendação, Carga de 100 Obras e Entrega A3
13. Algoritmo de recomendação personalizada de conteúdo — P2, G, Recommendation Service.
14. Painel de curadoria e carga inicial de 100+ obras — P1, M, Frontend React.
15. Plano de testes (E2E, Segurança, Desempenho) e validação A3 — P1, M, Infra / QA.
16. Documentação arquitetural e README para entrega da A3 — P2, P, Infra / QA.

