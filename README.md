# Samuel de Araújo

**Software Engineering · Distributed Systems · Scientific Computing**

Estudante de **Ciência da Computação** e desenvolvedor de software focado em construir sistemas com arquitetura explícita, rastreabilidade, testes e limites operacionais claros.

Meu portfólio combina **backend e produtos empresariais**, **sistemas distribuídos/event-driven**, **Android**, **engenharia de dados**, **computação científica** e **linguagens/compiladores**.

📍 Salvador, Bahia  
🎓 Ciência da Computação - Estácio  
💼 Suporte técnico, investigação de falhas e desenvolvimento de software

---

## O que eu construo

### Sistemas e produtos

- **Lumenza CRM** *(privado)* - CRM B2B multi-tenant com **Java 25, Spring Boot 4, Angular 22 e PostgreSQL 17**; autorização por tenant, concorrência otimista, analytics derivados do banco, webhooks com transactional outbox, auditoria e E2E em navegador real.
- **SignaForge** *(privado)* - plataforma de incident response e alert orchestration com **C# / .NET 10, ASP.NET Core, Next.js, PostgreSQL, Valkey e RabbitMQ**; ingestão assíncrona, deduplicação, idempotência, DLQ, SignalR e políticas de escalonamento.
- **Show** *(privado)* - plataforma de digital signage com **React/TypeScript, Supabase e Android Kotlin/Jetpack Compose/Media3**; player offline-first, revisions imutáveis, SHA-256, last-known-good, reprodução contínua e gateway de streaming.
- **Inteligência de Licitações - Bahia** *(privado)* - apoio à decisão com coleta, evidência, riscos, tarefas, estimativas e fronteiras explícitas de autoridade humana.
- **Radar de Importação Brasil** *(privado)* - descoberta multi-fonte, snapshots, sourcing, compliance, logística, recálculo seletivo e decisão econômica conservadora diante de dados incompletos.

### Ciência, dados e visualização

- **[Human Space Atlas](https://github.com/SamDevlab/human-space-atlas)** - atlas 3D com **CesiumJS**, catálogo orbital, propagação **SGP4**, Web Workers e dados de CelesTrak, NASA, NOAA e JPL.
- **[Molecule Generation & Virtual Screening Suite](https://github.com/SamDevlab/molecule-generation-suite)** - química computacional e ML com **RDKit, XGBoost, fingerprints moleculares e AutoDock Vina**.
- **[Transparência Municipal](https://github.com/SamDevlab/transparencia)** - framework reproduzível de dados públicos com proveniência, snapshots, evidência bruta, normalização e comparação conservadora.
- **[Fraud Detection with XGBoost](https://github.com/SamDevlab/fraud-detection-xgboost)** - estudo de detecção de fraude com avaliação orientada a Precision-Recall e tratamento correto de desbalanceamento.

### Linguagens e sistemas

- **S3** *(privado)* - linguagem experimental de sistemas baseada em ternário balanceado, com frontend de compilador, análise semântica, IR tipada, SSA/CFG, verifier, otimizações, assembly própria, emulador e backend Linux x86-64.
- **[S3-Benchmarks](https://github.com/SamDevlab/S3-Benchmarks)** - harness público de correção e benchmarking do ecossistema S3, com equivalência observável antes da comparação de desempenho.

---

## Stack atual

| Área | Tecnologias |
|---|---|
| **Backend** | Java 25, Spring Boot, C# / .NET 10, ASP.NET Core, Python, Node.js |
| **Frontend** | Angular 22, React, Next.js, TypeScript, Vite |
| **Mobile** | Kotlin, Android, Jetpack Compose, Media3 |
| **Dados** | PostgreSQL, SQLite, Supabase, Pandas, NumPy |
| **Mensageria / distribuídos** | RabbitMQ, transactional outbox/inbox, Valkey/Redis, workers concorrentes, idempotência |
| **ML / científico** | XGBoost, Scikit-learn, RDKit, AutoDock Vina, SGP4, CesiumJS |
| **Qualidade** | GitHub Actions, Testcontainers, Playwright, Vitest, pytest, E2E, testes de integração e differential testing |
| **Infra / operação** | Docker, Docker Compose, Linux, observabilidade, Prometheus/OpenAPI onde aplicável |

---

## Como eu projeto software

Tenho preferência por sistemas em que seja possível tornar explícitos:

- **fonte de verdade** e proveniência dos dados;
- **invariantes**, limites de autoridade e estados válidos;
- **isolamento entre tenants** e fronteiras de segurança;
- **idempotência**, concorrência e recuperação de falhas;
- **contratos versionados** entre componentes;
- **testes reproduzíveis** e CI como parte da arquitetura;
- diferença entre **fato, inferência e estimativa**;
- documentação suficiente para outra pessoa conseguir executar e auditar o sistema.

---

## Engenharia na prática

Exemplos de padrões usados nos projetos atuais:

```text
PostgreSQL como fonte autoritativa
        ↓
transações / invariantes / versionamento
        ↓
outbox + filas + workers idempotentes
        ↓
APIs e clientes web/mobile
        ↓
CI → integração → E2E → evidência reproduzível
```

Nem todo projeto usa todos esses componentes; a arquitetura é escolhida de acordo com o problema, e não para maximizar a quantidade de tecnologias.

---

## Contato

**E-mail:** [samusilvadev@gmail.com](mailto:samusilvadev@gmail.com)
