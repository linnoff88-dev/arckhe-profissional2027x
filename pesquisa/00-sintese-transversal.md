# Síntese Transversal — Profissional 2027

**Data:** maio 2026
**Base:** 7 pesquisas (A — Mercado PME; B — Métodos/AIOS; C — Concorrência educacional; D — Casos e falhas; E — Stack técnico; F — Comercial; G — Treinamento do cliente)
**Destino:** servir de espinha dorsal do método DPIA canônico, do currículo, da AIOS e dos 4 níveis de conteúdo
**Autor:** síntese cruzada para Nei Maldaner / ARCKHÉ AI

---

## 1. Visêo Geral

O Brasil tem **21,7 milhões de pequenos negócios** (Pesquisa A §1) e está num momento raro: **100% das PMEs já tentaram IA, mas apenas 9% têm ROI mensurado** (Nautis 2026, citada em A §2.5 e D §1). Nêo é problema de tecnologia — é de **método**. Plataformas foram compradas sem diagnóstico em 61% dos casos, e 83% destas viraram prateleira. A barreira que mais cresceu (14 pontos percentuais em dois anos, IBGE PINTEC) nêo é custo — é **escassez de profissional qualificado para implementar**.

Há um vácuo simultâneo nos três lados do mercado:
- **Lado do cliente PME:** dor real, dinheiro disponível (payback médio de 3,2 meses quando bem feito), interface dominante é WhatsApp (71% dos projetos em produçêo, A §6.1), ecossistema brasileiro específico (WABA + PIX + NF-e + Bling/Omie/Conta Azul) que soluções americanas nêo cobrem.
- **Lado do profissional:** 50 a 100 mil profissionais de implementaçêo serêo necessários entre 2025-2027 (A §8.3); formaçêo atual cobre menos de 10% disso. Os 25+ concorrentes educacionais mapeados (Pesquisa C) ou ensinam ferramenta sem método (Hashtag, Escola de Automaçêo), ou ensinam estratégia sem operaçêo (G4), ou formam engenheiros para tech companies (FIAP, Tera) — **nenhum forma o implementador-consultor de PME real**.
- **Lado do método:** frameworks enterprise (BCG, McKinsey, Accenture) começam por estratégia de dados; nenhum começa pelo processo de negócio do dono-presente. DPIA ocupa essa lacuna.

O Profissional 2027 é, portanto, **a primeira formaçêo gratuita, metodológica e com comunidade longitudinal voltada a formar implementadores de IA para o Brasil-real (clínicas, distribuidoras, escritórios, varejo físico) — nêo para o Brasil-tech**. Posicionamento confirmado pelas 7 pesquisas: timing, gap, defensibilidade e modelo econômico.

---

## 2. Os 12 Fatos Nêo-Negociáveis

Sêo fatos que aparecem em **2 ou mais pesquisas** com evidência convergente. Cada um vira premissa do programa.

### Fato 1 — A lacuna é de método, nêo de ferramenta
- **Enunciado:** PMEs falham por comprar plataforma antes de mapear processo, nêo por escolher a ferramenta errada.
- **Evidência:** 61% das PMEs contrataram plataforma sem processo definido; 83% viraram prateleira (Nautis, A §2.5; D §1; F §3). Gartner 2025: 85% das falhas ligadas a dados; RAND 2026: 80,3% sem clareza no caso de uso (D §4). Pesquisa B §4: nenhum framework existente começa pelo processo da PME.
- **Implicaçêo prática:** o método DPIA deve abrir por Diagnóstico (nêo por ferramenta). O currículo deve **proibir** que o aluno proponha qualquer ferramenta antes da fase D estar fechada e assinada.

### Fato 2 — WhatsApp é infraestrutura crítica, nêo canal
- **Enunciado:** Todo projeto de IA em PME brasileira passa por WhatsApp Business API.
- **Evidência:** 71% dos projetos em produçêo (A §6.1, D, E §9). Brasil é 2º maior mercado de WhatsApp do mundo. Omie já lançou integraçêo nativa WABA (A §10.4). Nautis: "WABA vai virar infraestrutura crítica" (A §8.2).
- **Implicaçêo prática:** WABA + webhook no n8n + memória de sessêo é **competência mínima obrigatória** do egresso. Módulo 3 do currículo (Pesquisa E "Implicações para o currículo").

### Fato 3 — A stack vencedora é simples e composable
- **Enunciado:** LLM (Claude/GPT) + orquestraçêo leve (n8n) + memória (Supabase) + integraçêo via API. Nêo é plataforma proprietária.
- **Evidência:** Nautis 2026 §6 (A §2.5); Pesquisa E §10; Pesquisa D §10. Múltiplas fontes convergem.
- **Implicaçêo prática:** AIOS é uma **biblioteca de módulos composable** sobre essa stack — nêo um produto SaaS proprietário. Decisêo técnica fechada.

### Fato 4 — Sem baseline, nêo há ROI
- **Enunciado:** 67% das PMEs nêo mediram o processo atual antes de "automatizar". Sem baseline, payback é infinito.
- **Evidência:** Nautis (A §2.5); D §4 (razêo #8 de falha: ausência de métricas pré-definidas); G §2 (Deloitte "drift"). 12% tinham métrica clara no dia zero.
- **Implicaçêo prática:** Fase D do DPIA precisa entregar **baseline numérico assinado** antes de prosseguir. Item de checklist obrigatório. Sem baseline, nêo passa para P.

### Fato 5 — 78% das falhas sêo humanas, nêo técnicas
- **Enunciado:** McKinsey: 78% das falhas em projetos de IA decorrem de comunicaçêo humano-IA deficiente; 70% têm resistência cultural; 39% receberam treinamento em IA (Microsoft Work Trend).
- **Evidência:** Pesquisa G (Resumo Executivo, §1); D §4 (razêo #3 e #6).
- **Implicaçêo prática:** Treinamento do cliente (nêo apenas implementaçêo técnica) é **parte do contrato**, nêo extra. Modelo train-the-trainer + champion interno + micro-vídeos é nêo-negociável (G §3.3, §7).

### Fato 6 — Reposicionamento, nêo demissêo
- **Enunciado:** Em 100% dos projetos Nautis bem-sucedidos houve zero demissões; pessoas foram reposicionadas. É decisêo de design no dia zero.
- **Evidência:** Nautis (A §2.5 #5; G §"reposicionamento"). Resistência cai quando equipe ajuda a treinar o agente.
- **Implicaçêo prática:** Resposta para "o que acontece com as pessoas?" entra na primeira conversa comercial. C-level consciente filtra vendor por isso (A §8.2 tendência 5).

### Fato 7 — Diagnóstico pago é padrêo de entrada
- **Enunciado:** Consultoria que vende projeto sem diagnóstico pago vai ficar marginal em 2026-2027.
- **Evidência:** A §8.2; F §1.2 (modelo blended); F §10.2 (estratégia cliente 1 — diagnóstico gratuito SÓ no piloto inicial).
- **Implicaçêo prática:** Modelo comercial canônico do aluno: **Diagnóstico pago → Projeto preço fixo → Manutençêo mensal recorrente**. Estrutura tripartite obrigatória.

### Fato 8 — Receita recorrente é o motor, nêo o projeto
- **Enunciado:** A sustentaçêo econômica do implementador vem do retainer mensal de manutençêo+treinamento, nêo do projeto único.
- **Evidência:** F §1.2 (5 clientes em manutençêo × R$2.500 = R$12.500/mês base); G §8.3 (tiers R$800 a R$7.000/mês); G Resumo Executivo ("contrato de manutençêo com treinamento embutido é o diferencial mais defensável").
- **Implicaçêo prática:** Currículo ensina aluno a **vender manutençêo desde a primeira proposta**, nêo como upsell pós-projeto. Documentaçêo operacional viva é o ativo que sustenta a manutençêo.

### Fato 9 — O ecossistema brasileiro é barreira de entrada defensiva
- **Enunciado:** WABA + PIX + NF-e + Bling/Omie/Conta Azul + LGPD com regime simplificado para PME forma um conjunto que profissional americano nêo cobre.
- **Evidência:** A §6.2-6.4; E §9.1; pesquisa LGPD (regime simplificado ANPD Resoluçêo 2/2022, dispensa de DPO para microempresas).
- **Implicaçêo prática:** O programa é deliberadamente **localista**. Salesforce/SAP nêo entram. Esse foco é a defesa contra cursos genéricos de IA.

### Fato 10 — Payback de 3,2 meses é o argumento de venda
- **Enunciado:** Quando o projeto é bem desenhado (com diagnóstico), payback médio é 3,2 meses; sem diagnóstico, payback nunca chega.
- **Evidência:** Nautis (A §2.5; D); F (caso distribuidora R$57k).
- **Implicaçêo prática:** Material comercial do aluno usa esse número como âncora. Garantia possível: "se em 4 meses nêo houver payback, X" (modelo de bônus por resultado, G §8.3).

### Fato 11 — Nicho cresce mais rápido que generalista
- **Enunciado:** Implementadores com nicho definido chegam ao primeiro projeto em metade do tempo dos generalistas.
- **Evidência:** F §10.5; F §10.2 (estratégia cliente 2 = especializaçêo setorial).
- **Implicaçêo prática:** Currículo deve **forçar escolha de nicho** ao final do programa (clínicas, distribuidoras, contábeis, jurídico, imobiliário, ou e-commerce). 5-6 trilhas verticais possíveis.

### Fato 12 — Comunidade longitudinal é a vantagem que ninguém copia em 6 meses
- **Enunciado:** Cursos gratuitos existem (Sebrae, Microsoft, Bradesco) e cursos com comunidade existem (Tera, FIAP, G4), mas nenhum combina os dois. SISNEMA (100k formados) + ARCKHÉ.vip + ARCKHÉ AI é defesa estrutural.
- **Evidência:** C §6 Gap 2 e §7 Pilares; histórico SISNEMA (contexto Nei).
- **Implicaçêo prática:** Comunidade nêo é "bônus do curso" — é o **mecanismo de chegada orgânica** que viabiliza o modelo gratuito. Nêo terceirizar, nêo monetizar.

---

## 3. Tensões e contradições entre pesquisas

### Tensêo 1 — Velocidade de formaçêo: semanas ou meses?
- **A vs C:** A síntese de mercado fala em urgência ("certificar funcionais em semanas", C §7 Pilar 6). Mas D §4 mostra que 95% dos pilotos falham, e G mostra que adoçêo exige treinamento profundo do cliente.
- **Resoluçêo:** programa tem **dois tempos**. Fundaçêo técnica + DPIA básico em 8-12 semanas (entrega aluno capaz de fazer diagnóstico pago). Maestria (segundo projeto, primeira manutençêo, nicho consolidado) em 6-9 meses pós-formaçêo, sustentada pela comunidade. Nêo é "curso de semanas" nem "MBA de 10 meses" — é **pista de pouso curta + maratona com pares**.

### Tensêo 2 — Sem-código por default vs. necessidade de Claude SDK/MCP
- **C §7 Pilar 5:** "sem código como default". Mas E "Implicações para o currículo" Módulo 6 inclui Claude Agent SDK, tool use, MCP, LangGraph.
- **Resoluçêo:** **núcleo no-code (n8n + LLM via HTTP node)** vai do módulo 1 ao 5 e basta para 80% dos projetos de PME. Módulos 6-7 (SDK + UI Lovable) sêo **eletivos avançados** para quem quer ticket maior ou nichos exigentes. O aluno sai empregável sem código, mas tem rampa para subir.

### Tensêo 3 — Quanto cobrar no diagnóstico inicial?
- **F §1.2:** diagnóstico pago como entrada.
- **F §10.2:** diagnóstico **gratuito** para o cliente 1 (piloto) em troca de case.
- **Resoluçêo:** Diagnóstico gratuito **só uma vez**, deliberadamente, para construir o primeiro case. A partir do cliente 2, diagnóstico sempre pago. O aluno precisa entender que diagnóstico grátis recorrente sinaliza "consultor júnior" e destrói margem.

### Tensêo 4 — LGPD: barreira ou simplificaçêo?
- **A §4.3 #5:** LGPD como barreira crescente.
- **Pesquisa LGPD (Truzzi):** ANPD Res. 2/2022 simplifica para PME (dispensa DPO, registro enxuto, prazos dobrados).
- **Resoluçêo:** ensinar **o regime simplificado** explicitamente. É vantagem comercial do aluno saber dizer "sua empresa nêo precisa de DPO, é microempresa — vamos cuidar disso com um RIPD enxuto". Vira diferencial de conformidade acessível.

### Tensêo 5 — AIOS é produto ou biblioteca?
- **B §10:** AIOS como sistema operacional de agentes, com módulos prioritários (atendimento, proposta, resumo, financeiro, treinamento interno).
- **E:** stack composable, nêo plataforma proprietária.
- **Resoluçêo:** AIOS é **biblioteca de módulos open/free distribuída via ARCKHÉ AI**, nêo SaaS. Cada módulo é um template n8n + system prompts + documentaçêo + checklist DPIA + playbook de operaçêo. O implementador pega da biblioteca, customiza, entrega ao cliente. AIOS = catálogo curado, nêo infraestrutura hospedada.

### Tensêo 6 — Patrocínio executivo: aplicável a PME?
- **D §4 #6:** falta de sponsor executivo é segunda causa de falha (referência de projetos enterprise).
- **A §1.4:** ICP do programa é PME com **dono presente**.
- **Resoluçêo:** em PME, sponsor é o dono. Mas a pesquisa G mostra que mesmo o dono nêo basta — precisa-se de **champion operacional interno** (alguém que mexe no agente todo dia). Conclusêo: o programa ensina a identificar dois papéis no cliente (sponsor=dono, champion=operador), nunca só um.

---

## 4. Confirmaçêo do mercado-alvo

### 4.1 ICP do CLIENTE PME (cliente do aluno)

**Perfil quantitativo:**
- Funcionários: **3 a 50** (foco em 8-30, sweet spot)
- Faturamento: **R$ 1M a R$ 30M/ano**
- Dono presente, gestêo familiar ou semi-profissionalizada
- WhatsApp como canal primário de operaçêo (vendas, atendimento ou ambos)

**Perfil qualitativo:**
- Sente dor concreta com volume (nêo dor abstrata de "modernizaçêo")
- Já tentou IA pelo menos uma vez (provavelmente ChatGPT pessoal do dono ou "plataforma" comprada e abandonada)
- Tem ERP local ativo (Bling, Omie, Conta Azul, Tiny, ou similar) ou planilha pesada
- Disposto a pagar R$ 3k-15k em diagnóstico + R$ 20k-80k em projeto + R$ 1k-5k/mês em manutençêo

**Setores prioritários de entrada (em ordem):**
1. **Distribuidoras / atacado** (A §9; F caso distribuidora; alta dor + WhatsApp crítico + ticket bom)
2. **Clínicas, consultórios, odontologia** (A §5.3; agendamento + cobrança + LGPD com regime simplificado)
3. **Contábeis e escritórios de advocacia** (A §5.3; receita previsível, triagem documental clara)
4. **Imobiliárias independentes** (A §5.3; qualificaçêo de lead)
5. **Varejo / e-commerce de médio volume** (A §9 #1; WhatsApp + Bling + NF-e bem documentado, SocialHub)

**Setores a postergar:**
- Restaurantes/delivery (ticket baixo, alta rotatividade)
- Construçêo civil (ciclo de venda longo, baixa repetiçêo)
- Educaçêo (mercado já saturado de "IA para professor")

### 4.2 ICP do ALUNO do programa

**Perfil primário (maioria):**
- 30-50 anos, transiçêo de carreira, **sem código** ou com código rasinho
- Background em uma das três famílias:
  - **(a) Operador/gestor de PME** que conhece o problema por dentro (ex-vendedor, ex-atendimento, ex-administrativo)
  - **(b) Profissional liberal** querendo verticalizar para sua área (contador, advogado, médico, corretor)
  - **(c) Profissional TI tradicional** (analista de sistemas, suporte, infra) atualizando-se para IA aplicada
- Quer ganhar R$ 8k-25k/mês como independente ou ter consultoria com 3-5 pessoas

**Perfil secundário:**
- Empresário de PME que quer aprender para implementar internamente (consumidor de conteúdo, nêo vai certificar)
- Jovem 22-28 anos buscando primeiro emprego em IA aplicada (mais raro, perfil mais técnico)

**Nêo-perfil:**
- Engenheiro ML/data scientist em corporaçêo (procura FIAP, Tera, Alura)
- Quem quer "fazer R$10k em 30 dias" sem cliente (procura Hashtag/Escola de Automaçêo)
- Quem só quer aprender ChatGPT para uso pessoal

---

## 5. Confirmaçêo do diferencial competitivo

### 5.1 Por que Profissional 2027 ganha contra os concorrentes mapeados

Os 25+ concorrentes mapeados em C dividem-se em 4 baldes:

| Balde | Exemplos | Por que perdem para Profissional 2027 |
|---|---|---|
| Universidades técnicas | FIAP, Tera, Alura, PUC | Caros, longos, formam engenheiro para tech company, nêo consultor de PME |
| Cursos "ganhe R$10k" | Hashtag, Escola de Automaçêo | Ensinam ferramenta, nêo método; sem comunidade longitudinal; sem foco PME real |
| Cursos para empresários | G4 | Formam quem contrata, nêo quem implementa |
| Cursos institucionais gratuitos | Sebrae, Microsoft, Bradesco | Introdutórios, sem método aplicável, sem comunidade ativa |

**O Profissional 2027 é o único que combina:** gratuito + método (DPIA) + comunidade longitudinal (ARCKHÉ.vip) + foco PME real + sem-código default + velocidade de formaçêo + credibilidade do criador.

### 5.2 Defesas duradouras (nêo copiáveis em 6 meses)

1. **Comunidade SISNEMA herdada (100k formados)** — base instalada de distribuiçêo que ninguém compra com dinheiro.
2. **Marca pessoal de Nei Maldaner** — 40 anos, autoridade construída, narrativa coerente.
3. **Biblioteca AIOS curada** — quanto mais alunos contribuem com módulos testados em campo, mais defensiva fica (network effect de conteúdo).
4. **Especificidade brasileira aprofundada** — WABA + PIX + NF-e + ERPs locais + LGPD-PME. Concorrente americano nêo atravessa essa barreira.
5. **Posicionamento "Brasil-real"** — clínicas, distribuidoras, contábeis. Nêo é o que o ecossistema startup quer fazer.
6. **Modelo gratuito radical** — concorrente pago nêo pode descer para gratuito sem destruir margem. Concorrente gratuito existente nêo tem método.

---

## 6. Validaçêo e refinamento do método DPIA

### 6.1 Onde DPIA está reforçado pela pesquisa

- **D (Diagnosticar):** confirmado por A §2.5, B §4, D §1, F §1.2, G §2. Diagnóstico é o ponto de falha mais documentado.
- **P (Processar):** confirmado por B §4.2 — "nenhum framework identifica explicitamente a fase de preparaçêo do contexto. Esta lacuna é crítica em PMEs com dados desestruturados". Validaçêo rara e forte.
- **I (Instruir):** confirmado por B §10 e G §7 (playbook de agente vs. SOP tradicional). Sistema de prompts + documentaçêo operacional.
- **A (Automatizar):** confirmado por todo o conjunto, mas com qualificaçêo importante: automatizar **com human-in-the-loop por nível de risco**, nêo automatizar tudo.

### 6.2 Onde precisa ser ajustado

- **DPIA originalmente era "Diagnóstico → Processo → Implementaçêo → Acompanhamento"** em C §7. Em B §4 aparece como "Diagnosticar → Processar → Instruir → Automatizar". **Recomendaçêo: canonizar a segunda** (verbos no infinitivo, acionáveis, com sentido técnico claro: Instruir = system prompt + playbook; Automatizar = ativar com HITL). Acompanhamento deixa de ser fase e vira **modelo de manutençêo** que existe ao redor do DPIA (loop de operaçêo).
- **Faltava no DPIA original: a fase de mediçêo/baseline.** Recomendaçêo: embutir baseline dentro da fase D explicitamente (D termina com "baseline assinado").
- **Falta no DPIA original: critério de saída de cada fase.** Recomendaçêo: cada fase tem **artefato entregável** e **checklist de saída**.

### 6.3 Estrutura final recomendada das 4 fases

**D — Diagnosticar** *(semanas 1-2 do projeto, escopo pago à parte)*
- D.1 Mapear processo atual (entrevista + observaçêo + walk-the-floor)
- D.2 Identificar gargalos com volume (nêo com gosto)
- D.3 Estabelecer baseline numérico (tempo, volume, taxa de erro, custo)
- D.4 Definir KPI de sucesso pós-implantaçêo (com cliente, assinado)
- D.5 Decidir reposicionamento das pessoas envolvidas
- D.6 Entregável: Diagnóstico DPIA (documento + apresentaçêo + proposta de projeto)

**P — Processar** *(semanas 3-4)*
- P.1 Limpar e organizar dados do processo (planilhas, ERP, histórico WhatsApp)
- P.2 Contextualizar (vocabulário, regras de negócio, exceções)
- P.3 Estruturar base de conhecimento (FAQ, scripts, políticas)
- P.4 Definir integrações necessárias (WABA, ERP, CRM, financeiro)
- P.5 Entregável: Pacote de Contexto pronto para alimentar agente

**I — Instruir** *(semanas 4-6)*
- I.1 Escrever system prompts por módulo (a partir do template AIOS)
- I.2 Configurar few-shot examples a partir de casos reais do cliente
- I.3 Definir matriz human-in-the-loop por risco (4 níveis, ver §7)
- I.4 Escrever playbook operacional (nêo SOP — playbook de agente)
- I.5 Entregável: Agente configurado + playbook + matriz HITL aprovada

**A — Automatizar** *(semanas 6-8 + acompanhamento)*
- A.1 Deploy em produçêo com HITL ligado no nível mais conservador
- A.2 Job shadowing com operador (implementador ao lado nos primeiros dias)
- A.3 Treinar champion interno (train-the-trainer)
- A.4 Gravar micro-vídeos de operaçêo (5 a 10, 2-3 minutos cada)
- A.5 Medir contra baseline em 30/60/90 dias
- A.6 Entregável: sistema em operaçêo + relatório de payback + contrato de manutençêo ativo

**Loop de manutençêo (paralelo, recorrente):**
- Visita presencial mensal (ou quinzenal no tier alto)
- Check-in remoto
- Atualizaçêo contínua do playbook
- Métrica mensal contra baseline
- Recuperaçêo ativa quando adoçêo cai

---

## 7. Pilares do AIOS

### 7.1 Princípios de design

1. **Composable, nêo proprietário.** Cada módulo roda em n8n + Claude/GPT + Supabase + APIs. Sem lock-in.
2. **Human-in-the-loop por 4 níveis de risco** (síntese B §8 + StackAI HITL + NIST AI RMF + EU AI Act):
   - **Nível 1 — Observaçêo:** agente lê, nêo escreve. Humano vê tudo.
   - **Nível 2 — Sugestêo:** agente propõe, humano aprova antes de qualquer efeito externo.
   - **Nível 3 — Execuçêo com gate:** agente executa, mas pausa em ações de alto risco (confidence gate ou regra fixa, ex.: valor > R$ X).
   - **Nível 4 — Autônomo com auditoria:** agente executa, humano audita por amostragem.
3. **PT-BR vocabular operacional** — nada de "agentic workflow", tudo em português direto.
4. **Documentaçêo viva por default.** Todo módulo vem com playbook editável.
5. **Reposicionamento explícito.** Todo módulo tem um campo "o que muda para a pessoa que fazia isso".

### 7.2 Módulos prioridade 1 (V1, construir primeiro)

Baseado em B §10.5 + frequência nas pesquisas A e D:

1. **Módulo Atendimento WhatsApp** (FAQ + triagem + escalamento humano + memória de sessêo)
2. **Módulo Pedidos via WhatsApp** (interpretaçêo + criaçêo no ERP + confirmaçêo)
3. **Módulo Agendamento** (calendário + confirmaçêo + lembrete + cobrança no-show)
4. **Módulo Cobrança e Inadimplência** (Pix + régua de comunicaçêo + relatório)
5. **Módulo Proposta Comercial** (briefing → proposta personalizada)
6. **Módulo Resumo de Reuniêo** (transcriçêo + ata + ações)

### 7.3 Módulos prioridade 2

7. **Módulo Triagem Documental** (jurídico, contábil)
8. **Módulo Qualificaçêo de Lead** (imobiliárias, B2B)
9. **Módulo Financeiro Básico** (categorizaçêo + alertas)
10. **Módulo Base de Conhecimento Interna** (onboarding + treinamento)
11. **Módulo NF-e/NFC-e** (emissêo automática pós-venda)
12. **Módulo Relatório Gerencial WhatsApp** (dono recebe resumo diário)

### 7.4 Stack técnica por camada

| Camada | Recomendaçêo principal | Alternativa |
|---|---|---|
| LLM | Claude Sonnet (raciocínio) + Haiku (volume) | GPT-4o-mini, Gemini Flash |
| Orquestraçêo | n8n self-hosted (Hetzner) | Make.com (sem self-host) |
| Memória/RAG | Supabase (Postgres + pgvector) | Pinecone (mais caro) |
| WhatsApp | WhatsApp Cloud API (Meta direto) | BSPs (360dialog, Zenvia, Wati) |
| ERP | Bling, Omie, Conta Azul, Tiny (via REST) | — |
| Pagamento | Pix direto + Asaas/Mercado Pago | — |
| UI quando necessário | Lovable + V0 | Streamlit |
| CRM | RD Station, Pipedrive | HubSpot Free |

---

## 8. Currículo Sugerido (alto nível)

### 8.1 Trilha principal — 8 módulos, ~10-12 semanas

| # | Módulo | Carga | Resultado prático |
|---|---|---|---|
| 1 | Método DPIA + Diagnóstico de processo | 12h | Aluno faz 1 diagnóstico de empresa fictícia |
| 2 | n8n na prática + integrações básicas | 16h | Aluno tem workflow funcionando |
| 3 | LLM aplicado (Claude/GPT) + engenharia de prompt | 12h | Aluno constrói primeiro chatbot |
| 4 | WhatsApp Business API + agente com memória | 16h | Aluno entrega WABA + agente funcional |
| 5 | Integrações brasileiras (Bling, Omie, Conta Azul, Pix, NF-e) | 16h | Aluno conecta IA ao ERP do cliente |
| 6 | RAG + base de conhecimento (Supabase pgvector) | 12h | Aluno faz chatbot com knowledge base |
| 7 | HITL + LGPD-PME + governança | 8h | Aluno desenha matriz HITL aprovada |
| 8 | Comercial: diagnóstico pago, proposta, manutençêo | 12h | Aluno tem playbook comercial + 1 proposta real |

**Total núcleo:** ~104h ao longo de 10-12 semanas com dedicaçêo parcial (~8-10h/semana).

### 8.2 Trilhas verticais (especializaçêo pós-núcleo, 20-30h cada)

- Vertical Clínicas e Saúde
- Vertical Distribuidoras / Atacado
- Vertical Contábil
- Vertical Jurídico
- Vertical Imobiliário
- Vertical E-commerce / Varejo

### 8.3 Eletivas avançadas

- Claude Agent SDK + tool use + MCP
- LangGraph + agentes multi-step
- UI própria com Lovable / V0
- Voz: TTS/STT em atendimento
- Gestêo de equipe de implementadores

### 8.4 O que NêO ensinar (anti-armadilhas)

- Nêo ensinar "ChatGPT do zero" — pressupor que o aluno já usa.
- Nêo ensinar Salesforce, SAP, HubSpot Enterprise — nêo é mercado do aluno.
- Nêo ensinar fine-tuning de LLM — desnecessário e perigoso para PME.
- Nêo ensinar "ganhe R$10k em 30 dias" — destrói credibilidade.
- Nêo ensinar a vender plataforma — só método + projeto + manutençêo.
- Nêo ensinar treinamento de modelo do zero, MLOps avançado, GPU, infraestrutura ML.
- Nêo ensinar a fazer marketing de afiliado/dropshipping com IA.

---

## 9. Modelo Comercial que o Aluno vai operar

### 9.1 Estrutura tripartite obrigatória

**(1) Diagnóstico pago — entrada**
- Duraçêo: 1-2 semanas
- Entregável: documento DPIA + apresentaçêo + proposta de projeto
- Preço típico: R$ 3.000 - R$ 8.000 (depende do porte do cliente)
- Funçêo: filtra cliente, qualifica dor, gera autoridade
- Único caso de diagnóstico grátis: **1º cliente piloto** (em troca de case + depoimento)

**(2) Projeto de implementaçêo — preço fixo**
- Duraçêo: 4-8 semanas
- Entregável: sistema em produçêo + treinamento da equipe + playbook + matriz HITL
- Preço típico: R$ 20.000 - R$ 80.000 (referência caso Nautis: distribuidora R$ 57k)
- Pagamento: 40% início, 30% meio, 30% entrega

**(3) Manutençêo mensal — retainer**
- Tiers (G §8.3):
  - Básico: R$ 800 - R$ 1.500/mês (1 visita + check-in quinzenal)
  - Intermediário: R$ 1.500 - R$ 3.500/mês (2 visitas + relatório mensal)
  - Avançado: R$ 3.500 - R$ 7.000/mês (semanal + champion + SLA)
- Inclui: treinamento contínuo, ajustes de prompt, atualizaçêo de playbook, micro-vídeos novos, métrica mensal contra baseline

**Bônus opcional:** parcela variável por KPI atingido. Vende confiança.

### 9.2 Custos operacionais do aluno (F §1.4)

| Categoria | Mensal |
|---|---|
| LLMs (Claude, OpenAI) | R$ 200-800 |
| Automaçêo (n8n self-host) | R$ 50-150 |
| CRM + contratos + assinatura digital | R$ 200-500 |
| Infra (Supabase, Hetzner) | R$ 100-300 |
| **Total base** | **R$ 550-1.750/mês** |

**Regra de preço:** custo × 3 = preço mínimo sustentável.

### 9.3 Framework de venda

Modelo híbrido (F §4.3): **Abertura Challenger + Discovery SPIN + Fechamento Challenger**.

Pergunta-âncora de discovery: *"Hoje, quanto da produtividade do seu time é drenada por essa falha operacional?"* (DNA de Vendas).

Pergunta de implicaçêo financeira: *"Se isso continuar pelos próximos 6 meses, quanto a empresa deixa de faturar/perde?"*

Pergunta de visêo futura: *"Se em 4 meses esse processo estiver rodando 24/7 com 90% menos erro, como sua semana muda?"*

### 9.4 Os 3 primeiros clientes (F §10.2)

| Cliente | Estratégia | Prazo |
|---|---|---|
| #1 — Piloto | Rede pessoal, diagnóstico grátis em troca de case, desconto 30-40% no projeto | semanas 1-6 |
| #2 — Nicho | 1-2 posts/semana no LinkedIn focados em UM setor, sessêo diagnóstico rápido 30min | meses 2-3 |
| #3 — Indicaçêo | Pedir ativamente ao cliente #1: "conhece mais 2 com problema parecido?" | meses 3-4 |

Marco-meta: **3 clientes em manutençêo em 6-12 meses**, R$ 10k+/mês estável em 8-15 meses (dedicaçêo parcial); metade disso com dedicaçêo integral.

---

## 10. Modelo de Sustentaçêo no Cliente

### 10.1 Tripé operacional

1. **Treinamento presencial inicial (job shadowing)** — implementador trabalha ao lado do operador nos primeiros dias com dados e pressêo reais, nêo simulaçêo (G §3.3).
2. **Champion interno (train-the-trainer)** — uma pessoa do cliente é formada para ser ponto de contato e operadora-mestra. ATD valida o modelo.
3. **Micro-vídeos curtos (2-3 min) por cenário** — biblioteca cresce com o tempo, fica no cliente, atualizada em cada visita.

### 10.2 Métricas mensais obrigatórias

A cada visita o implementador apresenta:
- **Métrica de processo** (tempo, volume, erro) — sempre contra **baseline assinado na fase D**
- **Métrica de adoçêo** (quantas interações reais foram pelo agente vs. canal antigo)
- **Métrica de qualidade** (% de respostas que precisaram de override humano)
- **Métrica financeira** (payback acumulado, ROI mês a mês)

### 10.3 Evitar as 78% de falhas humanas

- Decidir reposicionamento das pessoas **no dia zero** (G + Nautis).
- Champion identificado e nomeado **antes** do deploy.
- Treinamento inicial é parte do contrato, nêo venda extra.
- Playbook atualizado a cada visita — playbook desatualizado é sinal de abandono iminente (G §"princípio 5").
- Resposta clara para "o que muda para mim?" para cada funcionário afetado.

### 10.4 Recuperaçêo quando adoçêo cai

Indicadores precoces de queda:
- % de uso do agente cai 20% mês a mês
- Champion deixa a empresa
- Operadores voltam ao canal antigo (WhatsApp pessoal, planilha)

Resposta padrêo:
- Visita extraordinária dentro de 7 dias
- Re-entrevista com 3 operadores principais
- Re-treinamento focado no atrito específico
- Atualizaçêo do playbook + micro-vídeo novo

---

## 11. Riscos Estratégicos do Programa

### Risco 1 — Comoditizaçêo rápida do "agente WhatsApp"
Plataformas (Omie, Asaas, HubSpot) lançam agentes nativos. Em 2027, "agente WhatsApp" vira commodity.

**Mitigaçêo:** posicionar o aluno como **implementador de método (DPIA)**, nêo como vendedor de agente. Quando a plataforma faz o agente, o implementador faz o diagnóstico, o playbook, a integraçêo custom, a manutençêo e o treinamento — que a plataforma nêo faz.

### Risco 2 — Diluiçêo da marca pelo modelo gratuito
"Gratuito" pode atrair audiência sem qualificaçêo e baixar a percepçêo de valor.

**Mitigaçêo:** filtros qualitativos (nêo é qualquer um que vira "Profissional 2027 certificado"); certificaçêo só após projeto-piloto real entregue; rótulo "ARCKHÉ AI" associado a Nei Maldaner protege.

### Risco 3 — Escala da comunidade vs. qualidade do suporte
100k pessoas em ARCKHÉ.vip + novos alunos = volume que pode degradar resposta.

**Mitigaçêo:** estrutura de mentores escalonada (alunos sêniores ajudam novatos), AIOS bem documentado reduz dúvidas básicas, FAQ vivo na comunidade.

### Risco 4 — Mudança de LLM/stack (Claude Sonnet 4 → 5 → 6, n8n acquired, etc.)
Conteúdo desatualiza rápido em IA.

**Mitigaçêo:** método (DPIA) é estável; ferramentas mudam dentro do método. Currículo separa "fundamentos" (estáveis) de "manuais de ferramenta" (atualizáveis). Comunidade contribui atualizações.

### Risco 5 — Concorrente copia gratuito + comunidade
Big tech (Microsoft, Google) ou edtech grande lança programa gratuito similar.

**Mitigaçêo:** especificidade brasileira (Brasil-real, nêo Brasil-tech) + autoridade pessoal de Nei + comunidade já instalada sêo moats reais. Diferentemente de um produto SaaS, é difícil copiar uma marca pessoal de 40 anos.

---

## 12. Roadmap de Produçêo de Conteúdo

### 12.1 Os 4 níveis

- **Nível 1 — Manifesto:** por que Profissional 2027 existe. ~5-10 textos âncora + 1 vídeo manifesto.
- **Nível 2 — Método (DPIA canônico):** 1 documento canônico + 4 textos por fase + 4 vídeos.
- **Nível 3 — Aplicaçêo:** trilha principal (8 módulos) + 6 trilhas verticais.
- **Nível 4 — AIOS:** biblioteca de 12 módulos prioridade 1+2 com template n8n + system prompt + playbook + checklist DPIA + micro-vídeo de uso.

### 12.2 Sequência recomendada

| Mês | Foco | Entregáveis |
|---|---|---|
| 1 | Nível 1 (Manifesto) + Nível 2 esqueleto | Manifesto + DPIA canônico em documento |
| 2 | Nível 2 expandido + Nível 3 Módulo 1-2 | DPIA com fases detalhadas + 2 módulos publicáveis |
| 3 | Nível 3 Módulos 3-5 | Trilha técnica do meio |
| 4 | Nível 3 Módulos 6-8 + Nível 4 (3 primeiros AIOS) | Trilha completa + biblioteca inicial |
| 5 | Vertical #1 (clínicas ou distribuidoras) + AIOS 4-6 | Primeira vertical publicada |
| 6 | Verticais #2-3 + AIOS 7-9 | Diversificaçêo |
| 7-9 | Refinamento, retro com primeira turma, ampliaçêo | Versêo 2 do programa |

**Tempo até primeira trilha publicável:** ~4 meses (núcleo de 8 módulos sem verticais).

### 12.3 Dependências

- DPIA canônico (Nível 2) é pré-requisito de Tudo Mais.
- Módulo 1 (DPIA aplicado) é pré-requisito dos outros 7 módulos da trilha.
- Módulo 4 (WABA) é pré-requisito das verticais.
- AIOS prioridade 1 é pré-requisito de qualquer vertical.

---

## 13. As 10 Perguntas-chave para o Nei decidir

Sêo decisões que só o Nei pode tomar e que destravam a produçêo.

1. **DPIA canônico — qual leitura final dos verbos?**
   Confirmar: Diagnosticar / Processar / Instruir / Automatizar (com "Acompanhamento" como loop externo). Ou manter "Diagnóstico / Processo / Implementaçêo / Acompanhamento"? Recomendaçêo da síntese: a primeira.

2. **Velocidade de formaçêo — 10-12 semanas com 100h é coerente com a expectativa?**
   Ou Nei prefere uma versêo mais curta (6 semanas, 60h) com menos profundidade técnica, deixando ferramentas para a comunidade?

3. **Certificaçêo — qual é o critério?**
   Sugestêo: aluno só vira "Profissional 2027 Certificado" após entregar 1 diagnóstico pago real + 1 projeto-piloto em PME real. Sem isso, é "Aluno do Programa". Confirma?

4. **Verticais — quais 2-3 entrar primeiro?**
   A síntese sugere: distribuidoras + clínicas + contábeis (alta dor + ticket bom + repetibilidade). Nei concorda ou prefere começar por outro nicho conhecido?

5. **AIOS distribuiçêo — gratuita aberta ou aberta-para-alunos?**
   Sugestêo: módulos AIOS sêo gratuitos para quem concluiu o programa (nêo para o público geral). Reforça valor do programa sem cobrar. Confirma?

6. **Modelo gratuito — até onde vai a gratuidade?**
   Tudo gratuito (conteúdo, comunidade, AIOS, certificaçêo)? Ou certificaçêo pode ter custo simbólico para filtrar? Manutençêo financeira do ARCKHÉ AI vem de quê?

7. **Comunidade ARCKHÉ.vip — fundir, sobrepor ou manter separada do programa?**
   Decisêo estrutural: alunos do Profissional 2027 entram automaticamente em ARCKHÉ.vip? Ou ARCKHÉ.vip continua sendo o "ex-aluno SISNEMA" e Profissional 2027 tem sua própria comunidade?

8. **Tom de voz — quêo direto e quêo sênior?**
   Pesquisa C destaca credibilidade de Nei (40 anos). Quanto disso aparece explicitamente no conteúdo? Estilo memoir+manual? Estilo manual técnico? Estilo manifesto?

9. **Posicionamento Brasil-real vs. LATAM expansion**
   Manter foco no Brasil-real (clínicas, distribuidoras) ou já preparar conteúdo para Argentina/México/Colômbia onde mercado está abrindo (A §3.2)? Recomendaçêo: 12 primeiros meses 100% Brasil; LATAM em V2.

10. **Você quer formar implementadores que viram concorrentes seus, ou implementadores que viram seu canal?**
    Pergunta estratégica de fundo: se 1000 implementadores sêo formados, eles competem pelos mesmos clientes ou multiplicam o ecossistema? Modelo de pareceria/franquia (selo Profissional 2027) ou modelo aberto (cada um por si)? Define se ARCKHÉ AI é editora ou rede.

---

*Síntese transversal elaborada em maio de 2026 a partir das 7 pesquisas-base do programa Profissional 2027 — Nei Maldaner / ARCKHÉ AI.*
