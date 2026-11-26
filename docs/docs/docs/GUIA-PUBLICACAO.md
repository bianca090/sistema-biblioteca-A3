# Guia de publicação no GitHub — entrega Bibliotech

Repositório: https://github.com/bianca090/sistema-biblioteca-A3

## Ordem recomendada

### 1. Publicar a documentação
No repositório, clique em **Add file → Create new file**.
Crie `docs/SCRUM.md`, cole o conteúdo de `SCRUM.md` e faça Commit changes.
Repita para `docs/KANBAN.md` e `docs/README-PROJETO.md`.
Para as Issues, crie-as em **Issues → New issue** copiando o arquivo Markdown correspondente em `issues/`.

### 2. Criar as 16 Issues
Para cada arquivo de `issues/`:
1. Abra **Issues → New issue**.
2. Copie o título do nome do arquivo (sem número inicial) e o conteúdo Markdown.
3. Crie a Issue.
4. Associe o milestone correspondente:
   - Issues 1–7: Milestone 1 — Fundação & MVP Core.
   - Issues 8–12: Milestone 2 — Múltiplos Formatos, Offline e Checkout.
   - Issues 13–16: Milestone 3 — Recomendação, Carga de 100 Obras e Entrega A3.
5. Adicione labels conforme o conteúdo e atribua responsáveis somente depois de confirmar os usernames GitHub dos integrantes.

### 3. Criar os marcos
Em **Issues → Milestones → New milestone**, crie os três milestones com os nomes e descrições indicados no arquivo SCRUM.md.

### 4. Criar o Project Scrum
Abra a aba **Projects** do repositório ou do perfil Bianca e crie **Bibliotech — Scrum**.
- Vincule `bianca090/sistema-biblioteca-A3`.
- Adicione as 16 Issues.
- Crie campo Sprint (Sprint 1, Sprint 2, Sprint 3, Sprint 4, Sem Sprint).
- Crie Prioridade, Tamanho / Esforço e Microsserviço / Camada.
- Use Table para backlog e uma visão agrupada por Sprint, se disponível.

### 5. Criar o Project Kanban
Crie outro Project chamado **Bibliotech — Kanban**.
- Vincule o mesmo repositório.
- Adicione as mesmas 16 Issues.
- Use Board agrupado por Status.
- Configure: Backlog, Ready, In Progress, In Review / QA e Done.
- Inicialmente mantenha todas em Backlog. Mova para Ready apenas as tarefas realmente refinadas.

### 6. Conferência final
- [ ] Os dois Projects estão públicos ou visíveis ao professor, conforme as permissões da conta.
- [ ] O repositório contém documentação Scrum e Kanban.
- [ ] As 16 Issues existem e estão vinculadas aos dois Projects.
- [ ] Os três milestones foram criados.
- [ ] Os campos personalizados foram configurados.
- [ ] Responsáveis foram associados usando usernames corretos.
- [ ] O status reflete o trabalho real; não marcar como concluído o que ainda não foi feito.

## Observação importante
O conector disponível nesta sessão não recebeu permissão do GitHub para criar Issues (erro 403). Por isso, a publicação das Issues e a criação dos Projects precisam ser concluídas na interface web autenticada da conta Bianca. Não compartilhe senha, token ou código de autenticação.
