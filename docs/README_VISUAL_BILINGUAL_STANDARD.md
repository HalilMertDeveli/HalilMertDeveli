# README Visual Bilingual Standard

A reusable standard for README files in Halil Mert Develi's repositories.
Every README is written for two readers at once: a recruiter or hiring manager who scans for 60 seconds, and a senior engineer who reads for 10 minutes. Both languages, English and Turkish, live in the same file.

---

## 1. Principles

| # | Principle | In practice |
|---|---|---|
| 1 | **Verified, not claimed** | Every feature, version and diagram node is traceable to a file in the repo. If it is not in the code, it is not in the README. |
| 2 | **Honest maturity** | Status and limitations are stated up front. A learning project is called a learning project. |
| 3 | **Scannable first, deep second** | Hero + quick facts answer "what is this" in 10 seconds. Architecture and engineering notes reward a longer read. |
| 4 | **Bilingual by design** | English and Turkish are both first-class and written natively, not machine-translated line by line. |
| 5 | **Quiet visuals** | Tables, one diagram, real screenshots. No emoji rows, no decorative GIFs, no badge walls. |
| 6 | **Safe** | No secrets, real connection strings, personal phone numbers, customer data or internal hostnames. |

## 2. Project tiers

| Tier | When | Length | Required sections |
|---|---|---|---|
| **A — Flagship** | Product-grade or portfolio-defining projects | Long | Hero, quick facts, overview, problem & solution, features, stack, architecture (Mermaid), repo structure, data & auth, setup, run, testing & CI, screenshots, engineering notes, limitations, status |
| **B — Solid** | Working medium-size apps | Medium | Hero, quick facts, overview, features, stack, structure, run, limitations, status |
| **C — Learning** | Courses, tutorials, experiments, unfinished starts | Short | Hero, quick facts, overview, learning goals / topics, stack, structure, run, limitations, attribution |

Do not inflate a Tier C project. A clean, honest Tier C README is a positive signal; an over-sold one is a negative signal.

**Skip, do not rewrite:** unmodified copies of third-party projects (for example an imported upstream sample). Their upstream README is the correct documentation.

## 3. Bilingual layout

Never solve bilingual support with a link to another file or "Türkçe için tıkla".

### Layout A — paired sections (default for Tier B and C)

Each `##` heading carries both languages. English paragraph first, Turkish paragraph directly below, introduced by a bold `TR` label. Tables use bilingual column headers instead of being duplicated.

```markdown
## Overview · Genel Bakış

A role-based work-order manager for small teams ...

**TR —** Küçük ekipler için rol tabanlı bir iş emri yönetim uygulaması ...

| Feature · Özellik | Description · Açıklama |
|---|---|
| Role-based areas · Rol tabanlı alanlar | Admin and Member MVC areas · Admin ve Üye MVC alanları |
```

### Layout B — mirrored halves (default for Tier A)

A small language bar under the hero links to two in-page anchors. The English half comes first, the Turkish half mirrors its structure exactly (same headings, same tables, same diagram labels where practical). Shared assets (badges, quick facts, screenshots) can appear once and be referenced.

```markdown
<p align="center"><a href="#english">English</a> · <a href="#turkce">Türkçe</a></p>

<a id="english"></a>
## Overview
...
<a id="turkce"></a>
## Genel Bakış
...
```

Use explicit `<a id="...">` anchors (ASCII ids) rather than relying on GitHub's generated anchors for headings with Turkish characters.

### Layout C — collapsible Turkish

Only for very long READMEs where Layout B would exceed comfortable length: put the Turkish half inside `<details><summary><b>Türkçe</b></summary> ... </details>`. Leave a blank line after `<summary>` so Markdown renders inside.

### Turkish writing rules

- Use natural technical Turkish. Keep established English terms where Turkish engineers use them: *endpoint, middleware, repository, migration, commit, pipeline, idempotency*.
- Use correct Turkish characters (ç, ğ, ı, İ, ö, ş, ü). Never ASCII-fold Turkish prose.
- Formal, neutral register ("uygulama ... sağlar", "projeyi çalıştırmak için"). Avoid "biz"/marketing tone.
- Translate meaning, not word order. The Turkish section may be slightly shorter but must not drop facts, limitations or warnings.

## 4. Visual system

### Hero

```html
<div align="center">

# Project Name

**One-line summary in English.**
<br/>
<sub>Türkçe tek satırlık özet.</sub>

<!-- 3–6 meaningful badges -->

</div>
```

### Badges

- Use `https://img.shields.io/badge/<label>-<message>-<color>?style=flat-square&logo=<logo>&logoColor=white`.
- Allowed: runtime/framework version, database, main platform, CI (only if a workflow exists), license (only if a LICENSE file exists), status.
- Maximum six. No "made with love", no visitor counters, no star counters, no fake coverage.
- Status badge vocabulary: `active`, `completed`, `prototype`, `learning project`, `archived-style / no longer maintained`, `unfinished`.

### Quick facts table

| | |
|---|---|
| **Type · Tür** | Web application · Web uygulaması |
| **Status · Durum** | Completed academic project · Tamamlanmış akademik proje |
| **Stack · Teknoloji** | .NET 8, ASP.NET Core MVC, EF Core, SQL Server |
| **Category · Kategori** | Portfolio / Learning / Prototype |

### Feature matrix

Prefer a table (`Area · Alan | Capability · Yetenek | Where · Konum`) over long bullet walls once there are more than ~6 features. The `Where` column (a folder or file path) is a strong credibility signal for senior reviewers.

### Callouts

GitHub alert syntax is allowed, sparingly (at most two per README):

```markdown
> [!NOTE]
> Learning project based on a course. Code follows the course structure.

> [!WARNING]
> Not production-ready: no automated tests, secrets must be supplied locally.
```

### Repository structure block

A trimmed `text` tree of the important folders only, each with a short comment. Never paste a full `tree` dump.

## 5. Diagrams (Mermaid)

- Only draw what the code proves: projects/modules from project references, services from `Program.cs`/DI, external systems from config and client code.
- Never invent microservices, queues, caches, Kubernetes or cloud components.
- One architecture diagram is usually enough. Add a sequence diagram only for a genuinely interesting flow (auth, payment, realtime).
- Syntax safety: quote node labels that contain spaces, parentheses, slashes or dots: `API["ASP.NET Core API (.NET 8)"]`. Use `<br/>` for line breaks inside labels. Avoid `end` as a bare node id. Keep `flowchart LR` or `TD`.
- Diagram labels stay in English in both halves (they are technical identifiers); the caption is bilingual.

## 6. Screenshots

- Use only images already in the repository (or produced from a locally run app with seed/demo data).
- Never fabricate, mock up or AI-generate screenshots.
- Strip or avoid personal data, real customer names, phone numbers, emails, tokens.
- Store under `docs/images/` (or the repo's existing folder) and reference with relative paths.
- Present as a table grid (2 columns) with a bilingual caption under each: `Admin dashboard · Yönetici paneli`.
- If no screenshots exist and the app cannot be run reliably, omit the section rather than leaving placeholders.

## 7. Setup and run instructions

- Prerequisites with versions read from project files (`TargetFramework`, `pubspec.yaml` SDK constraint, `package.json` engines, Gradle config).
- Commands in fenced blocks with the right language tag (`bash`, `powershell`).
- Configuration through placeholders (`<your-connection-string>`, `.env.example`), never real values.
- If a command was not actually run, do not claim it was verified. Write "Expected commands" when unverified.
- Mention required external services (database, Firebase project, API keys) and that the reader must provide their own.

## 8. Audience rules

**Recruiters / hiring managers** read: hero, quick facts, overview, features, screenshots, status.
Write these so a non-specialist understands *what it does and for whom* without jargon.

**Senior engineers / interviewers** read: architecture, structure, data & auth, engineering notes, testing, limitations.
Write these with concrete identifiers (class names, folders, patterns, versions) and explicit trade-offs.

## 9. Honesty and limitations

Every README has a **Limitations · Sınırlamalar** section. Typical honest items:

- No automated tests / no CI.
- Not deployed; runs locally only.
- Secrets or external accounts required.
- Partially implemented features (name them).
- Course or tutorial origin, code not fully original (credit the source).
- Outdated framework versions.

Forbidden: invented user counts, uptime, performance numbers, "production-ready", "enterprise-grade", "scalable to millions", coverage percentages that were not measured.

## 10. Security checklist (before every commit)

- [ ] No API keys, tokens, passwords, connection strings with credentials.
- [ ] No private phone numbers or personal emails beyond what the owner already publishes publicly.
- [ ] No internal IPs, hostnames, admin URLs of live systems.
- [ ] Screenshots contain no real customer data.
- [ ] If a secret is noticed in the repository itself, do not reproduce it; report it to the owner separately.

## 11. Validation checklist (before every PR)

- [ ] Every internal `#anchor` link resolves.
- [ ] Every relative image/file link exists in the branch.
- [ ] External links are reachable (or removed).
- [ ] Mermaid blocks follow the syntax-safety rules above.
- [ ] Both languages contain the same facts, status and limitations.
- [ ] Every technical claim is traceable to code.

## 12. Git workflow

- Branch: `docs/visual-bilingual-readme` from the default branch.
- Commit: `docs: rewrite README with visual bilingual technical documentation`.
- PR title: `docs: rewrite README with visual bilingual technical documentation`.
- PR body: what changed, what was verified, what could not be verified.
- Never push to the default branch, never auto-merge.

## 13. Quality score (out of 100)

| Dimension | Points |
|---|---|
| Technical accuracy | 30 |
| Clarity | 20 |
| Visual quality | 15 |
| Bilingual quality | 15 |
| Setup / documentation completeness | 10 |
| Recruiter usefulness | 5 |
| Senior engineer usefulness | 5 |
