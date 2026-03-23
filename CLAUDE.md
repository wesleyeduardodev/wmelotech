# CLAUDE.md — WMelo Tech Website

## Projeto
Site institucional (landing page) da empresa **WMelo Tech** (W E DE O MELO - TECNOLOGIA ME).

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
| **E-mail** | wesleyeduardo.dev@gmail.com |
| **WhatsApp** | https://wa.me/5598981650805 |

## CNAEs Registrados

1. **6201-5/01** — Desenvolvimento de programas de computador sob encomenda (principal)
2. **6204-0/00** — Consultoria em tecnologia da informação
3. **6202-3/00** — Desenvolvimento e licenciamento de programas customizáveis
4. **6209-1/00** — Suporte técnico, manutenção e outros serviços em TI
5. **9511-8/00** — Reparação e manutenção de computadores e de equipamentos periféricos
6. **6311-9/00** — Tratamento de dados, hospedagem e atividades relacionadas
7. **8599-6/03** — Treinamento em informática

## Objetivo do Site

Landing page institucional para apresentar a empresa, serviços e captar clientes. **Não é e-commerce, não é blog, não é SaaS.** É uma página única de apresentação profissional.

## Stack & Decisões Técnicas

- **HTML/CSS/JS puro** — arquivo único `index.html`, sem framework
- **Fonts**: Outfit (display/headings) + JetBrains Mono (code/labels)
- **Estilo visual**: Dark mode, tech moderno
- **Cor accent**: `#00d4aa` (verde-tech)
- **Background**: `#0a0a0f` (quase preto com tom azulado)
- **Responsivo**: Mobile-first com breakpoints em 900px e 600px
- **Animações**: Scroll reveal (IntersectionObserver), typing effect no code block, orbs flutuantes, hover effects nos cards
- **Sem dependências externas** (exceto Google Fonts)

## Seções do Site

1. **Navegação** — Logo + links âncora + CTA "Fale Conosco" (fixo no topo, blur ao scroll)
2. **Hero** — Badge "disponível para projetos", título com accent/outline, descrição, botões (WhatsApp + Serviços), stats (10+ anos, 50+ projetos, 99% uptime)
3. **Sobre** — Code window animado com dados da empresa + texto descritivo + tags de tecnologias
4. **Serviços** — 6 cards representando os CNAEs:
   - Desenvolvimento Sob Medida (6201-5/01 + 6202-3/00)
   - Integrações Financeiras (especialidade do Wesley — PIX, boletos, BolePix)
   - Consultoria em TI (6204-0/00)
   - Cloud & DevOps (6311-9/00 + 6209-1/00)
   - Suporte Técnico (9511-8/00)
   - Treinamentos (8599-6/03)
5. **Depoimentos** — 3 cards (atualmente placeholders, substituir por reais)
6. **Contato** — CTA box com WhatsApp, e-mail, telefone e localização
7. **Footer** — Copyright + CNPJ + links

## Perfil Profissional do Wesley (para textos do site)

- Senior Software Engineer com 10+ anos de experiência
- Especialista em **Java/Spring Boot**, microserviços, PostgreSQL
- Forte em **integrações bancárias**: Santander, Bradesco, PIX, BolePix, Paymee
- Trabalha atualmente com sistemas financeiros na CVC Corp (maior grupo de viagens da América Latina)
- Professor no IFMA — ministra cursos de programação e IA
- Stack principal: Java, Spring Boot, React, React Native, PostgreSQL, Kubernetes, Docker, ArgoCD
- Localizado em Santa Luzia, Maranhão

## Tecnologias para Tags/Skills no Site

Java, Spring Boot, React, React Native, PostgreSQL, Kubernetes, Docker, ArgoCD, APIs Bancárias, PIX, Boletos, Microserviços, IA, Python, Git

## Contabilidade

- **Contador**: Henrique de Sousa Bueno — HB Contabilidade
- **CRC**: MA-015729/O-4
- **Contato contador**: (99) 98102-5333 | contato.hbcont@gmail.com
- **Honorários**: R$ 190,00/mês

## Paleta de Cores (CSS Variables)

```css
--bg-primary: #0a0a0f;
--bg-secondary: #12121a;
--bg-card: #16161f;
--accent: #00d4aa;
--accent-glow: rgba(0, 212, 170, 0.15);
--text-primary: #e8e8ef;
--text-secondary: #8888a0;
--text-muted: #55556a;
```

## Regras de Estilo

- NUNCA usar fontes genéricas (Arial, Inter, Roboto)
- NUNCA usar gradientes roxos clichê
- Manter o dark mode consistente em todo o site
- Priorizar animações CSS puras (performance)
- Todo texto visível deve ser em português (pt-BR)
- Labels de seção usam formato `// nome da seção` em mono
- Cards com hover que eleva (translateY) e borda accent

## Domínio (pendente)

- Domínio desejado: `wmelotech.com.br` (verificar disponibilidade no Registro.br)
- Alternativa: `wmelo.tech`

## TODO / Melhorias Futuras

- [ ] Substituir depoimentos placeholder por reais
- [ ] Adicionar favicon personalizado
- [ ] Adicionar meta tags Open Graph (compartilhamento social)
- [ ] Configurar Google Analytics
- [ ] Registrar e conectar domínio
- [ ] Deploy (Vercel, Netlify ou servidor próprio)
- [ ] Adicionar seção de portfólio com projetos reais
- [ ] Criar logo profissional da WMelo Tech
- [ ] Implementar formulário de contato (opcional)
- [ ] SEO: sitemap.xml, robots.txt
