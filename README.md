# Kelvin Biffi

### I build the interface and the reliability layer for AI products.

**AI Product Engineer** · React · Next.js · TypeScript · Python · **MCP** · AI Agents · LLM Evaluation
15+ years shipping production software · Remote, Brazil (UTC-3) · [kelvinbiffi.com](https://kelvinbiffi.com)

> AI made me faster. It did not make me necessary. Fifteen years of engineering did that, and it is why I can tell a model where to look instead of watching it guess.

I wrote the books on **MCP**, **Context Engineering** and **AI Agents in Python**. Then I shipped all three to production, which is a very different experience.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/kelvinbiffi/)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:kelvinbiffi.developer@gmail.com)
[![Website](https://img.shields.io/badge/kelvinbiffi.com-111?style=flat-square&logo=googlechrome&logoColor=white)](https://kelvinbiffi.com)
[![YellowKode](https://img.shields.io/badge/YellowKode%20Academy-FFD700?style=flat-square&logoColor=black)](https://yellowkode.com)

---

## The part most teams underbuild

An agent does not fail loudly.

It returns something plausible. The logs look clean. Three weeks later someone finds a corrupted record.

So I stopped trusting model output and started validating it like user input: **schema-constrained, value-checked, with guardrails that can refuse to answer**, evaluation loops, and cost tracked per conversation instead of per call.

That layer is most of what I do now. The other half is the interface on top of it, because a model's answer is worthless until a person can trust it and act on it.

---

## Products I built and run

| Product | What it is |
|---|---|
| **[Linkezera](https://linkezera.com)** | Link-in-bio SaaS. **3,700+ users** across LATAM. Built end to end. |
| **[Mentezinha](https://mentezinha.app)** | Child-safe conversational AI on Google Vertex AI. Built it for my son's homeschooling, now other families use it. With children as the users there is no acceptable failure rate, so the guardrail is a validation layer that can refuse to answer, not a line in a prompt. |
| **[StartAtende](https://startatende.com)** | AI-powered customer support on WhatsApp. Intent routing and cost control per conversation. |
| **[MentalKare](https://mentalkare.org)** | Accessible mental health platform, multilingual. |
| **[YellowKode Academy](https://yellowkode.com)** | Courses and technical books for developers. I teach the foundation that makes AI actually work. |

## Shipped for other people

- Subscription, billing and lifecycle flows on **Stripe**, used by thousands of paying members at **Firstleaf** (US wine subscription)
- An enterprise login and registration gateway with **Keycloak and MFA** serving **millions of users** at Lojas Renner
- A **Magento to Next.js migration** for Rede Drogasil, a national pharmacy chain. Two systems coexisting route by route, with high-volume checkout that could not go down during the cutover
- Frontend systems for **DIFC**, the Dubai International Financial Centre, and for **605 Media Analytics**
- A **Vue.js landing page builder** at Pmweb that cut development effort by **70%**, moving page creation out of the engineering queue and into the client's hands
- **Near Companion** at Hire With Near: a Chrome extension over an LLM pipeline with Recall.ai, Supabase, HubSpot, Cloudflare R2 and n8n. A bot joins the intake call as a silent participant and writes the structured job description live, during the call. I owned the whole interface, and every model output was schema-validated before it touched a CRM

---

## Stack

**Surface**
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react)
![Next.js](https://img.shields.io/badge/Next.js-000?style=flat-square&logo=nextdotjs)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)

**AI in production**
![Claude](https://img.shields.io/badge/Claude%20API-D97757?style=flat-square&logo=anthropic&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white)
![Vertex AI](https://img.shields.io/badge/Vertex%20AI-4285F4?style=flat-square&logo=googlecloud&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-000?style=flat-square)
![n8n](https://img.shields.io/badge/n8n-EA4B71?style=flat-square&logo=n8n&logoColor=white)

**Underneath**
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![GraphQL](https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

Agents with tool calling · MCP servers and clients · RAG and contextual retrieval · evaluation loops · guardrails · schema-constrained output · cost control · FFmpeg · WhisperX

**How I work:** Claude Code daily, with a written context file in every repo so the agent inherits the project's decisions instead of rediscovering them every session.

---

## Here on GitHub

Most of my production work is under contract and lives in private repos. What is public here is the teaching and the tooling.

- **[Guide-Book](https://github.com/kelvinbiffi/Guide-Book)** - design system and style guide generator that reads your CSS, SCSS, LESS or Stylus and produces the categories, elements and modules of your design system. On npm as [`guide-book-generator`](https://www.npmjs.com/package/guide-book-generator).
- **[javascript-book](https://github.com/kelvinbiffi/javascript-book)** - every code example from *JavaScript: Básico ao Avançado*.
- **[mcps](https://github.com/kelvinbiffi/mcps)** - MCP servers for Google Ads, Bing Ads and Meta Ads.
- **[Criando e aplicando um Style Guide do zero](https://github.com/kelvinbiffi/Criando-e-aplicando-um-Style-Guide-do-zero)** - full source for my design systems course.

---

## I write

Almost thirty published books. Four of them are the exact stack I work in.

**AI engineering**

| Book | |
|---|---|
| **MCP na Prática com Python** | [Amazon](https://www.amazon.com.br/dp/B0GX32HTH8) |
| **Context Engineering: O Guia Definitivo para LLMs** | [Amazon](https://www.amazon.com.br/dp/B0H1PTSJP7) |
| **Agentes de IA com Python** | [Amazon](https://www.amazon.com.br/dp/B0H2RZ1VBM) |
| **Spec Driven Development na Prática** | [Amazon](https://www.amazon.com.br/dp/B0H2RP3V54) |

<details>
<summary><b>Everything else I have written</b> (languages, fundamentals, and a cosmic horror series)</summary>

**Dev na Prática series**

- [JavaScript na Prática](https://www.amazon.com.br/dp/B0GZGG6Q77)
- [Go na Prática](https://www.amazon.com.br/dp/B0H3WTFPCW)
- [TDD na Prática com Python](https://www.amazon.com.br/dp/B0H2JRFTFT)
- [TypeScript na Prática](https://www.amazon.com.br/dp/B0GX6W5ZCV)
- [SQL na Prática com PostgreSQL](https://www.amazon.com.br/dp/B0H6688KL4)

**Technical, standalone**

- [JavaScript: Básico ao Avançado](https://www.amazon.com.br/dp/B0BS9VQTJW)
- [Lógica de Programação na Prática](https://www.amazon.com.br/dp/B0H3KVBPB2)
- [Guia do Programador Moderno](https://www.amazon.com.br/dp/B0H637DJGL)
- [Algoritmo para Leigos](https://www.amazon.com.br/dp/B0DG32258Z)

**Fiction: Arquivo Morto, a cosmic horror series**

- [O Andar que Não Existe](https://www.amazon.com.br/dp/B0H2ZBL27B) · [A Geometria do Arquiteto](https://www.amazon.com.br/dp/B0H2ZG8Z4V) · [O Corredor Sem Fim](https://www.amazon.com.br/dp/B0GXNQMJ43) · [A Escada do Consolação](https://www.amazon.com.br/dp/B0H3NN3QSB) · [O Arquivo Submerso](https://www.amazon.com.br/dp/B0H2W7C1NX) · [A Janela Fechada de Dentro](https://www.amazon.com.br/dp/B0H4F3D35M) · [O Jardim Sem Saída](https://www.amazon.com.br/dp/B0H581853P)

**Other**

- [MINTA!: Minta até que seja verdade](https://www.amazon.com.br/dp/B0GX3B6PMQ)
- [Método IAPA: Um Ciclo Constante de Crescimento Pessoal e Profissional](https://www.amazon.com.br/dp/B0DWMGVK5L)
- [As 5 Leis Universais do Dinheiro](https://www.amazon.com.br/dp/B0DTJHX4S6)
- [Construindo o Futuro: Os Benefícios do LEGO para Desenvolvimento Infantil](https://www.amazon.com.br/dp/B0DK6MRTDY)
- [O Menino Dentro da Cartola de Retalhos](https://www.amazon.com.br/dp/B0CW1CSD1N)
- [O Tamanduá Mensageiro do Rei](https://loja.uiclap.com/titulo/ua67047/)
- [Economópolis](https://economopolis.com.br/)

[→ All books on Amazon](https://www.amazon.com.br/s?i=digital-text&rh=p_27%3AKelvin%2BBaumhardt%2BBiffi&s=relevancerank&text=Kelvin+Baumhardt+Biffi)

</details>

---

Currently taking on remote contracts with US and European teams. UTC-3, so most of your day is my day too.

📩 **kelvinbiffi.developer@gmail.com** · [LinkedIn](https://www.linkedin.com/in/kelvinbiffi/) · [kelvinbiffi.com](https://kelvinbiffi.com)
