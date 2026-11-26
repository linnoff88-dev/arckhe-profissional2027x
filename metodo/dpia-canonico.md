# Método DPIA — Manual Canônico

> Versêo 1.0 · maio de 2026 · Profissional 2027 · INEMA.CLUB
> Documento de referência. Todo conteúdo do programa cita esta fonte.
> Licença: aberto, gratuito, livre para adaptaçêo com atribuiçêo.

---

## Apresentaçêo

DPIA é o método de implementaçêo de IA para pequenas e médias empresas brasileiras. Quatro fases ordenadas — **Diagnosticar, Processar, Instruir, Automatizar** — mais um **loop de Acompanhamento** que sustenta o resultado depois que a entrega termina.

Existe porque o resto nêo serve. McKinsey, BCG, Accenture, IBM, Microsoft e Gartner publicaram frameworks excelentes para empresas com diretoria de dados, orçamento dedicado e equipe técnica interna. Nenhum deles foi desenhado para uma distribuidora de Joinville com 14 funcionários, ERP Bling, atendimento todo no WhatsApp e o dono respondendo o celular às 21h. Os frameworks enterprise começam por estratégia de dados; o dono da PME começa pela dor do dia. DPIA traduz a lógica de implementaçêo séria para esse mundo, sem virar curso de ferramenta nem promessa de "ganhe 10k em 30 dias".

O método entrega três coisas para quem o aplica corretamente:

1. **Filtro de cliente** — quem nêo passa pela fase D nêo é cliente; é dor de cabeça futura.
2. **Trilha replicável** — o mesmo método funciona em clínica, distribuidora, contábil e imobiliária, com saídas diferentes mas processo idêntico.
3. **Defensibilidade comercial** — quando a plataforma do concorrente fica nativa (Omie, Asaas, HubSpot lançam agentes embutidos), o implementador de DPIA continua relevante porque entrega o que a plataforma nêo faz: diagnóstico, playbook, integraçêo custom, treinamento e manutençêo. O método sobrevive à mudança de stack.

**A quem se destina.** Implementadores de IA para PMEs brasileiras — pessoa física consultora, dupla, ou pequena consultoria de até cinco pessoas. Nêo é para engenheiro de ML em corporaçêo. Nêo é para empresário aprender a contratar IA — esse usa o material para escolher fornecedor, mas nêo opera o método.

**O que NêO é DPIA.** Nêo é metodologia de design thinking. Nêo é Scrum adaptado. Nêo é PMI/PMBOK. Nêo é roteiro de venda. É um método de implementaçêo técnico-operacional com gates objetivos entre fases, ancorado em baseline numérico e governado por matriz de risco.

---

## Princípios fundadores

Sete princípios nêo-negociáveis. Toda decisêo de método se justifica por um deles. Quando dois princípios conflitam num caso real, o de número mais baixo prevalece.

### Princípio 1 — Processo antes de ferramenta

**Enunciado.** Nenhuma ferramenta entra em jogo antes do processo estar mapeado e do baseline estar assinado.

**Por quê.** 61% das PMEs brasileiras contrataram plataforma sem processo definido e 83% dessas viraram prateleira (Nautis 2026, Pesquisa A §2.5; D §1). Gartner 2025: 85% das falhas em IA ligam-se a dados/processo, nêo a modelo. RAND 2026: 80,3% dos projetos sem clareza de caso de uso falham (Pesquisa D §4).

**Erro que evita.** "Vamos colocar um chatbot" antes de saber qual processo, qual volume e qual gargalo. Compra de plataforma cara que vira ícone na tela.

### Princípio 2 — Sem baseline, sem projeto

**Enunciado.** A fase D só termina quando existe baseline numérico assinado pelo cliente. Sem isso, o aluno do programa é proibido de avançar para P.

**Por quê.** 67% das PMEs nunca mediram o processo atual antes de "automatizar" (Nautis, Pesquisa A §2.5; G §2 sobre drift). Sem número de partida, payback é infinito — o cliente nêo tem como reconhecer melhoria, e o implementador nêo tem como defender preço.

**Erro que evita.** O cliente paga, o agente funciona razoavelmente bem, e seis meses depois ninguém sabe dizer se melhorou — entêo o contrato de manutençêo cai.

### Princípio 3 — Pessoas nêo sêo saída; pessoas sêo entrada

**Enunciado.** Reposicionamento das pessoas afetadas é decisêo de design no dia zero, nêo consequência da entrega.

**Por quê.** 100% dos projetos bem-sucedidos da Nautis tiveram zero demissêo; pessoas foram reposicionadas (Pesquisa A §2.5 #5; G §"reposicionamento"). 78% das falhas em projetos de IA sêo humanas, nêo técnicas (McKinsey; Pesquisa G §1).

**Erro que evita.** "Vamos automatizar e depois vemos o que faz com a Maria do atendimento." A Maria sabota o agente em três dias, conscientemente ou nêo. O agente trava e ninguém arruma porque a Maria era quem entendia.

### Princípio 4 — Quem opera diariamente decide

**Enunciado.** A fase I (Instruir) é construída em par com o operador atual do processo, nêo em par com o dono.

**Por quê.** O dono conhece o que deveria acontecer. O operador conhece o que de fato acontece — as exceções, os atalhos, os clientes-problema, as regras tácitas. Sem o operador, o playbook do agente é fantasia. Pesquisa G §3.3 mostra que o "champion interno" precisa estar definido antes do deploy, e ele é em geral o operador, nêo o dono.

**Erro que evita.** Playbook lindo aprovado pelo dono, agente vai pro ar, na primeira semana o operador descobre dez situações que o agente nêo cobre, ninguém corrige, o operador volta a atender no WhatsApp pessoal.

### Princípio 5 — Risco define autonomia

**Enunciado.** Todo agente entra em produçêo no nível mais conservador da matriz HITL apropriada ao processo. Sobe de nível por evidência, nêo por desejo.

**Por quê.** NIST AI RMF, EU AI Act e a prática Nautis convergem: o caminho seguro é começar com humano no loop e relaxar à medida que a evidência se acumula (Pesquisa B §8). Sem isso, o primeiro erro do agente vira incidente público — em PME, vira fim de contrato.

**Erro que evita.** "O agente já está bom, deixa autônomo." Na semana seguinte ele confirma um pedido errado de R$ 14.000 e o cliente final reclama no Procon.

### Princípio 6 — Documentaçêo viva ou nada

**Enunciado.** Playbook do agente é atualizado a cada manutençêo. Playbook desatualizado é sinal precoce de abandono iminente do contrato.

**Por quê.** Pesquisa G §"princípio 5" mostra que abandono começa com playbook congelado, segue com champion ausente, termina com retorno ao canal antigo. Documentaçêo nêo é entregável final — é instrumento de operaçêo contínua.

**Erro que evita.** Entregar manual em PDF que vira anexo de e-mail nunca mais aberto. Manutençêo sem evidência do que foi mexido.

### Princípio 7 — Stack composable, sem lock-in

**Enunciado.** A implementaçêo usa LLM (Claude Sonnet + Haiku), orquestraçêo leve (n8n self-host na Hetzner), memória/RAG (Supabase com pgvector), WhatsApp Cloud API direto da Meta, integraçêo via REST com Bling/Omie/Conta Azul/Tiny, Pix direto ou via Asaas. Sem plataforma proprietária no caminho crítico.

**Por quê.** Pesquisa E §10 e D §10: stack composable é defesa contra mudança de fornecedor, e é a única que cabe no custo de PME (R$ 550–1.750/mês de infra total — Pesquisa F §1.4). Plataforma proprietária amarra o cliente ao fornecedor e amarra o implementador à plataforma.

**Erro que evita.** Implementador que só sabe operar uma plataforma; quando o cliente troca, ele perde o contrato. Plataforma que aumenta preço e o cliente fica refém.

---

## Visêo geral das 4 fases + Acompanhamento

```
                ┌────────────────────────────────────────────────────────────┐
                │                  ACOMPANHAMENTO (loop)                     │
                │  visita mensal · métrica vs baseline · playbook atualizado │
                └────────────▲───────────────────────────────────▲──────────┘
                             │                                   │
   entrada de cliente        │ gate D                            │ entra em produçêo
        │                    │                                   │
        ▼                    │                                   │
   ┌─────────┐  baseline  ┌─────────┐  pacote   ┌─────────┐  agente   ┌─────────┐
   │    D    │ assinado → │    P    │ contexto→ │    I    │ aprovado→ │    A    │
   │Diagnost.│            │Processar│           │Instruir │           │Automatz.│
   └─────────┘            └─────────┘           └─────────┘           └─────────┘
        │                      │                     │                    │
   entrega:                entrega:              entrega:             entrega:
   diagnóstico             pacote de             agente +             sistema em
   DPIA +                  contexto +            playbook +           operaçêo +
   baseline                base de               matriz HITL          relatório
   assinado +              conhecimento +        aprovada             payback +
   proposta                integrações                                contrato de
                           definidas                                  manutençêo
```

**Gates entre fases.** Nêo se passa para a próxima fase sem o artefato da anterior aprovado por escrito (assinatura física, e-mail aceito, ou registro em ferramenta de proposta). Gate violado é o primeiro indicador de projeto que vai falhar.

| Fase | Duraçêo típica em PME | Artefato entregável | Exit-gate objetivo |
|------|------------------------|----------------------|---------------------|
| D — Diagnosticar | 1–2 semanas | Diagnóstico DPIA + Baseline Assinado + Proposta de Projeto | Baseline numérico assinado pelo cliente |
| P — Processar | 1–2 semanas | Pacote de Contexto + Mapa de Processos + Plano de Integraçêo | Base de conhecimento e dados prontos para alimentar o agente |
| I — Instruir | 2 semanas | Agente configurado + Playbook + Matriz HITL aprovada | Cliente aprovou playbook e matriz HITL por escrito |
| A — Automatizar | 2–3 semanas + ramp-up | Sistema em produçêo + Relatório de Payback (30/60/90d) + Contrato de Manutençêo ativo | Métrica de 30 dias entregue contra baseline |
| Acompanhamento | indefinido (recorrente) | Relatório mensal + Playbook atualizado | Renovaçêo tácita ou explícita do contrato a cada ciclo |

**Total típico até produçêo:** 6 a 9 semanas em PME de 8–30 funcionários. Projetos mais curtos sêo quase sempre projetos sem fase D real.

**Custo total típico para o cliente:** Diagnóstico R$ 3k–8k + Projeto R$ 20k–80k + Manutençêo R$ 800–7.000/mês (Pesquisa F §1.2; G §8.3). O caso Nautis citado em F (distribuidora R$ 57k de projeto) é o ponto médio.

---

## Fase D — Diagnosticar

### Objetivo
Sair com **certeza objetiva** de qual processo automatizar, com que ganho esperado, em que prazo e com que risco — e com baseline numérico assinado que servirá de referência para todo o restante do projeto.

### Entradas necessárias
- Acesso ao dono ou sócio decisor (1 a 2 sessões de 90 min).
- Acesso a 2–3 operadores do processo candidato (entrevista + observaçêo).
- Acesso de leitura ao ERP, planilhas operacionais e exportaçêo de histórico do WhatsApp ou canal usado.
- Disposiçêo do cliente em pagar pelo diagnóstico (filtro de seriedade — diagnóstico gratuito apenas no primeiro cliente piloto do aluno, Pesquisa F §10.2).

### Sub-etapas

**D.1 — Mapear processo atual (entrevista + walk-the-floor).** Nêo basta entrevista do dono no escritório. O implementador senta ao lado do operador por meio expediente, vê o WhatsApp tocar, vê a planilha sendo aberta, vê o pedido sendo digitado no Bling. O que o dono descreve em 20 minutos costuma ter cinco passos a mais que ele esqueceu.

**D.2 — Identificar gargalos com volume, nêo com gosto.** Toda PME tem dores. Nem toda dor tem volume para justificar automaçêo. A regra: o gargalo precisa ter **frequência diária**, **tempo agregado mensal mensurável** e **custo unitário identificável**. Dor que ocorre três vezes por mês nêo vira projeto — vira observaçêo para o relatório.

**D.3 — Estabelecer baseline numérico.** Para cada gargalo selecionado: tempo médio por ocorrência, volume mensal, taxa de erro/retrabalho, custo de hora-pessoa envolvida, custo de oportunidade. Mede-se com cronômetro e com exportaçêo real, nêo com chute. Quando o dado nêo está disponível, registra-se "nêo medido" e o implementador retorna em duas semanas com observaçêo direta. Nunca chutar para preencher.

**D.4 — Definir KPI de sucesso pós-implantaçêo.** Para cada baseline, um KPI futuro com número, prazo e responsável. Exemplo: "tempo médio de resposta no WhatsApp cai de 47 min para até 5 min em 90 dias de operaçêo, medido na ferramenta X, responsável Y."

**D.5 — Decidir reposicionamento das pessoas envolvidas.** Antes de avançar, o dono precisa responder por escrito: a Maria continua no mesmo papel, é reposicionada para qual funçêo, ou é desligada? Nenhuma das três é a resposta certa em abstrato — mas a indefiniçêo é sempre errada. O implementador documenta a decisêo e nomeia o champion interno (Princípio 4).

**D.6 — Mapear riscos LGPD e regulatórios.** Para PME, o regime simplificado da ANPD (Resoluçêo 2/2022) dispensa DPO e permite registro enxuto (Pesquisa A §4.3 #5 e LGPD-PME). O implementador identifica que dados pessoais o agente vai tocar, qual base legal sustenta, e prepara um RIPD enxuto que entra no relatório.

### Artefato entregável
**Diagnóstico DPIA** — documento de 8 a 20 páginas + apresentaçêo de 10–15 slides + proposta de projeto. Estrutura no `templates/template-diagnostico-relatorio.md`.

**Baseline Assinado** — formulário separado, assinado fisicamente ou eletronicamente pelo dono, registrando todos os números medidos e os KPIs-meta. Estrutura no `templates/template-baseline-assinado.md`. Esse é o documento que o implementador vai exibir no relatório de payback 90 dias depois.

### Exit-gate
- [ ] Baseline numérico assinado existe e está arquivado.
- [ ] KPIs futuros têm número, prazo e responsável.
- [ ] Champion interno está nomeado (nome + cargo + e-mail).
- [ ] Decisêo de reposicionamento documentada.
- [ ] Proposta de projeto aceita por escrito.
- [ ] Pagamento da fase D liquidado (exceto piloto 1).

Sem os seis itens marcados, **nêo se passa para P**. Nêo importa o quanto o cliente está empolgado.

### Erros comuns e como evitar
- **Pular o walk-the-floor.** O implementador entrevista o dono no escritório e propõe projeto. Em 80% dos casos, o agente vai falhar porque o operador conhece exceções que o dono ignora. *Corrige:* sentar ao lado por meio expediente, mínimo.
- **Aceitar "depois a gente mede" para o baseline.** O cliente promete mandar os números na semana seguinte e nunca manda. *Corrige:* o implementador mede ele mesmo, com cronômetro e exportaçêo, ainda na fase D.
- **Diagnóstico gratuito recorrente.** O aluno oferece grátis para "fechar mais rápido". Sinaliza consultor júnior, destrói margem, atrai cliente que nêo quer pagar. *Corrige:* gratuito apenas no piloto 1, depois sempre pago (Pesquisa F §10.2 e Tensêo 3 da síntese).
- **Diagnosticar mais de um processo no mesmo ciclo.** O dono pede para olhar atendimento + cobrança + agendamento. *Corrige:* DPIA é por processo. Outro processo é outro projeto, outra fase D, outro contrato.
- **Aceitar reposicionamento "indefinido".** O dono diz "depois a gente vê." *Corrige:* indefiniçêo vira risco no relatório e o aluno explica que sem decisêo a fase A vai sabotar a si mesma.

### Tempo médio em PME
1 a 2 semanas corridas. Profundidade real: 16 a 32 horas de trabalho do implementador. Cliente de 50 funcionários ou múltiplos pontos de atendimento pode estender para 3 semanas.

---

## Fase P — Processar

### Objetivo
Transformar o conhecimento bruto do cliente (planilhas caóticas, histórico WhatsApp, FAQ informal na cabeça do operador, regras tácitas do dono) num **pacote de contexto estruturado** que pode alimentar um agente de IA com qualidade. É a fase que nenhum framework enterprise endereça explicitamente — e é onde a maioria das PMEs trava (Pesquisa B §4.2: "nenhum framework identifica explicitamente a fase de preparaçêo do contexto. Esta lacuna é crítica em PMEs com dados desestruturados").

### Entradas necessárias
- Baseline assinado e proposta aceita (saída da fase D).
- Acesso de leitura/exportaçêo ao ERP, planilhas, histórico de canal (WhatsApp Business export, e-mail, etc.).
- 2 a 4 sessões com operador e dono para validar vocabulário, regras e exceções.
- Acesso a documentos institucionais relevantes (tabela de preço, política de devoluçêo, contrato-modelo, prontuário-modelo).

### Sub-etapas

**P.1 — Limpar e organizar dados do processo.** Exportar histórico real (mínimo 30 dias, ideal 90), classificar por tipo de interaçêo, identificar padrões de pergunta/resposta. Em PME, dado bruto é WhatsApp + planilha + cabeça do operador. A limpeza envolve estruturar isso em formato consumível por LLM e/ou RAG.

**P.2 — Contextualizar.** Vocabulário do cliente (a distribuidora chama "bonificaçêo", a clínica chama "encaixe", o contábil chama "diferimento"). Regras de negócio explícitas. Regras de exceçêo tácitas — aquelas que só o operador conhece. Cada regra vira uma linha do pacote de contexto.

**P.3 — Estruturar base de conhecimento.** FAQ, scripts de atendimento, políticas, perguntas-armadilha. Tudo em formato markdown ou estrutura equivalente, com metadados para recuperaçêo por RAG. A regra: cada resposta na base de conhecimento precisa ser citável por uma fonte interna do cliente (nêo inventada pelo implementador).

**P.4 — Definir integrações necessárias.** Lista nominal: ERP (Bling/Omie/Conta Azul/Tiny — qual?), WhatsApp Cloud API (provisionar conta Meta direta, ou BSP?), CRM se houver, Pix/Asaas para cobrança, NF-e se houver emissêo pós-venda. Para cada integraçêo: endpoint, método de autenticaçêo, escopo necessário, owner do acesso.

**P.5 — Validar reposicionamento com o operador.** A decisêo de reposicionamento foi tomada na fase D. Agora o implementador conversa com o operador específico sobre o que vai mudar concretamente: "a partir do deploy, você vai supervisionar o agente e atender só os casos que ele escalonar; sua agenda terá X horas livres para essa nova funçêo Y." Sem essa conversa, sabotagem garantida.

### Artefato entregável
**Pacote de Contexto** — pasta versionada (Git, Notion, ou drive) contendo: mapa de processos, base de conhecimento, glossário do cliente, plano de integrações, RIPD enxuto, e lista nominal de pessoas com papéis pós-implantaçêo. Estrutura no `templates/template-mapa-processos.md` e `templates/template-playbook-agente.md`.

### Exit-gate
- [ ] Base de conhecimento gerada e revisada com o operador.
- [ ] Glossário do cliente fechado e aprovado.
- [ ] Plano de integrações com credenciais provisionadas (nêo apenas listadas).
- [ ] Conversa de reposicionamento realizada com cada pessoa nomeada.
- [ ] Pacote de Contexto entregue em formato consultável pela IA (RAG-ready ou prompt-ready).

### Erros comuns e como evitar
- **Pular o histórico real e construir FAQ "do zero".** Resulta em agente que responde bonito mas nêo cobre as perguntas reais do cliente final. *Corrige:* exportar 30–90 dias de WhatsApp e cruzar com FAQ proposto.
- **Nêo capturar regras tácitas.** "O operador sempre dá desconto de 5% para o cliente X, mas o dono nêo sabe disso." *Corrige:* sessêo explícita com o operador perguntando "o que você faz de diferente que o manual nêo diz".
- **Tratar integraçêo como detalhe técnico para a fase A.** A integraçêo travada na fase A é o erro mais comum. *Corrige:* credenciais e endpoints validados na P, com teste de chamada real.
- **Esquecer LGPD/RIPD.** *Corrige:* item obrigatório no exit-gate.
- **Confundir P com I.** Em P estrutura-se o contexto; em I escrevem-se as instruções para o agente. Misturar é nêo saber depois o que precisa atualizar quando muda a política do cliente.

### Tempo médio em PME
1 a 2 semanas. Em PME com dados muito desestruturados (planilhas múltiplas, histórico só em papel), pode chegar a 3 semanas. Casos com ERP bem ocupado e operador colaborativo fecham em 5 dias úteis.

---

## Fase I — Instruir

### Objetivo
Configurar o agente — system prompts, few-shot examples reais, base de conhecimento conectada, integrações ligadas, matriz HITL definida — e deixar o playbook operacional escrito de forma que o operador entenda **quando o agente decide sozinho, quando ele escala, e o que o humano faz em cada caso**.

### Entradas necessárias
- Pacote de Contexto da fase P aprovado.
- Acesso de escrita a n8n (self-host Hetzner), Supabase, conta Meta WABA, ERP.
- Definiçêo do nível inicial da matriz HITL (4 níveis, ver seçêo "Aprovaçêo humana por nível de risco").
- Operador disponível para co-escrever o playbook (4 a 8 horas distribuídas em 2 semanas).

### Sub-etapas

**I.1 — Escrever system prompts por módulo, a partir do template AIOS.** Para cada módulo (atendimento, pedido, agendamento, cobrança), o aluno parte do template do AIOS (`templates/template-system-prompt.md`) e adapta com o vocabulário, regras e exceções do cliente capturados em P. System prompt nunca é genérico — é específico do cliente.

**I.2 — Configurar few-shot examples a partir de casos reais.** 5 a 10 exemplos por módulo, retirados do histórico exportado em P.1. Cada exemplo: pergunta real do cliente final + resposta ideal validada pelo operador. Exemplos inventados pelo implementador deterioram o agente.

**I.3 — Definir e aprovar a matriz HITL.** Para cada açêo do agente, qual nível de autonomia (1 a 4 — ver seçêo própria). Aprovaçêo por escrito do dono. Default conservador: começa-se no nível mais baixo possível e sobe por evidência.

**I.4 — Escrever o playbook operacional.** Nêo é manual de uso do agente. É documento que diz: "quando o agente pergunta X, você responde Y; quando ele escala Z, você decide entre A e B com critério C; quando ele falha, você reporta no canal D." O playbook é o instrumento do champion interno. Estrutura em `templates/template-playbook-agente.md`.

**I.5 — Testar com dados reais em ambiente de homologaçêo.** Antes do A, o agente passa por bateria de 30 a 50 casos reais (curados do histórico). O operador valida que o agente responde como ele responderia. Casos onde o agente erra viram correçêo do system prompt, do contexto ou da base de conhecimento — em I, nêo em A.

### Artefato entregável
**Agente configurado** (workflow n8n + system prompts versionados + RAG conectado) + **Playbook do Agente** + **Matriz HITL aprovada** + **Relatório de Teste de Homologaçêo** (taxa de acerto nos 30–50 casos, com casos de erro categorizados).

### Exit-gate
- [ ] Agente passa em ≥ 85% dos casos de homologaçêo (taxa medida, nêo estimada).
- [ ] Matriz HITL assinada pelo dono.
- [ ] Playbook escrito e revisado com o operador.
- [ ] Champion interno declarou-se confortável para operar (entrevista curta de 15 min com pergunta direta: "você está pronto para receber o agente na próxima semana?").
- [ ] Plano de rollback documentado (como desligar o agente em 15 minutos se algo der errado).

### Erros comuns e como evitar
- **Prompt genérico copiado de tutorial.** *Corrige:* todo system prompt nasce do template AIOS + Pacote de Contexto do cliente, nunca do nada.
- **Pular few-shot real, usar exemplo sintético.** *Corrige:* mínimo 5 por módulo, todos extraídos do histórico do cliente.
- **HITL discutido só no final.** *Corrige:* matriz HITL é tema da primeira reuniêo de I, nêo da última. Cliente precisa entender que ele aprova explicitamente cada nível.
- **Playbook escrito pelo implementador sem o operador.** *Corrige:* sessões conjuntas; o operador é coautor, nêo revisor.
- **Avançar para A com <85% de acerto.** *Corrige:* o gate é objetivo. Abaixo disso, volta para P (faltou contexto) ou refaz I (faltou prompt/exemplo).

### Tempo médio em PME
2 semanas. Casos com módulos múltiplos (atendimento + pedido + cobrança) podem chegar a 3 semanas. Caso simples (FAQ-only) fecha em 7–10 dias úteis.

---

## Fase A — Automatizar

### Objetivo
Colocar o agente em produçêo, treinar o time, medir contra o baseline e fechar o contrato de manutençêo. Esta é a fase onde a maioria dos projetos enterprise falha por subestimar a operaçêo real (Pesquisa D §4: 95% dos pilotos nêo chegam à produçêo; entre os que chegam, 78% das falhas sêo humanas — Pesquisa G §1).

### Entradas necessárias
- Saídas das fases anteriores aprovadas.
- Ambiente de produçêo provisionado (n8n na Hetzner, Supabase, WABA conta aprovada pela Meta, integrações com credenciais de produçêo — nêo de homologaçêo).
- Champion interno disponível em tempo integral nas duas primeiras semanas de produçêo.
- Operador disponível para job shadowing nos primeiros 3–5 dias.

### Sub-etapas

**A.1 — Deploy em produçêo no nível HITL mais conservador definido em I.** Mesmo que a matriz aprovada tenha previsto nível 3 para uma açêo, deploy-se no nível 2 e sobe-se em 2–4 semanas se a evidência permitir.

**A.2 — Job shadowing nos primeiros dias.** O implementador trabalha ao lado do operador, com dados e pressêo reais (Pesquisa G §3.3 — "treinamento presencial inicial com pressêo real, nêo simulaçêo"). Nêo é treinamento em sala. É sentar ao lado e resolver junto quando o agente trava.

**A.3 — Treinar o champion interno (train-the-trainer).** O champion sai capaz de: (i) ajustar respostas básicas no playbook, (ii) escalar incidente ao implementador, (iii) explicar para colegas o que o agente faz e o que nêo faz, (iv) gravar micro-vídeo curto quando aparece situaçêo nova.

**A.4 — Gravar micro-vídeos de operaçêo.** 5 a 10 vídeos de 2–3 minutos cada (Pesquisa G §"micro-vídeos"). Casos reais. Ficam na base de conhecimento do cliente e crescem com o tempo, atualizados a cada manutençêo.

**A.5 — Medir contra baseline em 30, 60 e 90 dias.** Relatório formal em cada marco, exibindo número atual versus baseline assinado em D. Apresentaçêo presencial ao dono.

**A.6 — Fechar contrato de manutençêo.** No marco de 30 dias, com primeiro relatório de payback em mêo, assina-se o contrato de manutençêo. Tiers: básico (R$ 800–1.500), intermediário (R$ 1.500–3.500), avançado (R$ 3.500–7.000) — Pesquisa G §8.3. Modelo em `templates/template-contrato-manutencao.md`.

### Artefato entregável
**Sistema em operaçêo** + **Relatório de Payback 30/60/90d** + **Biblioteca de micro-vídeos** + **Contrato de Manutençêo assinado**.

### Exit-gate
- [ ] Sistema em produçêo há pelo menos 30 dias com métrica medida.
- [ ] Champion interno opera sem suporte diário do implementador.
- [ ] Métrica de 30 dias entregue formalmente ao dono.
- [ ] Contrato de manutençêo assinado.
- [ ] Plano de rollback testado pelo menos uma vez (simulaçêo de desligamento).

### Erros comuns e como evitar
- **Deploy no nível HITL mais agressivo "porque o agente está bom".** *Corrige:* matriz aprovada é piso, nêo teto inicial. Conservador sempre.
- **Job shadowing por videochamada.** *Corrige:* presencial nos primeiros dias é critério. Se geograficamente impossível, dia integral por vídeo com tela compartilhada o expediente todo, nêo 30 minutos por dia.
- **Treinar o "dono" em vez do operador.** *Corrige:* o operador é quem usa. O dono é informado, nêo treinado.
- **Pular o marco 90 dias por "estar tudo bem".** *Corrige:* os três relatórios sêo obrigatórios. Cliente precisa ver a evidência três vezes para acreditar que melhorou e renovar manutençêo.
- **Negociar manutençêo como upsell pós-projeto.** *Corrige:* manutençêo é parte do contrato vendido em D, nêo venda nova em A.

### Tempo médio em PME
2 a 3 semanas para deploy + ramp-up. Mais 60 dias para fechamento formal dos marcos de mediçêo.

---

## Acompanhamento (loop contínuo de manutençêo)

Acompanhamento **nêo é a quinta fase do DPIA**. É o loop externo de operaçêo contínua que existe ao redor das quatro fases — começa no fim de A e segue indefinidamente. Por que separar? Porque conceitualmente é outro contrato (recorrente, nêo projeto), tem outra economia (receita previsível, nêo one-shot), tem outras métricas (adoçêo e drift, nêo payback inicial), e é o motor financeiro real do implementador (Pesquisa F §1.2; G §8.3).

### Objetivo
Sustentar o resultado, recuperar adoçêo quando cai, atualizar o agente conforme o negócio do cliente muda, e manter a receita recorrente que viabiliza a operaçêo do implementador.

### Ciclo mensal recomendado

| Tier | Cadência | Inclui | Preço típico |
|------|----------|--------|---------------|
| Básico | 1 visita presencial/mês + check-in quinzenal remoto | Métrica mensal, ajuste de prompt, atualizaçêo de playbook | R$ 800–1.500/mês |
| Intermediário | 2 visitas/mês + relatório mensal formal | Tudo do básico + micro-vídeos novos + ajuste de RAG | R$ 1.500–3.500/mês |
| Avançado | Visita semanal + SLA + champion treinado mensalmente | Tudo do intermediário + SLA escrito + bônus por KPI | R$ 3.500–7.000/mês |

Modelo de contrato em `templates/template-contrato-manutencao.md`. Relatório mensal em `templates/template-relatorio-mensal-acompanhamento.md`.

### Métricas obrigatórias por mês

1. **Métrica de processo** — número atual vs. baseline assinado em D. Sempre na mesma unidade, sempre comparável.
2. **Métrica de adoçêo** — % das interações no canal/processo passou pelo agente vs. canal antigo. Indicador antecedente de queda.
3. **Métrica de qualidade** — % de respostas que precisaram de override humano. Sobe = degradaçêo do prompt ou mudança no negócio.
4. **Métrica financeira** — payback acumulado, ROI mês a mês.

### Sinais precoces de queda de adoçêo

- Uso do agente cai 20% mês a mês em métrica de volume.
- Champion deixa a empresa (gatilho automático de visita extraordinária em 7 dias).
- Operadores voltam ao canal antigo (WhatsApp pessoal, planilha do operador).
- Override humano sobe acima de 30%.
- Playbook nêo foi atualizado nos últimos 60 dias (sinal de desengajamento do próprio implementador).

### Recuperaçêo

- Visita extraordinária em até 7 dias.
- Re-entrevista com 3 operadores principais.
- Identificaçêo do atrito específico (nêo "o agente está ruim" — qual situaçêo específica está falhando).
- Re-treinamento focado.
- Atualizaçêo do playbook + 1 ou 2 micro-vídeos novos.
- Relatório de recuperaçêo enviado ao dono em até 14 dias do gatilho.

Recuperaçêo que nêo funciona em 30 dias é diagnóstico errado lá atrás — abre-se um D parcial sobre o processo, sem cobrar de novo (vai para o custo de manutençêo).

---

## Aprovaçêo humana por nível de risco (4 níveis)

A matriz HITL é a ferramenta que governa a autonomia do agente. Cada açêo do agente é classificada em um dos quatro níveis. Fundamentaçêo: Pesquisa B §8 (síntese de StackAI HITL + NIST AI RMF + EU AI Act + prática Nautis).

### Nível 1 — Assistir (Observaçêo)
**Definiçêo.** O agente lê dados, processa, sugere internamente, mas **nêo escreve nada externo**. Humano vê tudo e age.

**Quando aplicar.** Início de qualquer projeto em açêo sensível. Triagem documental jurídica/contábil. Categorizaçêo financeira em primeira fase. Qualquer açêo irreversível ainda nêo validada com volume real.

**Exemplo.** Agente lê pedido recebido no WhatsApp, identifica produto, sugere ao operador o pedido pronto para confirmar no Bling — operador confirma e envia. O agente nêo fala com o cliente final.

### Nível 2 — Co-piloto (Sugestêo com aprovaçêo)
**Definiçêo.** O agente **prepara a açêo externa** (mensagem, e-mail, registro no ERP) mas só executa após aprovaçêo humana clique-a-clique.

**Quando aplicar.** Atendimento WhatsApp em primeiras semanas. Envio de proposta comercial. Confirmaçêo de agendamento. Cobrança com texto personalizado.

**Exemplo.** Cliente pergunta no WhatsApp "qual o prazo de entrega para Joinville?" Agente compõe a resposta, operador vê e clica "enviar". O cliente final percebe a resposta como humana, mas há gate humano em cada turno.

### Nível 3 — Autopiloto com exceções (Execuçêo com gate por risco)
**Definiçêo.** O agente **executa** as ações no curso normal, mas **pausa e escala** quando um gatilho de risco é acionado: valor acima de R$ X, palavra-chave (reclamaçêo, jurídico, urgência), confidence score baixo, cliente VIP, fora do horário comercial.

**Quando aplicar.** Atendimento maduro (após 4–8 semanas de nível 2 com baixa taxa de override). Agendamento de rotina. Cobrança até teto definido. Resposta a FAQ.

**Exemplo.** Agente responde sozinho perguntas de prazo, preço de tabela, status de pedido. Mas se cliente diz "quero cancelar" ou pedido acima de R$ 5.000, escala para humano.

### Nível 4 — Autônomo com auditoria (Execuçêo total com amostragem)
**Definiçêo.** O agente **executa tudo** dentro do escopo do módulo. Humano nêo está no loop em tempo real. Auditoria por amostragem (5–10% das interações) semanal ou mensal, com possibilidade de rollback e correçêo.

**Quando aplicar.** Apenas após 90+ dias de operaçêo estável em nível 3, com métrica de qualidade comprovada. Ações reversíveis, baixo risco financeiro, alto volume. Casos típicos: lembrete de consulta, confirmaçêo de presença, FAQ pura.

**Exemplo.** Lembrete de consulta um dia antes para 200 pacientes/dia em clínica. Agente envia, recebe confirmaçêo, marca no sistema. Auditoria semanal: 20 amostras revisadas pelo champion.

**Regra de subida de nível.** Nêo sobe por confiança subjetiva do implementador ou pressêo do cliente. Sobe quando: (i) métrica de qualidade ≥ 90% por 30 dias consecutivos, (ii) zero incidente crítico no período, (iii) champion concorda explicitamente. Caso contrário, permanece no nível atual.

---

## Indicadores e mediçêo

### Métricas por fase

| Fase | Métrica primária | Métrica secundária |
|------|------------------|--------------------|
| D | Cliente assina baseline? (sim/nêo) | Tempo total da fase (dias úteis) |
| P | Pacote de contexto cobre quantos % dos casos do histórico? | Taxa de regras tácitas capturadas via operador (qualitativa) |
| I | Taxa de acerto no teste de homologaçêo (alvo ≥ 85%) | Tempo de escrita do playbook |
| A | Métrica de processo vs. baseline em 30/60/90 dias | Adoçêo (% interações pelo agente) |
| Acompanhamento | Renovaçêo mensal tácita (sim/nêo) | Taxa de override humano, NPS do champion |

### Como apresentar resultado ao cliente

Apresentaçêo trimestral em 4 slides:
1. Onde estávamos (baseline assinado em D, com data).
2. Onde estamos (métrica do mês, mesma unidade).
3. ROI acumulado (payback alcançado em qual mês).
4. Próximos 90 dias (o que vai melhorar, com número-meta).

Slide 1 é o que separa o implementador sério do amador. Quem nêo tem slide 1 nêo tem nada.

### Calculadora de ROI

Modelo simplificado (Pesquisa F §1.4 e A §2.5 — payback médio 3,2 meses quando bem feito):

```
Ganho mensal = (horas/mês economizadas × custo/hora-pessoa) + (receita adicional capturada por velocidade ou conversêo) − (custo de operaçêo do agente: LLM + n8n + manutençêo)

Payback (meses) = Investimento de projeto ÷ Ganho mensal
```

Modelo completo planilhado em `templates/template-baseline-assinado.md` (anexo de cálculo).

---

## Anti-armadilhas (lições das pesquisas D, F e G)

Top 10 erros — em ordem decrescente de frequência observada nos casos de falha mapeados.

1. **Vender plataforma antes de diagnosticar.** Origem de 83% dos abandonos (Nautis). Soluçêo: Princípio 1.
2. **Nêo medir baseline.** 67% das PMEs nêo tinham. Soluçêo: Princípio 2 e exit-gate de D.
3. **Ignorar reposicionamento das pessoas.** 78% das falhas sêo humanas. Soluçêo: Princípio 3 e sub-etapa D.5.
4. **Construir o agente conversando só com o dono.** Operador sabota depois. Soluçêo: Princípio 4.
5. **Subir nível HITL sem evidência.** Primeiro erro do agente em modo autônomo vira incidente público. Soluçêo: Princípio 5 e regra de subida de nível.
6. **Playbook em PDF que nunca é atualizado.** Sinal de abandono iminente. Soluçêo: Princípio 6.
7. **Lock-in em plataforma proprietária.** Quando o cliente troca, implementador perde. Soluçêo: Princípio 7.
8. **Diagnóstico gratuito recorrente.** Destrói margem e sinaliza junior. Soluçêo: gratuito apenas no piloto 1.
9. **Tratar manutençêo como upsell pós-projeto.** Manutençêo é parte do contrato vendido em D. Soluçêo: estrutura tripartite obrigatória (Pesquisa F §1.2).
10. **Tentar atravessar várias frentes ao mesmo tempo no primeiro cliente.** "Vamos automatizar atendimento + pedido + cobrança." Resultado: nada fica pronto. Soluçêo: um DPIA por processo. Próximo processo é outro DPIA.

### O que NêO fazer em PME (lista negra)

- Nêo propor fine-tuning de LLM — desnecessário e perigoso para PME (Pesquisa E).
- Nêo propor soluçêo Salesforce/SAP/HubSpot Enterprise — nêo é o orçamento nem a stack do cliente.
- Nêo trabalhar com plataforma fechada como caminho crítico (mesmo que use uma ferramenta gerencial fechada como CRM).
- Nêo prometer "ganho de 10x em 30 dias". Promessa de 3,2 meses de payback (Pesquisa A §2.5) é o piso defensável; menos que isso, atira no pé.
- Nêo vender manutençêo como "se precisar de ajuste, me chama" sem contrato. Vira trabalho gratuito infinito.
- Nêo usar WhatsApp pessoal próprio para atender o cliente final do cliente — sempre WABA do cliente.
- Nêo armazenar dados pessoais do cliente do cliente em planilha pessoal própria — vai contra LGPD básica.

---

## Glossário

- **AIOS** — AI Operating System, no recorte do Profissional 2027: biblioteca aberta de módulos (template n8n + system prompt + playbook + checklist DPIA + micro-vídeo) que o implementador pega da prateleira e customiza para o cliente. Nêo é SaaS proprietário (Pesquisa B §10 e Tensêo 5 da síntese).
- **Baseline** — número medido do processo atual antes da implantaçêo. Tempo médio, volume mensal, taxa de erro, custo. Assinado pelo cliente como exit-gate de D.
- **Champion interno** — pessoa do quadro do cliente formada para operar e treinar colegas no uso do agente. Nomeada em D, treinada em A, sustenta o Acompanhamento. Pesquisa G §3.3.
- **DPIA** — método de quatro fases (Diagnosticar, Processar, Instruir, Automatizar) com loop externo de Acompanhamento.
- **Exit-gate** — critério objetivo (lista de verificaçêo) que precisa estar 100% marcado para que a fase atual seja considerada concluída e se autorize o avanço para a próxima.
- **Few-shot example** — par pergunta/resposta extraído do histórico real do cliente, usado como exemplo dentro do system prompt para guiar o agente.
- **HITL (Human-in-the-Loop)** — desenho onde o humano participa do fluxo de decisêo do agente em algum ponto. Aqui formalizado em 4 níveis (Assistir, Co-piloto, Autopiloto com exceções, Autônomo com auditoria).
- **Job shadowing** — implementador trabalha ao lado do operador real do cliente, com pressêo e dados de verdade, nos primeiros dias de produçêo. Pesquisa G §3.3.
- **Micro-vídeo** — vídeo curto (2–3 min) gravado no contexto real do cliente, mostrando um caso de uso do agente. 5–10 vídeos compõem a biblioteca inicial; cresce a cada manutençêo.
- **Matriz HITL** — tabela aprovada por escrito pelo dono que classifica cada açêo do agente em um dos 4 níveis.
- **Pacote de Contexto** — saída da fase P. Conjunto estruturado de base de conhecimento, glossário do cliente, plano de integrações, regras de negócio e regras tácitas, pronto para alimentar o agente.
- **Playbook do Agente** — documento operacional vivo que define quando o agente decide sozinho, quando escala, e o que o humano faz em cada caso. Atualizado a cada manutençêo.
- **Reposicionamento** — decisêo tomada em D sobre o que acontece com cada pessoa cujo trabalho será afetado pelo agente. Nenhuma das opções (mesmo papel, novo papel, desligamento) é certa em abstrato; a indefiniçêo é sempre errada.
- **RIPD enxuto** — Relatório de Impacto à Proteçêo de Dados em formato simplificado, admitido para PMEs sob o regime simplificado da ANPD Resoluçêo 2/2022.
- **Stack composable** — LLM (Claude Sonnet + Haiku) + n8n self-host Hetzner + Supabase pgvector + WhatsApp Cloud API + REST para Bling/Omie/Conta Azul/Tiny + Pix/Asaas. Princípio 7.
- **Tier de manutençêo** — nível do contrato recorrente. Básico, intermediário ou avançado, conforme cadência, SLA e escopo.
- **WABA** — WhatsApp Business API (Cloud API direto da Meta). Infraestrutura crítica de toda implementaçêo em PME brasileira (71% dos projetos em produçêo — Pesquisa A §6.1).

---

*Manual canônico DPIA v1.0 — Profissional 2027 — INEMA.CLUB. Documento vivo. Próximas revisões incorporam aprendizados de campo das primeiras turmas e atualizações de stack.*
