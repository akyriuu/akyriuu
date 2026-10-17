<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=230&color=0:09090B,50:172554,100:0891B2&text=Marcus%20Vin%C3%ADcius&fontSize=48&fontColor=E2F3FF&fontAlignY=38&desc=BACKEND%20ENGINEER%20%E2%80%A2%20PAYMENTS%20%E2%80%A2%20AWS&descAlignY=58&descSize=15&animation=fadeIn" width="100%" alt="Marcus Vinícius — Backend Engineer"/>

<a href="https://readme-typing-svg.demolab.com/">
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=16&duration=2800&pause=900&color=22D3EE&center=true&vCenter=true&width=750&lines=Building+reliable+payment+systems;Idempotency+%7C+Transactional+Outbox+%7C+Retries;Node.js+%7C+NestJS+%7C+TypeScript+%7C+AWS;Distributed+systems+where+correctness+matters" alt="Animated introduction"/>
</a>

<br/>

<a href="https://github.com/akyriuu">
<img src="https://img.shields.io/badge/GitHub-akyriuu-111827?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/>
</a>
<a href="https://www.linkedin.com/in/marcusvin%C3%ADcius-/">
<img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
</a>
<a href="mailto:akyriu@hotmail.com">
<img src="https://img.shields.io/badge/Email-Let's_talk-0891B2?style=for-the-badge&logo=microsoftoutlook&logoColor=white" alt="Email"/>
</a>

Brazil 🇧🇷 · Open to Backend Engineering Opportunities

</div>

# Who am I?

I build backend systems where correctness matters as much as performance.

My main focus is payment infrastructure, asynchronous processing, distributed systems, and cloud-native applications. I work with Node.js, TypeScript, NestJS, PostgreSQL, and AWS, designing systems that remain predictable under retries, concurrent requests, and partial infrastructure failures.

I care about the engineering decisions behind reliable software: database-enforced idempotency, explicit transaction boundaries, resilient message processing, and observability that makes failures actionable.

const marcus = {
  role: "Backend Engineer",
  location: "Brazil 🇧🇷",
  focus: [
    "Payment Systems",
    "Distributed Systems",
    "Event-Driven Architecture",
    "AWS Serverless",
  ],
  stack: ["Node.js", "TypeScript", "NestJS", "PostgreSQL"],
  principles: [
    "Correctness over assumptions",
    "Idempotency over duplicate charges",
    "Observability over guesswork",
  ],
};

I don't just build APIs that work. I design systems that behave correctly when things go wrong.
~/engineering-impact

<div align="center">

<table>
<tr>
<td align="center" width="33%">
<h2>15+</h2>
REST API endpoints<br/>delivered
</td>
<td align="center" width="33%">
<h2>80%</h2>
Less batch message<br/>reprocessing
</td>
<td align="center" width="33%">
<h2>100%</h2>
Unauthenticated webhooks<br/>rejected
</td>
</tr>
<tr>
<td align="center" width="33%">
<h2>5</h2>
AWS resources provisioned<br/>as infrastructure as code
</td>
<td align="center" width="33%">
<h2>60s</h2>
Dead-letter queue<br/>failure detection target
</td>
<td align="center" width="33%">
<h2>2</h2>
Payment providers<br/>integrated
</td>
</tr>
</table>

</div>

Metrics refer to projects and implementations described in my portfolio.

# My projects

01. Asynchronous Payment Pipeline

<a href="https://github.com/akyriuu"> <img src="https://img.shields.io/badge/AWS-Serverless-FF9900?style=flat-square&logo=amazonaws&logoColor=white"/> </a> <img src="https://img.shields.io/badge/Architecture-Event--Driven-0891B2?style=flat-square"/> <img src="https://img.shields.io/badge/Focus-Reliability-6366F1?style=flat-square"/>

Designed an asynchronous payment processing pipeline that removes external payment provider latency from the HTTP request lifecycle.

AWS Lambda functions for asynchronous processing.
SQS FIFO, SNS, S3, and CloudWatch infrastructure.
Partial batch failure handling to prevent unnecessary message reprocessing.
Layered retry policies and dead-letter queues.
Infrastructure provisioned through Serverless Framework.

Stack: Node.js · TypeScript · AWS Lambda · SQS · SNS · CloudWatch

02. Idempotent Payment Processing

<img src="https://img.shields.io/badge/Focus-Data_Consistency-0891B2?style=flat-square"/>
<img src="https://img.shields.io/badge/Database-PostgreSQL-4169E1?style=flat-square"/>

Designed payment flows that prevent duplicate charges under retries, concurrent requests, and partial infrastructure failures.

Idempotency keys enforced by database unique constraints.
Optimistic concurrency control using conditional updates.
Stable idempotency keys reused across provider retries.
Explicit separation between external payment effects and local database transactions.

Stack: NestJS · PostgreSQL · Prisma ORM · SQS

03. Transactional Outbox

<img src="https://img.shields.io/badge/Pattern-Transactional_Outbox-6366F1?style=flat-square"/>
<img src="https://img.shields.io/badge/Messaging-RabbitMQ_%7C_AWS-0891B2?style=flat-square"/>

Implemented reliable domain event publication without coupling database commits to broker availability.

Domain state changes and outbox events persisted in the same database transaction.
Asynchronous publishing with exponential backoff.
Dead-letter handling for messages that exhaust their retry policy.
Reusable approach across SQS/SNS and RabbitMQ.

Stack: PostgreSQL · Prisma · RabbitMQ · SQS · SNS

04. Payment Gateway Integrations

<img src="https://img.shields.io/badge/Payments-Stripe-635BFF?style=flat-square&logo=stripe&logoColor=white"/>
<img src="https://img.shields.io/badge/Payments-Mercado_Pago-00AEEF?style=flat-square"/>
<img src="https://img.shields.io/badge/Security-HMAC-0891B2?style=flat-square"/>

Integrated Stripe and Mercado Pago for checkout, PIX payments, and authenticated webhook processing.

HMAC signature verification before payment state changes.
Shared payment state machine for checkout and PIX flows.
Idempotent processing and explicit handling of uncertain provider outcomes.
Protection against inconsistent local state following external authorization.

Stack: NestJS · TypeScript · Stripe · Mercado Pago · PIX · Webhooks

<div align="center">

<a href="https://github.com/akyriuu?tab=repositories">
<img src="https://img.shields.io/badge/Explore_all_projects-akyriuu-0891B2?style=for-the-badge&logo=github" alt="Explore projects"/>
</a>

</div>

# What I use.

<div align="center">

Backend Engineering

<img src="https://skillicons.dev/icons?i=nodejs,ts,nestjs,express&theme=dark" alt="Node.js, TypeScript, NestJS and Express"/>

Databases & Messaging

<img src="https://skillicons.dev/icons?i=postgres,redis,rabbitmq&theme=dark" alt="PostgreSQL, Redis and RabbitMQ"/>

Cloud & Infrastructure

<img src="https://skillicons.dev/icons?i=aws,docker,terraform,githubactions,linux&theme=dark" alt="AWS, Docker, Terraform, GitHub Actions and Linux"/>

Testing & Frontend

<img src="https://skillicons.dev/icons?i=jest,vitest,react,nextjs,git&theme=dark" alt="Testing, React, Next.js and Git"/>

</div>

Area	Technologies and practices
Backend	Node.js, TypeScript, NestJS, REST APIs
Architecture	Clean Code, SOLID, event-driven systems, state machines
Data	PostgreSQL, Prisma, Redis, schema migrations, indexing
Messaging	SQS FIFO, SNS, RabbitMQ, transactional outbox
Reliability	Idempotency, retries, backoff, DLQs, partial batch failures
Payments	Stripe, Mercado Pago, PIX, HMAC webhooks
AWS	Lambda, SQS, SNS, S3, CloudWatch, IAM
DevOps	Docker, Docker Compose, Serverless Framework, GitHub Actions
Testing	Jest, Vitest, Supertest, Testcontainers
Frontend	React, Next.js
~/engineering-decisions

I enjoy solving the problems that only appear when a system encounters real-world failures.

<details>
<summary><strong>01 — Why isn't idempotency just an application-level check?</strong></summary>

A read-then-write check can fail under concurrency. Two requests may both observe that a payment has not been processed.

I use database-enforced uniqueness as the final protection against duplicate operations, combined with stable idempotency keys and explicit handling of retries.

Principle: enforce invariants at the strongest layer available.

</details>

<details>
<summary><strong>02 — Why keep external payment calls outside database transactions?</strong></summary>

A database rollback cannot undo a payment provider's successful authorization. Holding a transaction open during a network request also increases contention and failure exposure.

I separate external effects from local state transitions and explicitly model uncertain outcomes, reconciliation, and safe retries.

Principle: a local transaction cannot make a remote side effect atomic.

</details>

<details>
<summary><strong>03 — How do you avoid losing events when a broker is unavailable?</strong></summary>

The transactional outbox stores domain changes and their corresponding events in the same database transaction. A separate publisher delivers pending events and retries transient failures.

Principle: persist intent before attempting asynchronous delivery.

</details>

<details>
<summary><strong>04 — Why shouldn't one invalid message fail an entire batch?</strong></summary>

Partial batch failure handling lets successfully processed messages remain successful while failed messages can be retried independently.

Combined with bounded retries, a dead-letter queue, and monitoring, this limits unnecessary work and improves operational visibility.

Principle: isolate failures instead of amplifying them.

</details>

<details>
<summary><strong>05 — Why is observability part of reliability?</strong></summary>

Retries alone do not explain whether a dependency is failing, a message is stuck, or a queue is accumulating errors.

Metrics, structured logs, and actionable alarms help distinguish transient failures from incidents that need intervention.

Principle: a failure that cannot be detected promptly is harder to recover from safely.

</details>

# Activity

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=akyriuu&show_icons=true&hide_border=true&bg_color=0D1117&title_color=22D3EE&icon_color=818CF8&text_color=C9D1D9&rank_icon=github" height="180" alt="GitHub statistics"/>

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=akyriuu&layout=compact&hide_border=true&bg_color=0D1117&title_color=22D3EE&text_color=C9D1D9&langs_count=8" height="180" alt="Most used languages"/>

<br/>

<img src="https://streak-stats.demolab.com/?user=akyriuu&hide_border=true&background=0D1117&ring=22D3EE&fire=818CF8&currStreakLabel=22D3EE&sideLabels=C9D1D9&currStreakNum=FFFFFF&sideNums=FFFFFF&dates=8B949E" width="80%" alt="GitHub contribution streak"/>

<br/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=akyriuu&bg_color=0D1117&color=C9D1D9&line=0891B2&point=818CF8&area=true&hide_border=true" width="100%" alt="GitHub activity graph"/>

</div>

# Currently

🔭 Focused on backend engineering, payment reliability, and AWS.
🧩 Interested in distributed systems and event-driven architecture.
🧪 Improving automated testing and failure-handling strategies.
🌱 Continuously learning about cloud architecture and production systems.
💼 Open to backend engineering opportunities and freelance projects.
# Contact

Have a backend challenge, a payment system to build, or an interesting engineering opportunity?

<div align="center">

<a href="mailto:akyriu@hotmail.com">
<img src="https://img.shields.io/badge/Email-akyriu%40hotmail.com-0891B2?style=for-the-badge&logo=gmail&logoColor=white" alt="Email Marcus"/>
</a>

<a href="https://www.linkedin.com/in/marcusvin%C3%ADcius-/">
<img src="https://img.shields.io/badge/LinkedIn-Let's_connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="Connect on LinkedIn"/>
</a>

<a href="https://github.com/akyriuu">
<img src="https://img.shields.io/badge/GitHub-akyriuu-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub profile"/>
</a>

<br/><br/>

<img src="https://media.giphy.com/media/qgQUggAC3Pfv687qPC/giphy.gif" width="320" alt="Developer coding animation"/>

Reliable systems. Explicit trade-offs. Software built to handle failure.

Designed and built with ☕ by Marcus Vinícius · Brazil 🇧🇷

<img src="https://capsule-render.vercel.app/api?type=waving&height=110&color=0:0891B2,50:172554,100:09090B&section=footer" width="100%" alt="Footer decoration"/>

</div>
