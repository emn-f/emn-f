<p align="center">
  <a href="https://emn-f.github.io/holmes/pt-br/">
    <img src="./.github/assets/banner.svg" alt="Emanuel Ferreira aka HOLMES_" width="100%" />
  </a>
</p>

<p align="center">
  <a href="https://emn-f.github.io/holmes/pt-br/"><b>Portfólio</b></a> ·
  <a href="https://www.linkedin.com/in/emanuelferreira">LinkedIn</a> ·
  <a href="https://medium.com/@emnferreira">Medium</a> ·
  <a href="http://lattes.cnpq.br/1681360365008995">Lattes</a> ·
  <a href="mailto:emnferreira.wk@gmail.com">Email</a>
</p>

## Oi, eu sou o Emanuel

Sou de Salvador, curso Engenharia de Software na UCSal (conclusão em 2028) e sou técnico em TI pelo IFBA. Trabalho com TI desde 2022: comecei testando ERP, passei por suporte e banco de dados, e hoje atuo com infraestrutura e automação na Continental, ao mesmo tempo em que mantenho projetos próprios em produção.

O que mais me interessa é backend, dados e segurança aplicados a problemas reais, e foi isso que eu fiz até agora:

- **Vox AI:** assistente open source de informação e acolhimento para a população LGBTQIA+ de Salvador. Sou fundador e tech lead. Nasceu como um MVP em planilhas e hoje roda com RAG sobre Supabase.
- **MentoraOS:** SaaS de gestão pedagógica para escolas, multi-tenant e em produção desde 2026.
- **Continental:** administro acessos no Active Directory e escrevo automações em Python e PowerShell para auditoria de endpoints.
- **Antes disso:** dois anos e meio mexendo com SQL, ETL e migração de dados em sistemas de folha de pagamento e ERP.

Estou buscando minha próxima posição como analista ou assistente júnior em desenvolvimento, dados ou segurança. O jeito mais rápido de falar comigo é por [email](mailto:emnferreira.wk@gmail.com) ou [LinkedIn](https://www.linkedin.com/in/emanuelferreira). Mais detalhes, diagramas e demos estão no [portfólio](https://emn-f.github.io/holmes/pt-br/), que também tem versão em inglês.

---

## Projetos principais

### Vox AI

O primeiro MVP usava planilhas, JSON no repositório e um modelo de embeddings local que era baixado a cada boot do Streamlit. Funcionava para a demo, mas não escalava.

Migrei a base para Supabase com `pgvector`, troquei a inferência local por chamadas de API (Gemini) e desenhei o projeto para não coletar dado pessoal nenhum. Isso reduziu o uso de RAM em cerca de 80% e permitiu atender mais gente ao mesmo tempo.

Para não depender de revisão manual, criei o **Gatekeep**: um funil em Git hooks e GitHub Actions que procura segredos vazados, confere migrations e pede uma revisão ao Gemini sobre o diff já sanitizado. O Semgrep roda junto na esteira.

[Repositório](https://github.com/emn-f/vox-ai) · [Documentação](https://emn-f.github.io/vox-ai-docs/) · [Aplicação](https://vox-ai.streamlit.app/)

### MentoraOS

Escolas precisam de isolamento forte entre os dados de cada instituição e de proteção para informações de alunos. O sistema é dividido em dois: um control plane (`mentora-adm`), que faz o onboarding das escolas sem intervenção manual, e um data plane (`mentora-os`), onde ficam os dados.

O isolamento entre tenants é feito com Row Level Security no PostgreSQL. Dados sensíveis ficam criptografados em repouso (AES-256-GCM), senhas usam Argon2id e os segredos de cada tenant ficam no Infisical. Arquivos vão para um bucket privado no Cloudflare R2, e o deploy é feito em containers na OCI, com imagens verificadas pelo Trivy. A stack é React 19, Node.js e Express 5.

[mentoraos.com](https://mentoraos.com) · [app.mentoraos.com](https://app.mentoraos.com)

### Odé CLI e KillerOffice (Continental)

Auditar software não homologado nas estações exigia interromper o usuário e procurar à mão instalações portáteis, chaves de registro e tarefas agendadas. O Odé CLI faz esse trabalho remotamente: um orquestrador em Python que dispara agentes em PowerShell. Em mais de 40 testes, o tempo gasto pelos auditores caiu cerca de 90%.

O KillerOffice complementa a ferramenta com um diagnóstico somente leitura de licenciamento do Microsoft Office 365, para apoiar decisões de custo sem mexer nas máquinas. Os dois são projetos privados da empresa, por isso não há repositório público.

---

## Outros projetos

| Projeto | O que é | Stack |
| :--- | :--- | :--- |
| [Respire](https://respiretea-mvp.vercel.app/) (beta) | Jogo narrativo de cartas para treinar flexibilidade cognitiva e autorregulação (respiração 4-7-8) em jovens com TEA | React 19, TypeScript, Tailwind, Vitest |
| [PsiBook](https://psibook-site.vercel.app) | Prontuário eletrônico para psicólogos, com isolamento por RLS e um modo de privacidade que borra a tela em 1 clique | Next.js 15, TypeScript, Supabase |
| [Sonitus](https://github.com/emn-f/sonitus) | Mapa comunitário de ruído urbano para acessibilidade sensorial (extensão UCSal) | TypeScript |
| [EcoCílios](https://github.com/emn-f/ecocilios) | Prevenção de enchentes urbanas com IoT e biomimética (extensão UCSal) | IoT |
| [Plumbum](https://github.com/emn-f/plumbum) | Plataforma de correção de textos, feita no Grupo de Pesquisa Mosaico (bolsa IFBA) | React, TypeScript, PHP, MySQL |
| bomberman-sd | Bomberman 1v1 em Java RMI, com uma ponte HTTP local para o frontend em React | Java, React, JUnit 5 |
| mentora-pw | CLI que grava as demos dos produtos como código (Playwright + FFmpeg) | TypeScript |

---

## Pesquisa e escritos

- **Prêmio Jovem Cientista 2026 (CNPq):** submeti o artigo *Vox AI: Inteligência Artificial e Ética no Acesso a Direitos Civis*, orientado pela Profa. Angela Peixoto Santana (UCSal). Avaliei o assistente em 65 cenários com LLM-as-a-Judge e obtive 94,5% de fidelidade normativa e 85,1% de revocação. [Artigo (PDF)](https://drive.google.com/file/d/10Ln4yzmlf9YjXhTkt5MzPCfZjReVknlD/view?usp=drivesdk) · [Repositório da pesquisa](https://github.com/emn-f/vox-ai/tree/develop/cnpq)
- **NOSS 2026:** palestra *De Sheets a um RAG escalável: como evoluí a arquitetura do Vox AI*. [Assistir](https://www.youtube.com/live/2GLyGSolizQ?t=15600&is=V7f9KamR9Vuf0V3I)
- **Baralho Inorgânico:** jogo para aprender funções químicas, 1º lugar no Prêmio Jovem na Ciência (2019) e publicado na Revista Jovens Cientistas (2021). [Artigo (PDF)](https://encontrodejovenscientistas.wordpress.com/wp-content/uploads/2021/11/revista-jc_2021_final_19-11_2.pdf)
- **Medium:** [Do MVP ao RAG: como o Vox AI evoluiu de planilhas para uma arquitetura escalável com Supabase](https://emnferreira.medium.com/do-mvp-ao-rag-como-o-vox-ai-evoluiu-de-planilhas-para-uma-arquitetura-escal%C3%A1vel-com-supabase-4c51b951ed56)
- **LinkedIn:** [Gatekeep: DevSecOps e code review com IA no Vox AI](https://lnkd.in/p/enFbtGYi)

---

## Tecnologias

<img src="https://skillicons.dev/icons?i=python,ts,js,nodejs,express,java,react,nextjs,tailwind,postgres,mysql,supabase,prisma,docker,linux,githubactions,powershell,cloudflare,vitest,playwright,git&perline=11" alt="Tecnologias que uso" />

---

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/emn-f/emn-f/refs/heads/output/github-contribution-grid-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/emn-f/emn-f/refs/heads/output/github-contribution-grid-snake.svg" />
    <img alt="github contribution grid snake animation" src="https://raw.githubusercontent.com/emn-f/emn-f/refs/heads/output/github-contribution-grid-snake.svg" />
  </picture>
</p>
