# Diário da Dissertação

**Tema:** Sistema Inteligente de Observabilidade e Diagnóstico de Incidentes em Plataformas Cloud-IoT

- **Orientador:** Prof. Doutor Hélder Zagalo
- **Coorientador:** Fernão Abreu
- **Projeto:** CUK4ALL - New Technologies for Autonomous Kitchens
- **Empresa:** Wish And Cook
- **Bolsa:** Bolsa de Investigação (BI) - DETI, Universidade de Aveiro

---

## Semana 1 - 21 a 27 de setembro de 2026

### Tarefas realizadas
- [x] Ler a proposta da tese e o plano de trabalhos da bolsa (projeto CUK4ALL), percebendo a ligação entre ambos: a plataforma Wish And Cook é o caso de estudo da dissertação
- [x] Levantar as tecnologias envolvidas (Docker, Prometheus/Grafana, OpenTelemetry, ELK, Python, deteção de anomalias)
- [x] Identificar os 3 pilares da observabilidade: logs, métricas e traces

### Tarefas a realizar
- [ ] Reunião com orientador e coorientador na Wish&Cook
- [ ] Conhecer a plataforma Cloud-IoT existente
- [ ] Iniciar leitura de papers

### Notas
- Tarefa 1 (meses 1-2): estado da arte
- Tarefa 2 (meses 2-3): requisitos + arquitetura
- Tarefa 3 (meses 3-6): desenvolvimento + testes preliminares

---

## Semana 2 - 28 de setembro a 4 de outubro de 2026

### Tarefas realizadas
- [x] Reunião (segunda-feira) no escritório da Wish&Cook com o orientador e o coorientador
- [x] Perceber o funcionamento da plataforma existente
- [x] Conhecer o espaço novo de construção das cozinhas autónomas
- [x] Ler paper: *Adaptive Anomaly Detection for IoT Data in Hierarchical Edge Computing* - apontamentos e análise
- [x] Ler paper: *Anomaly Detection and Failure Root Cause Analysis in (Micro) Service-Based Cloud Applications* - apontamentos e análise

### Tarefas a realizar
- [ ] Ler paper: *Integrating Large Language Models with Cloud-Native Observability for Automated Root Cause Analysis and Remediation* - apontamentos e análise
- [ ] Ler paper: *Observability in Fog Computing* - apontamentos e análise
- [ ] Fazer e preparar a apresentação para a Sprint 1

### Notas
- Existem vários métodos de root cause analysis e de deteção de anomalias
- Ver mais tarde qual se aplica melhor ao caso da Wish&Cook

---

## Semana 3 - 5 a 11 de outubro de 2026

### Tarefas realizadas
- [ ] Ler paper: *Integrating Large Language Models with Cloud-Native Observability for Automated Root Cause Analysis and Remediation* - apontamentos e análise
- [ ] Ler paper: *Observability in Fog Computing* - apontamentos e análise
- [ ] Fazer e preparar a apresentação para a Sprint 1

### Tarefas a realizar
- Preparar para apresentação da Sprint 1
- Ver que logs, métricas e monitorização já existem na plataforma Wish and Cook
- Ler paper: *Anomaly Detection for IoT Time-Series Data: A Survey* - apontamentos e análise



### Notas
No primeiro paper, usam o LLM para diagnosticar a causa raiz e propor a remediação, mas não explicam como separaram os dados de treino dos de teste nem como mediram os resultados, por isso os ganhos reportados não são verificáveis.

---

## Semana 4 - 12 a 18 de outubro de 2026

### Tarefas realizadas
- [x] Preparar a apresentação da Sprint 1
- [x] Ver que logs, métricas e monitorização já existem na plataforma Wish and Cook
- [x] Ler paper: *Anomaly Detection for IoT Time-Series Data: A Survey* - apontamentos e análise

### Tarefas a realizar
- [ ] Ler paper: *A Survey of AIOps Methods for Failure Management* (Notaro, Cardoso, Gerndt) - apontamentos e análise
- [ ] Ler paper: *Automatic Root Cause Analysis via Large Language Models for Cloud Incidents* (Chen et al.) - apontamentos e análise
- [ ] Ler paper: *Anomaly Detection and Root-Cause Identification in Microservices: A Survey* (Barata et al.) - apontamentos e análise




### Notas
Com base apenas na análise do código e da configuração (a stack ainda não foi executada): a monitorização cobre parte da infraestrutura, mas a configuração da aplicação tem erros, os alertas não estão ativos e não há traces. No repositório, as métricas não identificam os robôs e o broker MQTT não é monitorizado.

---

## Semana 5 - 19 a 25 de outubro de 2026

### Tarefas realizadas
- [x] Ler paper: *A Survey of AIOps Methods for Failure Management* (Notaro, Cardoso, Gerndt) - apontamentos e análise
- [x] Ler paper: *Automatic Root Cause Analysis via Large Language Models for Cloud Incidents* (Chen et al.) - apontamentos e análise
- [x] Ler paper: *Anomaly Detection and Root-Cause Identification in Microservices: A Survey* (Barata et al.) - apontamentos e análise

### Tarefas a realizar
- [ ] Ler paper: *Evaluation of IoT Self-healing Mechanisms using Fault-Injection in Message Brokers* (Duarte et al.) - apontamentos e análise
- [ ] Ler paper: *ART: A Unified Unsupervised Framework for Incident Management in Microservice Systems* (Sun et al.) - apontamentos e análise
- [ ] Ler paper: *Flow-of-Action: SOP Enhanced LLM-Based Multi-Agent System for Root Cause Analysis* (Pei et al.) - apontamentos e análise
- [ ] Ler paper: *Solving The IoT Cascading Failure Dilemma using A Cooperative Multi-agent System* (Guittoum et al.) - apontamentos e análise
- [ ] Ler paper: *RCAEval: A Benchmark for Root Cause Analysis of Microservice Systems with Telemetry Data* (Pham et al.) - apontamentos e análise
- [ ] Fazer o PPT da Sprint 2 de PDE

### Notas
- **Notaro et al.:** organiza a gestão de falhas em AIOps. O sistema da tese é reativo (deteção, causa raiz e remediação), e a remediação é a parte menos estudada.
- **Chen et al. (RCACopilot):** usa um LLM para classificar a causa raiz de incidentes cloud a partir de evidência recolhida automaticamente. Depende de um histórico de incidentes rotulados, que a Wish&Cook não tem.
- **Barata et al.:** a abordagem mais comum é deteção não supervisionada com causa raiz baseada em grafos. Os resultados dos artigos não são comparáveis entre si e não há trabalhos em IoT.

---

## Semana 6 - 26 de outubro a 1 de novembro de 2026

### Tarefas realizadas
- [x] Ler paper: *Evaluation of IoT Self-healing Mechanisms using Fault-Injection in Message Brokers* (Duarte et al.) - apontamentos e análise
- [x] Ler paper: *ART: A Unified Unsupervised Framework for Incident Management in Microservice Systems* (Sun et al.) - apontamentos e análise
- [x] Ler paper: *Flow-of-Action: SOP Enhanced LLM-Based Multi-Agent System for Root Cause Analysis* (Pei et al.) - apontamentos e análise
- [x] Ler paper: *Solving The IoT Cascading Failure Dilemma using A Cooperative Multi-agent System* (Guittoum et al.) - apontamentos e análise
- [x] Ler paper: *RCAEval: A Benchmark for Root Cause Analysis of Microservice Systems with Telemetry Data* (Pham et al.) - apontamentos e análise
- [x] Fazer o PPT da Sprint 2 de PDE

### Tarefas a realizar
- [ ] Fazer a apresentação para a Sprint 2 de PDE
- [ ] Ler paper: *OpsCortex: Operational Memory for Self-Diagnosing Microservice Systems* (Seedat) - apontamentos e análise
- [ ] Ler paper: *MicroRCA-Agent: Microservice Root Cause Analysis Method Based on Large Language Model Agents* (Tang et al.) - apontamentos e análise
- [ ] Ler paper: *ST-GraphRCA: A Root Cause Analysis Model for Spatio-Temporal Graph Propagation in IoT Edge Computing* (Su et al.) - apontamentos e análise

