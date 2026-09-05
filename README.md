<p align="center">
  <img src="name-animado.svg" alt="Sérgio Guilherme" width="100%" style="max-width:700px;" />
</p>

<h3 align="center">Desenvolvedor Backend Java & Spring Boot · Estudante de Ciência da Computação (UFPB)</h3>

<p align="center">
  <img src="https://skillicons.dev/icons?i=java,spring,hibernate,mysql,react,vite,ts,js,html,css,git,githubactions,docker,maven,postman" />
</p>

<p align="center">
  <sub>
    <img src="https://cdn.simpleicons.org/gmail/EA4335" width="14" height="14" valign="middle"/> <a href="mailto:sergiodeveloperprofissional27@gmail.com">sergiodeveloperprofissional27@gmail.com</a> ·
    <img src="https://cdn.simpleicons.org/github/9e9e9e" width="14" height="14" valign="middle"/> <a href="https://github.com/umdevaprendiz">github.com/umdevaprendiz</a> ·
    <img src="https://appstudying.onrender.com/favicon.svg" width="14" height="14" valign="middle"/> <a href="https://appstudying.onrender.com">appstudying.onrender.com</a>
  </sub>
</p>

---

### Sobre mim

Estudante de Ciência da Computação (UFPB) em busca de estágio em Desenvolvimento Java / Full Stack, com foco em Backend.

Construí sozinho, do zero, aplicações completas ponta a ponta com Spring Boot e React — da modelagem do banco de dados à automação de deploy em produção — incluindo autenticação real, WebSocket, testes automatizados e CI/CD com Docker.

Aplico boas práticas de segurança por padrão (isolamento de credenciais, autorização por dono do recurso, rate limiting, proteção contra mass assignment) e mantenho o código versionado no Git com histórico limpo e organizado.

**Diferenciais:** autonomia para levar um projeto do zero à produção sem supervisão · segurança e controle de acesso pensados no design, não como algo adicionado depois · cobertura de testes (JUnit 5, Mockito, MockMvc) antes de considerar algo pronto · boa comunicação escrita e facilidade em equipes remotas.

---

### Projetos

<img src="https://appstudying.onrender.com/favicon.svg" width="16" height="16" valign="middle"/> **[AppStudying](https://github.com/umdevaprendiz/AppStudying)** — plataforma de estudos com rede social entre estudantes
`Spring Boot 4` `React (Vite)` `MySQL` `Docker` `WebSocket` — [em produção](https://appstudying.onrender.com)

AppStudying nasceu de um problema pessoal: estudar sozinho é fácil de abandonar. A plataforma organiza o estudo individual (matérias, cronômetro de sessão com histórico, linha do tempo de progresso) e, ao mesmo tempo, cria um espaço social entre estudantes — parceria de estudo par a par, feed de sugestões e chat privado em tempo real via WebSocket (STOMP/SockJS).

- Segurança orientada a dados sensíveis: verificação de e-mail obrigatória no cadastro, sessão persistida em banco, autorização por dono do recurso em todos os endpoints, rate limiting contra força bruta/spam e proteção contra mass assignment.
- Ciclo de vida completo de conta: exclusão protegida por confirmação em e-mail e expurgo automático diário de contas inativas via job agendado.
- Pipeline de deploy real em produção: Dockerfile multi-stage, CI no GitHub Actions (testes com MySQL real + build), migrations versionadas com Flyway e CSRF/CORS configurados.
- Cobertura de testes unitários (JUnit 5 + Mockito) em todas as camadas de serviço e testes de integração (MockMvc) validando autenticação e controle de acesso.

**[API Bank](https://github.com/umdevaprendiz/financialbank)** — API REST de simulação bancária
`Java` `Spring Boot` `Spring Security` `Docker` `Railway`

Evoluindo de uma simulação bancária para uma plataforma financeira com componente social — controle financeiro pessoal unido a uma camada social voltada a metas, não à exibição de gastos.

- **Perfil próprio:** cada usuário tem um perfil, como uma rede social, mas com posts sobre conquistas financeiras — reserva de emergência formada, dívida quitada, meta de economia batida — em vez de fotos do dia a dia.
- **Feed e conexões:** possibilidade de seguir outras pessoas e acompanhar essas conquistas em um feed, criando um incentivo social para manter o controle financeiro.
- **Motor de análise de gastos:** categorização das transações, limite de gasto definido por categoria, cálculo de quanto ainda pode ser gasto no mês e quanto foi efetivamente guardado no período.
- **Base técnica reaproveitada:** o modelo de dados atual (contas, transações, papéis de usuário) seria estendido para suportar perfis, posts, seguidores e metas, mantendo a mesma autenticação e autorização por papéis já implementadas.

---

### Formação & idiomas

Ciência da Computação — UFPB *(previsão de conclusão: 2030)* · Técnico em Redes de Computadores — ETEMERB
Português (nativo) · Inglês (B2) · Espanhol (básico/intermediário)
