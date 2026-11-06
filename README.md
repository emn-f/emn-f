<h1>Emanuel Ferreira <sub><sup>aka Holmes</sup></sub></h1>

**Engenharia de Software (UCSal)** · **Técnico em TI (IFBA)** · **IT Intern @ Continental AG** · **Tech Lead @ Projeto Vox**

## Sobre mim

Sou estudante de Engenharia de Software e profissional de TI focado em construir sistemas seguros, automações de infraestrutura e arquiteturas orientadas a dados.

- **Corporativo & SecOps:** Atuo na **Continental AG** com gestão de identidades e acessos (IAM) via Active Directory, conformidade e padronização de endpoints e automação de auditorias técnicas.
- **Dados & Backend:** Mais de 2 anos de experiência prática trabalhando com múltiplos SGBDs em produção, trabalhando com rotinas de ETL, limpeza, migrações críticas de bancos de dados e investigação de causa raiz via SQL.
- **Open Source & IA:** Sou fundador e Tech Lead do **Projeto Vox AI**, onde desenho a arquitetura ponta a ponta: banco vetorial, pipeline RAG, integração de LLMs e esteiras de DevSecOps.
- **Comunidade:** Palestrante no [NOSS 2026](https://github.com/cumbucadev/NOSS), voluntário em eventos de hacking/segurança e presença constante em comunidades de IA e software livre. Tudo feito da comunidade pra comunidade faz meu coração bater mais forte.

**Foco atual:** Engenharia de Software (Backend/Full-Stack) · DevSecOps & Automação · Engenharia de Dados (SQL/ETL) · GenAI & RAG


## Destaques

### 1. Projeto Vox AI (Open Source)
Assistente de IA com busca semântica (RAG) voltado à saúde e apoio da comunidade LGBTQIA+.

| Problema | Solução | Resultado |
| :--- | :--- | :--- |
| MVP sem escala (Google Sheets/JSON) | Migração para Supabase (PostgreSQL + `pgvector`) | Arquitetura escalável com RLS |
| Inferência local pesada (Sentence Transformers) | Substituição por APIs externas + Gemini | ~80% de redução no uso de RAM |
| Revisão manual de segurança e banco | **Gatekeeper** (Python + GitHub Actions + AI Review) | PRs, segredos e migrations validados automaticamente |

🔗 [Repositório](https://github.com/emn-f/vox-ai) · [Documentação Técnica](https://github.com/emn-f/vox-ai-docs) · [Deploy](https://vox-ai.streamlit.app/)

### 2. Outros Projetos e Ferramentas
- **Ecossistema MentoraOS** *(SaaS B2B Multi-Tenant — Privado)*: Plataforma educacional dividida em *Data Plane* e *Control Plane* com Node.js/Express 5, React 19, PostgreSQL (RLS), criptografia de PII em repouso (`AES-256-GCM`), hashing `Argon2id`, gerenciamento de segredos por tenant via **Infisical**, armazenamento privado no **Cloudflare R2** e orquestração em **DevContainers + OCI**. Saiba mais em [https://mentoraos.com](https://mentoraos.com) 
- **Odé CLI & KillerOffice** *(Automação SecOps & FinOps — Privados)*: Ferramentas CLI em Python e PowerShell para auditoria remota de conformidade de softwares em estações Windows (incluindo montagem segura de `NTUSER.DAT` em perfis deslogados) e coleta *read-only* de evidências para otimização de licenciamento M365.
- **[Sonitus](https://github.com/emn-f/sonitus)** *(Open Source)*: Plataforma web de acessibilidade sensorial (React + TypeScript) projetada sob o conceito *Sensory Sanctuary*, com suporte nativo a redução de movimento (`prefers-reduced-motion`) e mapeamento de conforto acústico urbano.
- **[Chat Scott](https://github.com/emn-f/chat-scott) e Bomberman SD** *(Sistemas Distribuídos)*: Implementações de comunicação distribuída em **Java RMI** puro com callbacks remotos bidirecionais e arquitetura *Local HTTP Adapter Bridge* integrando Java RMI a um frontend **React + HTML5 Canvas**.


## Tech Stack

**Linguagens, Backend & Frontend**
<div align="left">
  <img src="https://skillicons.dev/icons?i=python,ts,js,nodejs,express,java,spring,react&perline=10" alt="Backend and Frontend Stack" />
</div>

**Dados, Cloud, DevSecOps & Automação**
<div align="left">
  <img src="https://skillicons.dev/icons?i=postgres,mysql,supabase,prisma,docker,linux,githubactions,powershell,git&perline=10" alt="Data and DevOps Stack" />
</div>


## Artigos
Compartilho um pouco do que aprendo na prática:
- 📝 [Do MVP ao RAG: Como o Vox AI evoluiu de planilhas para uma arquitetura escalável com Supabase](https://emnferreira.medium.com/do-mvp-ao-rag-como-o-vox-ai-evoluiu-de-planilhas-para-uma-arquitetura-escal%C3%A1vel-com-supabase-4c51b951ed56)


## Contato

<div>
  <a href="mailto:emnferreira.wk@gmail.com"><img src="https://img.shields.io/badge/-Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail" /></a>
  <a href="https://www.linkedin.com/in/emanuelferreira"><img src="https://img.shields.io/badge/-LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://emnferreira.medium.com"><img src="https://img.shields.io/badge/-Medium-12100E?style=for-the-badge&logo=medium&logoColor=white" alt="Medium" /></a>
  <a href="http://lattes.cnpq.br/1681360365008995"><img src="https://img.shields.io/badge/-Lattes-1A73E8?style=for-the-badge&logo=google-scholar&logoColor=white" alt="Lattes" /></a>
</div>

---

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/emn-f/emn-f/refs/heads/output/github-contribution-grid-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/emn-f/emn-f/refs/heads/output/github-contribution-grid-snake.svg" />
    <img alt="github contribution grid snake animation" src="https://raw.githubusercontent.com/emn-f/emn-f/refs/heads/output/github-contribution-grid-snake.svg" />
  </picture>
</p>
