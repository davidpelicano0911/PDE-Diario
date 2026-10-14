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
- Preparar para  apresentação da Sprint 1
- Ver que logs, métricas e monitorização já existem na plataforma Wish and Cook
- Ler paper: *Anomaly Detection for IoT Time-Series Data: A Survey* - apontamentos e análise



### Notas
No primeiro paper, usam o LLM para diagnosticar a causa raiz e propor a remediação, mas não explicam como separaram os dados de treino dos de teste nem como mediram os resultados, por isso os ganhos reportados não são verificáveis.