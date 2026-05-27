# CLAUDE.md — WMelo Tech Website

## Projeto
Site institucional (landing page) da empresa **WMelo Tech** (W E DE O MELO - TECNOLOGIA ME).
Arquivo único `index.html` na raiz, sem build, deploy via Railway com domínio próprio na Cloudflare.

---

## Dados da Empresa

| Campo | Valor |
|---|---|
| **Razão Social** | W E DE O MELO - TECNOLOGIA ME |
| **Nome Fantasia** | WMelo Tech |
| **CNPJ** | 65.736.086/0001-60 |
| **Natureza Jurídica** | Empresário Individual (EI) |
| **Porte** | ME - Microempresa |
| **Regime Tributário** | Simples Nacional |
| **Início das Atividades** | 13/03/2026 |
| **Sede** | Rua da Mangueira, S/N, Centro, Santa Luzia - MA, CEP 65.390-000 |
| **Titular** | Wesley Eduardo de Oliveira Melo |
| **Telefone** | (98) 98165-0805 |
| **E-mail** | contato@wmelotech.com.br (Cloudflare Email Routing → Gmail pessoal) |
| **WhatsApp** | https://wa.me/5598981650805 |
| **LinkedIn (fundador)** | https://www.linkedin.com/in/wesley-eduardo-8a1066169/ |

---

## CNAEs Registrados

1. **6201-5/01** — Desenvolvimento de programas de computador sob encomenda (principal)
2. **6204-0/00** — Consultoria em tecnologia da informação
3. **6202-3/00** — Desenvolvimento e licenciamento de programas customizáveis
4. **6209-1/00** — Suporte técnico, manutenção e outros serviços em TI
5. **9511-8/00** — Reparação e manutenção de computadores e de equipamentos periféricos
6. **6311-9/00** — Tratamento de dados, hospedagem e atividades relacionadas
7. **8599-6/03** — Treinamento em informática

---

## Posicionamento estratégico

**Não é só "mais uma dev shop".** A WMelo Tech tem um nicho claro que deve transparecer no site:

1. **Sistemas de missão crítica em produção** — passagens por CVC Corp (maior grupo de viagens da AL), Caixa Econômica via Globalweb (FGTS / Saque-Aniversário, milhões de usuários), Neogrid (fiscal nacional).
2. **Integrações financeiras** — especialidade do fundador: PIX, BolePix, boletos, APIs bancárias (Santander, Bradesco), gateways, sistemas de pagamento.
3. **IA aplicada com prova concreta** — Argonaut (Claude/OpenAI/Gemini + ArgoCD), ConstVision (pgvector + arquitetura pra NLQ), publicação acadêmica em IA (Computer on The Beach 2021), docência em IA no IFMA.
4. **Arquitetura sênior** — Java/Spring Boot, microsserviços, observabilidade, DevOps, segurança (OAuth2, JWT, cache distribuído).

O site deve **vender essa combinação rara**, não competir como dev genérico.

---

## Objetivo do Site

Landing page institucional para apresentar a empresa, serviços e captar clientes B2B. **Não é e-commerce, não é blog, não é SaaS.** É uma página única de apresentação profissional, otimizada para conversão (WhatsApp + e-mail).

---

## Stack & Decisões Técnicas

- **HTML/CSS/JS puro** — arquivo único `index.html`, sem framework, sem build step
- **Fonts**: Outfit (display/headings) + JetBrains Mono (code/labels)
- **Estilo visual**: Dark mode, tech moderno
- **Cor accent**: `#00d4aa` (verde-tech)
- **Background**: `#0a0a0f` (quase preto com tom azulado)
- **Responsivo**: Mobile-first com breakpoints em 900px e 600px
- **Animações**: Scroll reveal (IntersectionObserver), typing effect no code block, orbs flutuantes, hover effects
- **Sem dependências externas** (exceto Google Fonts)
- **Logo**: SVG inline (vector, sem fundo, escala perfeita) + `logo.png` na raiz para OG image / sharing
- **Deploy**: Railway (push pra branch `main` faz deploy automático)
- **DNS**: Cloudflare (nameservers `corey.ns.cloudflare.com` + `jade.ns.cloudflare.com`)
- **E-mail**: Cloudflare Email Routing — `contato@wmelotech.com.br` → forward pro Gmail pessoal

---

## Seções do Site (estado atual — 27/05/2026)

1. **Navegação** — Logo SVG inline + links âncora + CTA "Fale Conosco" (fixo no topo, blur ao scroll)
2. **Hero** — Badge "disponível para projetos", título com accent/outline, descrição, botões (WhatsApp + Serviços), stats (15+ anos, 7 projetos, 4 passagens corporativas)
3. **Sobre** — Code window animado com dados da empresa + texto descritivo + tags de tecnologias
4. **Serviços** — 6 cards representando os CNAEs (Dev Sob Medida / Integrações Financeiras / Consultoria TI / Cloud & DevOps / IA / Treinamentos)
5. **Projetos** — 6 cases reais clicáveis: ConstVision, F. Galvão Eng, DevQuote, Argonaut, PlanFin, Achei Pedreiro
6. **Trajetória** — Timeline vertical com 5 marcos: CVC Corp → Globalweb (Caixa/FGTS) → Neogrid → Mentor Construção → IFMA pesquisa → Início autodidata (2011-2018)
7. **Contato** — CTA box com WhatsApp, e-mail, telefone e localização
8. **Footer** — Copyright + CNPJ + links âncora

---

## Perfil Profissional do Wesley (para textos do site)

- Senior Software Engineer com 15+ anos no mercado
- Especialista em **Java/Spring Boot**, microsserviços, PostgreSQL
- Forte em **integrações bancárias**: Santander, Bradesco, PIX, BolePix, Paymee
- Trabalha atualmente com sistemas financeiros na **CVC Corp** (maior grupo de viagens da AL) — desde fev/2024
- **Professor no IFMA** — ministra cursos de programação e IA
- Stack principal: Java, Spring Boot, React, React Native, PostgreSQL, Kubernetes, Docker, ArgoCD
- **Publicação acadêmica em IA**: análise de sentimentos com SVM/Naive Bayes/redes neurais (Computer on The Beach 2021)
- Localizado em Santa Luzia, Maranhão

---

## Portfólio de Projetos Reais (referência para cards do site)

| Projeto | URL | Stack | Tipo |
|---|---|---|---|
| ConstVision | constvision.com.br | Java 25, Spring Boot 4, React 19, PostgreSQL/pgvector | SaaS multi-tenant para construção civil |
| F. Galvão Engenharia | fgalvaoeng.com.br | Next.js 16, Prisma 6, Auth.js v5, AWS S3 | Portfólio + admin |
| DevQuote | wesley.devquote.com.br | React/TS + Spring Boot, JWT, RBAC 4 níveis | Gestão de tarefas/faturamento |
| Argonaut | argonaut-six.vercel.app | Next.js 16, Claude/OpenAI/Gemini API, ArgoCD, AES-256 | Chat IA + DevOps |
| PlanFin | planfin-blue.vercel.app | Next.js, NextAuth, PostgreSQL, Prisma | Planejamento financeiro |
| Achei Pedreiro | achei-pedreiro-site-production.up.railway.app | Spring Boot, PostgreSQL, mobile | Marketplace |

---

## Tecnologias para Tags/Skills no Site

Java, Spring Boot, React, React Native, PostgreSQL, Kubernetes, Docker, ArgoCD, APIs Bancárias, PIX, Boletos, Microsserviços, IA, Claude API, RAG, pgvector, Python, Git

---

## Contabilidade

- **Contador**: Henrique de Sousa Bueno — HB Contabilidade
- **CRC**: MA-015729/O-4
- **Contato contador**: (99) 98102-5333 | contato.hbcont@gmail.com
- **Honorários**: R$ 190,00/mês

---

## Paleta de Cores (CSS Variables)

```css
--bg-primary: #0a0a0f;
--bg-secondary: #12121a;
--bg-card: #16161f;
--bg-card-hover: #1c1c28;
--accent: #00d4aa;
--accent-glow: rgba(0, 212, 170, 0.15);
--accent-dim: rgba(0, 212, 170, 0.6);
--text-primary: #e8e8ef;
--text-secondary: #8888a0;
--text-muted: #55556a;
--border: rgba(255,255,255,0.06);
--border-accent: rgba(0, 212, 170, 0.2);
```

---

## Regras de Estilo

- NUNCA usar fontes genéricas (Arial, Inter, Roboto)
- NUNCA usar gradientes roxos clichê
- Manter o dark mode consistente em todo o site
- Priorizar animações CSS puras (performance)
- Todo texto visível deve ser em português (pt-BR)
- Labels de seção usam formato `// nome da seção` em mono
- Cards com hover que eleva (translateY) e borda accent
- Logo na nav: SVG inline, nunca PNG (mantém nitidez retina + tema)

---

## Domínio & Infraestrutura

| Item | Status |
|---|---|
| Domínio `wmelotech.com.br` registrado no Registro.br | ✅ |
| Domínio na Cloudflare (nameservers configurados) | ⏳ Aguardando propagação |
| Site no Railway (`wmelotech-production.up.railway.app`) | ✅ Ativo |
| Domínio customizado no Railway (`wmelotech.com.br` + `www`) | ⏳ Aguardando DNS |
| Cloudflare Email Routing (`contato@wmelotech.com.br`) | ⏳ Aguardando zona Active |
| Gmail "Send mail as" configurado | ❌ Pendente (depois do Email Routing) |

---

## TODO / Roadmap

### Prioridade 1 — Posicionamento (próxima onda do site)
- [ ] **Seção dedicada "IA & Automação"** — destacar Argonaut, ConstVision NLQ, publicação acadêmica, docência IFMA
- [ ] **Promover Integrações Financeiras** como serviço-bandeira (reordenar)
- [ ] **Seção "Por que WMelo Tech"** com 3-4 diferenciais (sistemas críticos, IA aplicada, integrações financeiras, sr engineering)
- [ ] **Seção "Como Trabalhamos"** (processo: Descoberta → Spec → Sprint → Entrega → Suporte)
- [ ] **Logos de empresas onde Wesley atuou** (CVC, Caixa via Globalweb, Neogrid, Mentor) como prova social honesta

### Prioridade 2 — SEO técnico
- [ ] `sitemap.xml`
- [ ] `robots.txt`
- [ ] Schema.org `Service` em cada serviço
- [ ] Schema `FAQPage` (se criar FAQ)
- [ ] Google Analytics ou Plausible

### Prioridade 3 — Conversão
- [ ] Form de contato simples (nome / e-mail / mensagem)
- [ ] FAQ (preço, prazo, manutenção, processo)

### Prioridade 4 — Assets visuais
- [ ] Favicon de alta resolução (gerar quadrado a partir do icon do logo)
- [ ] `apple-touch-icon` (180x180)
- [ ] Versão da logo com fundo transparente (para outros usos)

### Prioridade 5 — Deploy & operação
- [ ] Confirmar SSL ativo no Railway após DNS propagar
- [ ] Configurar Gmail "Send mail as" → responder saindo como `contato@wmelotech.com.br`
- [ ] Validar OG image no [opengraph.dev](https://opengraph.dev) após propagação

### Concluído ✅
- [x] Hero, Sobre, Serviços, Contato, Footer iniciais
- [x] Seção Projetos (substituindo depoimentos placeholder)
- [x] Seção Trajetória (timeline com 5 marcos do LinkedIn)
- [x] JSON-LD LocalBusiness + sameAs LinkedIn do fundador
- [x] Open Graph + Twitter Card
- [x] Logo SVG inline na navegação (substituindo PNG)
- [x] Stats reais (15+ anos / 7 projetos / 4 passagens corporativas)
- [x] E-mail trocado pra `contato@wmelotech.com.br`
- [x] Domínio registrado e nameservers apontados pra Cloudflare
- [x] Email Routing configurado na Cloudflare (regra criada, aguardando ativação)

---

## Como trabalhar neste repo

- Editar `index.html` direto — arquivo único, sem build
- Para testar local: abrir `index.html` no browser (ou usar `python -m http.server` na raiz)
- Para deploy: `git push` na branch `main` — Railway detecta e faz redeploy
- Logo em PNG (`logo.png`) é usada como OG image — manter na raiz, committed no git
- Manter o tom do CSS: NUNCA introduzir frameworks ou bibliotecas — o diferencial é a leveza
