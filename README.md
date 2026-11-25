## Mason W. Foley

QA leader who builds his own tools with AI coding agents. 15+ years in QA, 12+ managing QA teams.

Portfolio and write-ups: **[masonfoley.me](https://masonfoley.me)**

### Sprint Intelligence
A multi-layered scoring algorithm that assessed whether a sprint was on track to release on time. Built for the QA team I managed, it read raw Jira, Xray and Bitbucket data (test coverage, test-plan pacing, defect arrival rate, time in status) and rolled 24 weighted scoring rules up to a green-to-red status. Every report then had to pass 62 validation rules that checked its arithmetic before anyone saw it.

TypeScript, Node.js, PostgreSQL, Next.js

### Release calendar
Designed from the requirements to replace Monday.com for leadership release reviews: calendar, roadmap table, Gantt view, presentation mode, role-based access and an audit trail. Built in about five weeks (68 merged pull requests), then hardened after a security assessment. The deployed app cleared a Tenable web application scan with no critical, high or medium findings.

TypeScript, Docker, CI on every pull request, Netlify

### masonfoley.me
My personal site. Its build runs Playwright and axe checks and publishes the results on the site.

Astro, Playwright, axe, Netlify

### SellStack
A web app for selling household items online. It tracks each item from the moment it's picked to sell until the sale closes, on eBay and other marketplaces. The Claude API helps write listing text, and a barcode scan looks up the product. Every flow starts as a sequence diagram, and its tests are written from that diagram. The MVP is nearly done.

TypeScript, Next.js, React, Supabase, Claude API, Netlify; Vitest, Playwright, axe, Stryker mutation testing

### D.A.R.E. Ministries volunteer site
The public site and volunteer portal for D.A.R.E. Ministries, an Atlanta faith-based disaster recovery charity I deploy with: **[whofixedtheroof.com](https://whofixedtheroof.com)**. Volunteers register and sign up for trips by the day, and coordinators approve accounts, manage trip rosters, publish stories from the field, email the volunteer list and review photos members upload. A scheduled health check watches the site and its TLS certificate.

Eleventy, Nunjucks, Netlify Functions, Netlify Database (Postgres), Netlify Identity, Resend; Vitest, GitHub Actions

### How I build
Claude Code is the main agent and Codex works on its own branches, under written rules both read every session. GitNexus indexes each repo into a code knowledge graph, so the agent checks the blast radius of a change before it edits and runs change detection on the graph before it commits. Every change is a pull request reviewed by CodeRabbit AI and two custom skills: one turns the PR's sequence diagram into adversarial tests, the other works every review comment. 454 merged PRs and roughly 5,600 automated tests across my projects.

The repos are private. Code available for review on request.
