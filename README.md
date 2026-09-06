<p align="center">
  <img src="name-animado.svg" alt="Sérgio Guilherme" width="100%" style="max-width:700px;" />
</p>

<h3 align="center">Java & Spring Boot Backend Developer · Computer Science Student (UFPB)</h3>

<p align="center">
  <img src="https://skillicons.dev/icons?i=java,py,spring,hibernate,mysql,react,vite,ts,js,html,css,git,githubactions,docker,maven,postman" />
</p>

<p align="center">
  <sub>
    <img src="https://cdn.simpleicons.org/gmail/EA4335" width="14" height="14" valign="middle"/> <a href="mailto:sergiodeveloperprofissional27@gmail.com">sergiodeveloperprofissional27@gmail.com</a> ·
    <img src="https://cdn.simpleicons.org/github/9e9e9e" width="14" height="14" valign="middle"/> <a href="https://github.com/umdevaprendiz">github.com/umdevaprendiz</a> ·
    <img src="https://appstudying.onrender.com/favicon.svg" width="14" height="14" valign="middle"/> <a href="https://appstudying.onrender.com">appstudying.onrender.com</a>
  </sub>
</p>

---

### About me

Computer Science student (UFPB) looking for an internship in Java / Full Stack development, with a focus on Backend.

I've built complete, end-to-end applications on my own, from scratch, with Spring Boot and React — from database modeling to production deploy automation — including real authentication, WebSocket, automated testing, and CI/CD with Docker.

I apply security best practices by default (credential isolation, resource-owner authorization, rate limiting, protection against mass assignment) and keep code versioned in Git with a clean, organized history.

**Highlights:** autonomy to take a project from zero to production without supervision · security and access control designed in from the start, not bolted on afterward · test coverage (JUnit 5, Mockito, MockMvc) before considering anything done · good written communication and ease working in remote teams.

---

### Projects

<img src="https://appstudying.onrender.com/favicon.svg" width="16" height="16" valign="middle"/> **[AppStudying](https://github.com/umdevaprendiz/AppStudying)** — a study platform with a social network for students
`Spring Boot 4` `React (Vite)` `MySQL` `Docker` `WebSocket` — [live](https://appstudying.onrender.com)

AppStudying came out of a personal problem: studying alone is easy to give up on. The platform organizes individual study (subjects, session timer with history, progress timeline) while also creating a social space between students — peer study partnerships, a suggestions feed, and real-time private chat via WebSocket (STOMP/SockJS).

- Security built around sensitive data: mandatory email verification on signup, database-backed sessions, resource-owner authorization on every endpoint, rate limiting against brute force/spam, and protection against mass assignment.
- Full account lifecycle: deletion protected by email confirmation, and daily automatic purging of inactive accounts via a scheduled job.
- Real production deploy pipeline: multi-stage Dockerfile, CI on GitHub Actions (tests against real MySQL + build), versioned migrations with Flyway, and CSRF/CORS configured.
- Unit test coverage (JUnit 5 + Mockito) across every service layer, plus integration tests (MockMvc) validating authentication and access control.

**[API Bank](https://github.com/umdevaprendiz/financialbank)** — a banking simulation REST API
`Java` `Spring Boot` `Spring Security` `Docker` `Railway`

Evolving from a banking simulation into a financial platform with a social layer — personal finance tracking combined with a social layer built around goals, not showing off spending.

- **Own profile:** every user has a profile, like a social network, but with posts about financial milestones — an emergency fund built up, a debt paid off, a savings goal hit — instead of everyday photos.
- **Feed and connections:** the ability to follow other people and see those milestones in a feed, creating a social incentive to stay on top of your finances.
- **Spending analysis engine:** transaction categorization, a spending limit per category, and calculating how much is still available to spend this month and how much was actually saved in the period.
- **Reused technical foundation:** the current data model (accounts, transactions, user roles) would be extended to support profiles, posts, followers, and goals, keeping the same authentication and role-based authorization already in place.

---

### Education & languages

Computer Science — UFPB *(expected graduation: 2030)* · Networking Technician — ETEMERB
Portuguese (native) · English (B2) · Spanish (basic/intermediate)
