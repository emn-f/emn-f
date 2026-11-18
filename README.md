<p align="center">
  <a href="https://emn-f.github.io/holmes/pt-br/">
    <img src="./.github/assets/banner.svg" alt="Emanuel Ferreira aka HOLMES_" width="100%" />
  </a>
</p>

<p align="center">
  <a href="https://emn-f.github.io/holmes/pt-br/"><img src="https://img.shields.io/badge/PORTF%C3%93LIO-HOLMES__%20%E2%86%97-e62429?style=for-the-badge&labelColor=090d16" alt="Portfólio HOLMES_" /></a>
  <a href="https://www.linkedin.com/in/emanuelferreira"><img src="https://img.shields.io/badge/LINKEDIN-%2Femanuelferreira-0891b2?style=for-the-badge&labelColor=090d16" alt="LinkedIn" /></a>
  <a href="https://medium.com/@emnferreira"><img src="https://img.shields.io/badge/MEDIUM-%40emnferreira-6ee7b7?style=for-the-badge&labelColor=090d16" alt="Medium" /></a>
  <a href="http://lattes.cnpq.br/1681360365008995"><img src="https://img.shields.io/badge/CNPQ-LATTES-f1f1f6?style=for-the-badge&labelColor=090d16" alt="Currículo Lattes" /></a>
  <a href="mailto:emnferreira.wk@gmail.com"><img src="https://img.shields.io/badge/CONTATO-EMAIL%20%E2%9C%89-e62429?style=for-the-badge&labelColor=090d16" alt="Email" /></a>
</p>

```text
$ whoami --context
> Emanuel Ferreira (Salvador, BA) · Graduando em Engenharia de Software (UCSal · 2028) · Técnico em TI (IFBA)
> Na área desde 2022: QA de ERP → Suporte & SQL/ETL → Infraestrutura, IAM (AD) e Automação na Continental
> Foco atual: posições como Analista ou Assistente Júnior em Desenvolvimento, Dados ou Segurança
```

---

## <img src="https://img.shields.io/badge/%C2%A7-01-e62429?style=flat-square&labelColor=e62429" alt="§ 01" /> Sistemas em Produção & Cases

<table>
  <thead>
    <tr>
      <th width="34%" align="left">Case / Sistema</th>
      <th align="left">Arquitetura & Impacto em Produção</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td valign="top">
        <h3>🌈 Vox AI</h3>
        <code>RAG · Supabase · Gemini · DevSecOps</code><br /><br />
        Fundador & Tech Lead<br /><br />
        <a href="https://github.com/emn-f/vox-ai"><b>Repositório</b></a> ·
        <a href="https://emn-f.github.io/vox-ai-docs/"><b>Docs</b></a> ·
        <a href="https://vox-ai.streamlit.app/"><b>App ↗</b></a>
      </td>
      <td valign="top">
        Assistente open source de informação e acolhimento para a população LGBTQIA+ de Salvador.<br /><br />
        • <b>De Planilhas a RAG escalável:</b> migração do MVP local para <code>Supabase + pgvector</code> e inferência via API Gemini, com política de coleta zero de dados pessoais e <b>redução de ~80% no consumo de RAM</b>.<br />
        • <b>Gatekeep (DevSecOps):</b> esteira em Git hooks + GitHub Actions com varredura de segredos, validação de migrations, Semgrep e code review automatizado sobre diff sanitizado.
      </td>
    </tr>
    <tr>
      <td valign="top">
        <h3>🏛️ MentoraOS</h3>
        <code>React 19 · Node.js · Express 5 · PostgreSQL · OCI</code><br /><br />
        SaaS Multi-Tenant em Produção<br /><br />
        <a href="https://mentoraos.com"><b>mentoraos.com</b></a> ·
        <a href="https://app.mentoraos.com"><b>App ↗</b></a>
      </td>
      <td valign="top">
        Plataforma SaaS de gestão pedagógica para escolas, dividida em <b>control plane</b> (<code>mentora-adm</code>, onboarding automatizado) e <b>data plane</b> (<code>mentora-os</code>).<br /><br />
        • <b>Segurança & Isolamento:</b> Row Level Security (RLS) no PostgreSQL, criptografia <code>AES-256-GCM</code> em repouso, senhas com <code>Argon2id</code> e gestão de segredos por tenant no <b>Infisical</b>.<br />
        • <b>Infraestrutura:</b> armazenamento privado no Cloudflare R2 e containers na OCI verificados com <b>Trivy</b>.
      </td>
    </tr>
    <tr>
      <td valign="top">
        <h3>🛡️ Odé CLI & KillerOffice</h3>
        <code>Python · PowerShell · Active Directory · M365</code><br /><br />
        Continental · Ferramentas Internas
      </td>
      <td valign="top">
        Automação de auditoria de endpoints e diagnóstico de licenciamento corporativo sem interromper o usuário.<br /><br />
        • <b>Odé CLI:</b> orquestrador em Python que dispara agentes em PowerShell para varrer instalações portáteis, chaves de registro e tarefas agendadas remotamente — <b>reduzindo em ~90% o tempo dos auditores</b> em mais de 40 baterias de teste.<br />
        • <b>KillerOffice:</b> diagnóstico somente leitura de licenciamento do Microsoft Office 365 para apoiar decisões de custo sem alterar as estações.
      </td>
    </tr>
  </tbody>
</table>

---

## <img src="https://img.shields.io/badge/%C2%A7-02-e62429?style=flat-square&labelColor=e62429" alt="§ 02" /> Outros Projetos & Laboratório

| Projeto | O que resolve | Stack |
| :--- | :--- | :--- |
| [**Respire**](https://respiretea-mvp.vercel.app/) `beta` | Jogo narrativo de cartas para treinar flexibilidade cognitiva e autorregulação (respiração 4-7-8) em jovens com TEA | `React 19` `TypeScript` `Tailwind` `Vitest` |
| [**PsiBook**](https://psibook-site.vercel.app) | Prontuário eletrônico para psicólogos com isolamento por RLS e modo de privacidade em 1 clique | `Next.js 15` `TypeScript` `Supabase` |
| [**Sonitus**](https://github.com/emn-f/sonitus) | Mapa comunitário de ruído urbano para acessibilidade sensorial (extensão UCSal) | `TypeScript` |
| [**EcoCílios**](https://github.com/emn-f/ecocilios) | Prevenção de enchentes urbanas com IoT e biomimética (extensão UCSal) | `IoT` |
| [**Plumbum**](https://github.com/emn-f/plumbum) | Plataforma de correção de textos desenvolvida no Grupo de Pesquisa Mosaico (bolsa IFBA) | `React` `TypeScript` `PHP` `MySQL` |
| **bomberman-sd** | Bomberman 1v1 em Java RMI com ponte HTTP local para frontend em React | `Java` `React` `JUnit 5` |
| **mentora-pw** | CLI que grava demos de produto a 60fps como código (Playwright + FFmpeg) | `TypeScript` `Playwright` |

---

## <img src="https://img.shields.io/badge/%C2%A7-03-e62429?style=flat-square&labelColor=e62429" alt="§ 03" /> Pesquisa Científica, Palestras & Escritos

<table>
  <thead>
    <tr>
      <th width="26%" align="left">Tipo · Ano</th>
      <th align="left">Produção & Links</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td valign="top"><b>Submissão Científica · 2026</b><br /><code>Prêmio Jovem Cientista (CNPq)</code></td>
      <td valign="top">
        <b>Vox AI: Inteligência Artificial e Ética no Acesso a Direitos Civis</b> (orientação: Profa. Angela Peixoto Santana — UCSal). Avaliação em 65 cenários com <i>LLM-as-a-Judge</i> atingindo <b>94,5% de fidelidade normativa</b> e <b>85,1% de revocação</b>.<br />
        <a href="https://drive.google.com/file/d/10Ln4yzmlf9YjXhTkt5MzPCfZjReVknlD/view?usp=drivesdk">Artigo (PDF) ↗</a> · <a href="https://github.com/emn-f/vox-ai/tree/develop/cnpq">Repositório da pesquisa ↗</a>
      </td>
    </tr>
    <tr>
      <td valign="top"><b>Palestra · 2026</b><br /><code>NOSS 2026</code></td>
      <td valign="top">
        <b>De Sheets a um RAG escalável: como evoluí a arquitetura do Vox AI</b><br />
        <a href="https://www.youtube.com/live/2GLyGSolizQ?t=15600&is=V7f9KamR9Vuf0V3I">Assistir gravação no YouTube ↗</a>
      </td>
    </tr>
    <tr>
      <td valign="top"><b>Artigos Técnicos · 2026</b><br /><code>Medium & LinkedIn</code></td>
      <td valign="top">
        • <a href="https://emnferreira.medium.com/do-mvp-ao-rag-como-o-vox-ai-evoluiu-de-planilhas-para-uma-arquitetura-escal%C3%A1vel-com-supabase-4c51b951ed56">Do MVP ao RAG: como o Vox AI evoluiu de planilhas para uma arquitetura escalável com Supabase (Medium) ↗</a><br />
        • <a href="https://lnkd.in/p/enFbtGYi">Gatekeep: DevSecOps e code review com IA no Vox AI (LinkedIn) ↗</a>
      </td>
    </tr>
    <tr>
      <td valign="top"><b>Prêmio & Publicação · 2019–2021</b><br /><code>Revista Jovens Cientistas</code></td>
      <td valign="top">
        <b>Baralho Inorgânico:</b> jogo didático para funções químicas — <b>1º lugar no Prêmio Jovem na Ciência (2019)</b> e publicado na Revista Jovens Cientistas (2021).<br />
        <a href="https://encontrodejovenscientistas.wordpress.com/wp-content/uploads/2021/11/revista-jc_2021_final_19-11_2.pdf">Artigo (PDF) ↗</a>
      </td>
    </tr>
  </tbody>
</table>

---

## <img src="https://img.shields.io/badge/%C2%A7-04-e62429?style=flat-square&labelColor=e62429" alt="§ 04" /> Tecnologias & Ferramentas

<p align="center">
  <img src="https://skillicons.dev/icons?i=python,ts,js,nodejs,express,java,react,nextjs,tailwind,postgres,mysql,supabase,prisma,docker,linux,githubactions,powershell,cloudflare,vitest,git&perline=10" alt="Tecnologias que uso" />
</p>

---

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/emn-f/emn-f/refs/heads/output/github-contribution-grid-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/emn-f/emn-f/refs/heads/output/github-contribution-grid-snake.svg" />
    <img alt="github contribution grid snake animation" src="https://raw.githubusercontent.com/emn-f/emn-f/refs/heads/output/github-contribution-grid-snake.svg" />
  </picture>
</p>
