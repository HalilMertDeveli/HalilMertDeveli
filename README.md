<h1 align="center">Halil Mert Develi</h1>

<p align="center">
  <strong>.NET Backend &amp; Full-Stack Software Engineer</strong><br />
  Flutter &amp; cross-platform mobile · Istanbul, Türkiye
</p>

<p align="center">
  <a href="https://halilmertdeveli.com.tr"><img src="https://img.shields.io/badge/Portfolio-halilmertdeveli.com.tr-111?style=flat-square" alt="Portfolio" /></a>
  <a href="https://www.linkedin.com/in/halil-mert-develi-00983a225/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:halilmertdeveliii@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
</p>

---

## About me

I'm a Computer Engineer who builds backend systems with **C# and ASP.NET Core**, and cross-platform mobile apps with **Flutter**.

Most of my work happens in the LED display industry: support tooling, B2B commerce and service-management platforms, where the hard part is modelling a messy domain correctly. I care about layered architecture, explicit domain models, tests that run against real databases, and APIs that are boring to consume.

## Core engineering skills

- **Backend & APIs** — ASP.NET Core, REST, Razor Pages / MVC, EF Core, authentication and role-based authorization
- **Architecture** — Clean / Onion / layered architecture, domain modelling, idempotent operations, ports and adapters
- **Data** — PostgreSQL, SQL Server, Cloud Firestore, Supabase, migrations and integration tests on real databases
- **Mobile** — Flutter and Dart for Android and iOS, Firebase, some native Android with Kotlin and Jetpack Compose
- **Web front end** — Next.js, React, TypeScript
- **Delivery** — Docker, GitHub Actions CI, Vercel container deployments
- **Integrations** — payment providers, email, WhatsApp and LLM APIs with validation and failure handling

## Technology stack

<p>
  <img src="https://skillicons.dev/icons?i=cs,dotnet,postgres,flutter,dart,nextjs,react,ts,firebase,supabase,docker,githubactions&theme=dark" alt="C#, .NET, PostgreSQL, Flutter, Dart, Next.js, React, TypeScript, Firebase, Supabase, Docker, GitHub Actions" />
</p>

## Featured projects

### Open source

| Project | What it is | Stack |
| --- | --- | --- |
| [**LEDCare OS**](https://github.com/HalilMertDeveli/LEDCare-OS) | Service-management platform for LED screen technical support: a web app, a mobile app and an API, with CI that runs backend tests on real PostgreSQL, web E2E tests and an Android build. In development. | ASP.NET Core · EF Core · PostgreSQL · SignalR · Next.js · React · Flutter |
| [**ASP.NET-APP-FOR-LED**](https://github.com/HalilMertDeveli/ASP.NET-APP-FOR-LED) | Live support website for Colorlight, NovaStar and Huidu LED control systems: request form, Google sign-in, realtime customer chat and an admin panel. [Live site](https://asp-net-app-for-led.vercel.app) | ASP.NET Core 8 · Razor Pages · Supabase · Resend · Vercel |
| [**TaskManagementSystem**](https://github.com/HalilMertDeveli/TaskManagementSystem) | My Computer Engineering capstone: a task manager with Admin and Member roles, built with Onion architecture. | ASP.NET Core MVC · MediatR · FluentValidation · EF Core · SQL Server |
| [**yazilim-sitesi**](https://github.com/HalilMertDeveli/yazilim-sitesi) | My portfolio site, with small playable demos of my products and a printable recruiter brief. [Live site](https://halilmertdeveli.com.tr) | ASP.NET Core 8 · Razor Pages · vanilla JS · Docker |

### Private product work

The source of these lives in private repositories. You can try small demos of the first four on [my portfolio](https://halilmertdeveli.com.tr).

| Project | What it is | Stack | Status |
| --- | --- | --- | --- |
| **Mevora** | Dating app that shows why two people match and keeps exact location private; matching, safety rules and moderation run on the server. | Flutter · Firebase · Cloud Functions (TypeScript) | Pre-launch |
| **LED B2B Platform** | Managed B2B platform that turns an LED screen request into a configured, priced order, with suppliers and costs hidden from the customer. | .NET 10 · ASP.NET Core · EF Core · PostgreSQL | Not publicly available |
| **Motor** | E-commerce site for a motorcycle parts business, with parts searched by make, model and year. | .NET 10 · ASP.NET Core · EF Core · PostgreSQL · Docker | Demo stage |
| **LED Support Bot** | WhatsApp intake system that collects a technician's diagnostic details, then hands the conversation to a human. | .NET 8 · ASP.NET Core · PostgreSQL · Node.js | In testing |
| **ClearPay** | Demo digital wallet on a double-entry ledger, with web and Flutter clients. | .NET 8 · SQL Server · Hangfire · Flutter | Demo |

## Engineering highlights

- **Tests against real infrastructure.** The LED B2B Platform's suite runs locally against PostgreSQL (last recorded run: 2,691 passed). [LEDCare OS](https://github.com/HalilMertDeveli/LEDCare-OS) runs backend tests on real PostgreSQL, contract and web E2E tests, mobile analysis and an Android build in GitHub Actions.
- **Money handled carefully.** ClearPay derives balances from a double-entry ledger instead of updating them, and transfers are idempotent: a replayed request returns `409`.
- **Pricing safety through types.** In the LED B2B Platform, supplier cost, platform margin and customer price are separate value objects, so cost and sale price can't be mixed up.
- **Trust moved to the server.** Mevora computes matches, applies safety rules and validates purchases in Cloud Functions rather than on the client.
- **Deterministic first, AI second.** The LED Support Bot parses sizes, counts and IDs with plain code; an LLM is only called behind a cost gate, with a strict JSON schema and validation.

## GitHub activity

<p>
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://streak-stats.demolab.com/?user=HalilMertDeveli&theme=github-dark-blue&hide_border=true&border_radius=8" />
    <img src="https://streak-stats.demolab.com/?user=HalilMertDeveli&theme=default&hide_border=true&border_radius=8" alt="GitHub contribution streak for HalilMertDeveli" />
  </picture>
</p>

## Portfolio & contact

- **Portfolio** — [halilmertdeveli.com.tr](https://halilmertdeveli.com.tr)
- **LinkedIn** — [halil-mert-develi](https://www.linkedin.com/in/halil-mert-develi-00983a225/)
- **Email** — [halilmertdeveliii@gmail.com](mailto:halilmertdeveliii@gmail.com)

Open to conversations about .NET backend, full-stack and Flutter roles.
