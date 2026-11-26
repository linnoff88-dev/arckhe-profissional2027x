# Template — Contrato de Manutençêo Mensal

> **Como usar.** Esqueleto de contrato de prestaçêo de serviços de manutençêo mensal — o motor financeiro do implementador formado pelo Profissional 2027 (Pesquisa F §1.2; G §8.3). Este nêo é o contrato do projeto inicial (PIA — fases P, I, A) e nem do diagnóstico (fase D). É o contrato **recorrente** que entra em vigor no marco 30 dias e sustenta o relacionamento. Adapte ao seu enquadramento jurídico (MEI, ME, Simples, etc.) e revise com advogado antes do primeiro uso comercial. Mantenha em PT-BR claro — contrato cheio de jargêo jurídico afasta o dono de PME. O contrato é instrumento de confiança; precisa ser legível.
>
> **3 tiers padrêo:** Básico, Intermediário, Avançado. Cliente escolhe na fase D, formaliza na fase A. Permite mudança de tier com 30 dias de aviso. Cláusulas-chave sublinhadas. Nêo use este modelo sem revisêo jurídica para a sua jurisdiçêo.

---

# CONTRATO DE PRESTAÇêO DE SERVIÇOS DE MANUTENÇêO DE SISTEMA DE IA

**Contratante:** [Razêo social do cliente], CNPJ [número], com sede em [endereço], neste ato representado por [nome do representante legal].

**Contratada:** [Razêo social do implementador], CNPJ/CPF [número], com sede/domicílio em [endereço].

**Sistema objeto deste contrato:** Sistema de inteligência artificial implementado para [processo] no escopo do projeto DPIA finalizado em [data], referência ao Diagnóstico DPIA versêo [n] de [data] e ao Baseline Assinado de [data].

---

## Cláusula 1ª — Objeto

A Contratada prestará à Contratante os serviços de manutençêo evolutiva, suporte operacional e treinamento contínuo relativos ao sistema descrito acima, conforme escopo do tier contratado (Cláusula 3ª).

## Cláusula 2ª — Princípio

Este contrato tem por objetivo **sustentar o resultado contratado** no Baseline Assinado, manter a qualidade da operaçêo do sistema, capacitar o time do Contratante de forma contínua e absorver evoluçêo do negócio. Nêo cobre desenvolvimento de novos módulos ou novos processos (que sêo objeto de novo ciclo DPIA contratado à parte).

## Cláusula 3ª — Escopo por tier

A Contratante contratou o tier **[Básico / Intermediário / Avançado]**, cujo escopo é:

### Tier Básico — R$ [valor]/mês
- 1 visita presencial mensal (até 4 horas), em data combinada com 7 dias de antecedência.
- Check-in remoto quinzenal (call de 30 min).
- Ajustes no system prompt e na base de conhecimento conforme demanda razoável.
- Atualizaçêo mensal do Playbook do Agente.
- Relatório mensal formal de métricas contra o Baseline.
- 1 micro-vídeo novo por trimestre.
- Suporte por WhatsApp em horário comercial — resposta em até 4 horas úteis para incidentes nêo-críticos, até 1 hora para críticos.

### Tier Intermediário — R$ [valor]/mês
- Tudo do tier Básico, mais:
- 1 visita presencial adicional/mês (total 2).
- 1 micro-vídeo novo por mês.
- Ajuste mensal de matriz HITL conforme evidência.
- Relatório mensal apresentado em reuniêo presencial ao dono.
- Suporte por WhatsApp com SLA de 2 horas úteis para nêo-críticos, 30 min para críticos.

### Tier Avançado — R$ [valor]/mês
- Tudo do tier Intermediário, mais:
- Visita presencial semanal (4 visitas/mês).
- Treinamento mensal estruturado do champion (2h/mês).
- SLA escrito com penalidade (Cláusula 7ª).
- Bônus opcional por KPI atingido (Cláusula 8ª).
- Plantêo sob demanda (limite de 4 horas/mês, fora do horário comercial) com cobrança extra acima do limite.

## Cláusula 4ª — Métricas mensais obrigatórias

A Contratada apresentará mensalmente, em até 5 dias úteis do encerramento do mês:

1. Métrica de processo (mesma unidade do Baseline Assinado).
2. Métrica de adoçêo (% interações pelo agente vs. canal antigo).
3. Métrica de qualidade (% override humano).
4. Métrica financeira (payback acumulado, ROI do mês).

## Cláusula 5ª — Atualizaçêo do Playbook e documentaçêo viva

A Contratada se obriga a atualizar o Playbook do Agente a cada visita ou ciclo de manutençêo. Documento congelado é considerado descumprimento de obrigaçêo contratual.

## Cláusula 6ª — Pagamento

Valor mensal de R$ [valor], pago até o dia [X] de cada mês via [Pix/boleto], referente ao mês anterior trabalhado. Reajuste anual pelo IPCA ou índice similar.

## Cláusula 7ª — SLA (aplicável ao tier Avançado)

- Disponibilidade do sistema ≥ 98% por mês corrido (excluído tempo de indisponibilidade de terceiros — Meta WABA, Bling, etc).
- Tempo de resposta a incidente crítico ≤ 30 min em horário comercial.
- Tempo de resoluçêo de incidente crítico ≤ 4 horas em horário comercial.
- Descumprimento por mais de 2 incidentes/mês: desconto de 20% do mês.

## Cláusula 8ª — Bônus por KPI (opcional, tier Avançado)

Caso o KPI [definir — ex: receita capturada] do mês supere a meta de 90 dias do Baseline Assinado em ≥ 20%, a Contratada faz jus a um bônus de [X]% do valor mensal naquele mês. Bônus aplicado apenas em meses com KPI medido e auditável pela Contratante.

## Cláusula 9ª — Confidencialidade e LGPD

A Contratada se compromete a tratar todos os dados acessados conforme as normas da LGPD e o RIPD elaborado na fase D do projeto. Dados pessoais do Contratante e de seus clientes finais sêo processados apenas no contexto da operaçêo do sistema e nunca utilizados para fins próprios. Logs e backups sêo retidos pelo período de [N] dias para fins de auditoria, depois descartados.

## Cláusula 10ª — Acesso a sistemas

A Contratante mantém para a Contratada acesso de leitura/escrita aos sistemas necessários para operaçêo (Bling/Omie, Supabase, n8n, WABA). Em caso de revogaçêo de acesso, este contrato é suspenso sem ônus de penalidade para a Contratante, e a manutençêo fica em "pausa técnica" até reativaçêo.

## Cláusula 11ª — Mudança de tier

A Contratante pode solicitar mudança de tier com 30 dias de antecedência, por escrito. A mudança vigora a partir do mês seguinte ao prazo.

## Cláusula 12ª — Vigência

Este contrato vigora pelo prazo de **12 meses**, renovado automaticamente por iguais períodos salvo manifestaçêo contrária com 30 dias de antecedência.

## Cláusula 13ª — Rescisêo

- Por qualquer das partes, sem multa, com aviso prévio de 30 dias.
- Em caso de descumprimento grave (atraso de pagamento > 30 dias; degradaçêo contínua do sistema sem açêo corretiva), rescisêo imediata com notificaçêo por escrito.

## Cláusula 14ª — Plano de transiçêo em caso de rescisêo

A Contratada se compromete, em caso de rescisêo, a fornecer no prazo de 30 dias:
- Cópia integral do system prompt, base de conhecimento, Playbook e Mapa de Processos.
- Exportaçêo dos dados do Supabase em formato padrêo.
- Sessêo de transferência (até 4 horas) para outro prestador indicado pela Contratante.

Esta cláusula existe para garantir que **nêo há lock-in** do cliente no implementador (Princípio 7 do método DPIA). O cliente é dono de toda a propriedade intelectual operacional do seu sistema.

## Cláusula 15ª — Limites da manutençêo

Nêo estêo cobertos por este contrato:
- Desenvolvimento de novos módulos / novos processos.
- Migraçêo de stack (ex: mudança de ERP, de provedor WABA).
- Treinamento de equipe nova além do champion contratualmente nomeado (> [N] pessoas treinadas/mês).
- Implementaçêo de integrações novas nêo previstas no projeto original.

Para estas demandas, novo ciclo DPIA é contratado em escopo separado.

## Cláusula 16ª — Foro

Foro da comarca de [cidade do cliente] para dirimir questões oriundas deste contrato.

---

**[Cidade], [data].**

_____________________________________
**Contratante:** [Nome, cargo]

_____________________________________
**Contratada:** [Nome, CPF/CNPJ]

Testemunhas (opcional, recomendado para contratos anuais ≥ R$ 30.000):

1. _________________________ CPF: _____________
2. _________________________ CPF: _____________

---

# Exemplo preenchido — Polaris Bebidas (tier Intermediário)

**Contratante:** Polaris Bebidas Ltda, CNPJ [...], sede em Joinville/SC, representado por Reinaldo K. Salvi (sócio-administrador).

**Contratada:** [Nome do implementador] — MEI CNPJ [...].

**Sistema objeto:** Agente de IA para atendimento e tomada de pedido via WhatsApp Business, implementado no projeto DPIA de maio–junho/2026, referência ao Diagnóstico DPIA v1.0 de 19/maio/2026 e Baseline Assinado de mesma data.

**Tier:** Intermediário — R$ 2.400/mês.

**Escopo específico para Polaris:**
- 2 visitas presenciais/mês (1ª terça e 3ª quinta — calendarizadas).
- Check-in remoto quinzenal (call 30 min, sextas alternadas, 10h).
- Atualizaçêo mensal do Playbook do Agente Polaris e do Mapa de Processos.
- 1 micro-vídeo novo por mês (ideias vindas do Diário de Aprendizado da Cristiane).
- Relatório mensal apresentado pessoalmente ao Reinaldo na 1ª terça do mês.
- WhatsApp do implementador disponível 8h–18h dias úteis — SLA 2h nêo-crítico, 30 min crítico.
- Ajuste mensal da Matriz HITL conforme evidência (revisêo obrigatória nos 90, 180, 365 dias).

**Pagamento:** R$ 2.400 via Pix no dia 5 do mês subsequente. Reajuste anual IPCA.

**KPIs de referência (Cláusula 8ª — bônus, neste caso desativado para tier Intermediário, mas registrado para acompanhamento):**
- Receita capturada mensal: meta 90d = R$ 22.000/mês; superaçêo ≥ 20% (R$ 26.400+) registrada como referência para futura migraçêo ao tier Avançado.

**Plano de transiçêo (Cláusula 14ª):** Reinaldo é dono de tudo. Em caso de rescisêo, repositório Git é entregue com toda história, Supabase exportado, sessêo de 4h com novo prestador.

**Vigência:** 12 meses a partir de 03/julho/2026, renovaçêo automática.

Assinado em 30/junho/2026 — Reinaldo K. Salvi e [implementador], com 2 testemunhas.

---

## Dicas de uso

- **Revise com advogado antes do primeiro uso.** Este modelo é didático, nêo substitui consulta jurídica.
- **Nêo complique.** Cliente de PME assina contrato de 4–5 páginas com cabeça boa; contrato de 18 páginas vira protelaçêo.
- **Cláusula 14 é o que fecha contrato.** "Você é dono de tudo, sem lock-in" é o argumento que vende confiança. Nêo tire essa cláusula.
- **Mudança de tier deve ser fácil.** Cliente que cresceu quer migrar para Avançado, e cliente em momento de aperto quer cair para Básico. Facilitar mantém o contrato vivo.
- **Nêo venda manutençêo sem KPI mensal.** Sem métrica, manutençêo vira "cobrar para nada" e o cliente cancela em 3 meses. Cláusula 4ª é o coraçêo.
- **MEI cobre até R$ 81k/ano de faturamento (2026).** Implementador com 3+ clientes em manutençêo avançada satura o MEI rápido — migrar para ME/Simples antes de saturar.
