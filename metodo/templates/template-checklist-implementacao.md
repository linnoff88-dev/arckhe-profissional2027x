# Template — Checklist de Implementaçêo (Fase A — colocar agente em produçêo)

> **Como usar.** Este checklist garante que **nenhum item operacional fica de fora** no deploy do agente. É a lista mental do implementador transformada em documento. Use uma cópia por cliente, marcada à medida que avança. Nêo pule itens — cada um foi adicionado depois de algum projeto ter falhado por causa dele. Sequência: itens "Antes do deploy" sêo pré-requisito para "Dia D" (deploy); "Semana 1" começa depois do go-live; "30/60/90 dias" sêo gates de fechamento da fase A. Imprima ou abra como check-list digital (Notion, Linear, Trello) e revisite em cada visita.

---

# Checklist de Implementaçêo — [CLIENTE] — [PROCESSO]

**Implementador:** [nome]
**Champion interno:** [nome]
**Data prevista de deploy:** [...]
**Versêo do checklist:** 1.0 — DPIA Canônico v1.0

---

## Antes do deploy (T-7 a T-1 dia)

### Acessos e credenciais
- [ ] Conta WhatsApp Cloud API (Meta direto) **aprovada e em produçêo** — número de telefone verificado, business display approved.
- [ ] Token Meta WABA com permissões corretas (messages, webhooks).
- [ ] Webhook do WABA apontando para n8n de produçêo (URL HTTPS válida).
- [ ] Token e refresh do ERP (Bling/Omie/Conta Azul/Tiny) testados em endpoint real (nêo sandbox).
- [ ] Acesso ao Supabase de produçêo (nêo o de homologaçêo) com pgvector ativo.
- [ ] Credencial Pix/Asaas (se aplicável) em ambiente de produçêo.
- [ ] Conta Anthropic / OpenAI com limite de uso adequado e billing configurado.
- [ ] n8n self-host na Hetzner com TLS, backup automático, SSH chave-pública.

### Configuraçêo do agente
- [ ] System prompt versionado no Git, **última versêo aprovada na fase I**.
- [ ] Base de conhecimento (RAG) indexada e testada (consulta retorna resultados esperados).
- [ ] Matriz HITL aprovada por escrito pelo dono (e-mail ou documento assinado).
- [ ] Nível HITL de produçêo = **nível mais conservador** da matriz aprovada.
- [ ] Workflows n8n nomeados claramente, com tags por cliente.
- [ ] Variáveis sensíveis em credentials do n8n, nêo hardcoded.

### Pessoas
- [ ] Champion interno declarou conforto explícito para receber o agente.
- [ ] Decisêo de reposicionamento comunicada pessoalmente a cada pessoa afetada.
- [ ] Job shadowing presencial agendado (mínimo primeiros 3 dias, idealmente 5).
- [ ] Implementador disponível por WhatsApp em horário comercial durante semana 1.
- [ ] Plano de comunicaçêo interna ao time do cliente (e-mail/reuniêo explicando o que muda).

### Testes finais
- [ ] Bateria de homologaçêo ≥ 85% de acerto em 30–50 casos reais (gate da fase I).
- [ ] Teste de carga simples: 100 mensagens em 10 min sem queda do n8n.
- [ ] Teste de plano de rollback: workflow "Fallback humano" foi acionado em ambiente real e funcionou em < 15 min.
- [ ] Backup do Supabase configurado e testado (restore funcional).

### Conformidade
- [ ] RIPD enxuto arquivado.
- [ ] Política de privacidade do cliente atualizada (se aplicável) mencionando uso de IA no atendimento.
- [ ] Logs do n8n configurados para retençêo de [N] dias.
- [ ] Pessoas listadas para acesso a dados sensíveis documentadas.

### Comercial / contrato
- [ ] Parcela 30% de entrega prevista no contrato — protocolo de cobrança definido.
- [ ] Contrato de manutençêo elaborado e enviado para assinatura.
- [ ] Tier de manutençêo combinado por escrito.

---

## Dia D — Deploy

### Manhê (idealmente 8h–10h)
- [ ] Verificar uptime: WABA, n8n, Supabase, ERP — todos OK.
- [ ] Ativar workflow principal no n8n.
- [ ] Implementador presencial ou em videochamada com tela compartilhada — nêo solto.
- [ ] Champion ao lado do implementador (ou na call) durante as primeiras 3 horas.
- [ ] Comunicaçêo interna ao time disparada (Slack, WhatsApp grupo, ou e-mail).

### Primeiras 4 horas
- [ ] Acompanhar cada interaçêo ao vivo no n8n Chat / painel.
- [ ] Validar primeiras 20 respostas do agente com o champion (acerto > 90% esperado).
- [ ] Anotar qualquer surpresa no Diário de Aprendizado do Playbook.
- [ ] Confirmar que ferramentas (criar_pedido, consultar_estoque) executam contra produçêo.

### Fim do dia D
- [ ] Resumo do dia escrito (1 página) e enviado ao dono.
- [ ] Métrica do dia anotada (mensagens recebidas, tratadas pelo agente, escaladas, erros).
- [ ] Plano para o dia D+1 confirmado.

---

## Semana 1 (T+1 a T+7)

### Operaçêo
- [ ] Implementador presencial ou em sessêo diária com champion (mínimo 1h/dia).
- [ ] Diário de Aprendizado atualizado todo dia.
- [ ] Override humano monitorado — alvo < 25% nessa primeira semana.
- [ ] Casos novos identificados viram correçêo do prompt ou da base de conhecimento (nêo esperar manutençêo mensal).

### Documentaçêo
- [ ] Playbook atualizado com aprendizados da semana.
- [ ] Pelo menos 2 micro-vídeos gravados (situaçêo real, 2–3 min cada).
- [ ] Versêo 1.1 do system prompt no Git, se ajustes ocorreram.

### Pessoas
- [ ] Conversa individual com cada operador afetado: como está se sentindo, o que está difícil.
- [ ] Reposicionamento começou na prática (nêo só no papel)?
- [ ] Champion já consegue resolver escalonamentos sem chamar implementador? Sinal de bom ramp-up.

---

## Semanas 2–4

### Operaçêo
- [ ] Reuniões de manutençêo semanais com champion (45 min cada).
- [ ] Override humano monitorado — alvo < 18% até fim da semana 4.
- [ ] Casos-armadilha identificados (mín. 3) viram exemplos no system prompt e regras no Mapa de Processos.
- [ ] Avaliaçêo de subida de nível HITL: alguma açêo atende critério (≥ 90% qualidade 30d + zero incidente)?

### Documentaçêo
- [ ] Biblioteca de micro-vídeos com pelo menos 5 itens.
- [ ] Mapa de Processos atualizado com regras tácitas descobertas em produçêo (sempre aparecem novas).
- [ ] Versêo estável do system prompt promovida.

### Pessoas
- [ ] Champion sai liderando uma das reuniões semanais (sinal de propriedade).
- [ ] Time do cliente referenciando o agente pelo nome próximo a uma pessoa, nêo como ferramenta.

---

## Marco 30 dias

- [ ] Coletar métricas formais (planilha do baseline assinado, mesmas unidades).
- [ ] Reuniêo presencial ou videochamada com o dono — apresentaçêo em 4 slides.
- [ ] **Relatório de Payback 30 dias** entregue (estrutura abaixo).
- [ ] **Contrato de manutençêo assinado** — se ainda nêo foi.
- [ ] Avaliar adoçêo (% volume pelo agente vs. canal antigo). Alvo: ≥ 50% no D+30.
- [ ] Diário de Aprendizado fechado para o mês, vira insumo do plano D+60.

**Slides:**
1. Onde estávamos (baseline + data assinatura).
2. Onde estamos (números atuais).
3. ROI até aqui.
4. Próximos 30 dias.

---

## Marco 60 dias

- [ ] Coletar métricas formais.
- [ ] Relatório de Payback 60 dias.
- [ ] Reavaliar matriz HITL — propor subidas onde evidência permitir.
- [ ] Adoçêo alvo: ≥ 65%.
- [ ] Override alvo: ≤ 18%.
- [ ] Recuperaçêo se algum KPI < 60% da meta — visita extraordinária dentro de 7 dias.

---

## Marco 90 dias — fechamento formal da fase A

- [ ] Coletar métricas formais.
- [ ] **Relatório de Payback 90 dias** entregue formalmente — define se o projeto foi sucesso conforme critérios assinados no baseline.
- [ ] Plano de rollback testado pelo menos uma vez nesse período.
- [ ] Champion opera de forma independente em > 80% dos casos do mês.
- [ ] Manutençêo mensal entra em ritmo cruzeiro (cadência conforme tier contratado).
- [ ] Caso de uso documentado (com permissêo do cliente) para portfólio do aluno.
- [ ] Pedido de indicaçêo ao cliente: "quem mais do seu círculo tem dor parecida?".

**Status final da fase A:**
- [ ] Sistema em produçêo estável.
- [ ] Métricas dentro da meta acordada (ou plano de recuperaçêo ativo).
- [ ] Contrato de manutençêo ativo.
- [ ] Cliente referenceável.

---

# Exemplo preenchido — Marcos Polaris Bebidas

**Implementador:** [nome]
**Champion:** Cristiane Bertoldi
**Data deploy:** 03/junho/2026

### Status semana 4 (até 30/jun):

| Item | Status | Observaçêo |
|------|--------|------------|
| Override humano | ✓ 16% | meta < 18% ✓ |
| Adoçêo (% volume agente) | ✓ 71% | meta ≥ 50% no D+30 ✓✓ |
| Micro-vídeos gravados | ✓ 6 | meta ≥ 5 ✓ |
| Contrato manutençêo assinado | ✓ | tier intermediário R$ 2.400/mês |
| Plano de rollback testado | ✓ 22/jun | desligamento simulado, 11 min |
| Mapa de Processos v1.3 | ✓ | incorporou RT-05 (cliente do interior aceita boleto 21d) |
| Sistema em produçêo estável | ✓ | sem incidente crítico |

### Relatório de Payback — 30 dias

| Métrica | Baseline | Junho | Meta 90d | Status |
|---------|----------|-------|----------|--------|
| Tempo médio resposta | 47 / 11 min | 3,1 min | ≤ 5 min | ✓ atingido |
| Volume pelo agente | 0% | 78% | ≥ 70% | ✓ atingido |
| Pedidos perdidos/dia | 4 | 0,8 | ≤ 1 | ✓ atingido |
| Receita capturada | R$ 0 (perda R$ 33.440) | R$ 26.400 | R$ 22.000/mês | ✓ atingido |

Payback efetivo já no 1º mês — investimento R$ 42.000, ganho mensal observado R$ ~22.000 (economia operacional + receita recuperada), payback em **~1,9 mês**.

---

## Dicas de uso

- **Nêo pule itens "Antes do deploy".** Cada um já matou um projeto. Marcar item para "lembrar de fazer depois" sempre vira esquecimento e incidente.
- **Imprima e cole na parede do escritório do implementador.** Funciona como lembrete diário no ramp-up.
- **Compartilhe a versêo do cliente com o champion.** Ele acompanha o que falta e cobra junto.
- **Adapte o checklist por setor.** Clínica adiciona "verificar agenda no PEP", contábil "checar regime tributário". A coluna do meio adapta-se; o esqueleto nêo.
- **Use como instrumento de retro no 90.** O que ficou marcado tarde demais? O que faltou? Vira melhoria do método para o próximo cliente.
