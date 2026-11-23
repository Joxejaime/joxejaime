# Hi, I'm Jaime 👋

**DevOps / Cloud engineer.** I build delivery pipelines, AWS infrastructure and recovery tooling, and I write down exactly what has been run and what hasn't. 3 years of freelance DevOps and cloud consulting (part-time), and co-founder and technical lead of **Juega App**, a product I built and operate on AWS. Based in Managua, Nicaragua · open to remote roles across Latin America.

## Currently: Juega App

A free iOS, Android and web app for organizing pickup football: sign-ups, balanced teams, ratings and stats. I own development and operations; my partner owns marketing and sales. It is **live on AWS in a closed test with real users**, on infrastructure I created and configured myself. The source is private because the app is headed to the App Store and Google Play; the architecture, decisions and measurements are public in the portfolio.

- **Infrastructure as code:** Terraform for the VPC, server, registry, buckets, alarms, budget and cost monitor; no drift between the code and AWS.
- **Keyless delivery:** every push is tested, scanned and deployed by GitHub Actions through OIDC and SSM, with no stored cloud keys and no SSH.
- **Operations:** SLOs, runbooks, game days, an uptime check and alarms, and a nightly backup that is restored into a scratch database and verified before it is uploaded.
- **Measured over 7 days on AWS (to 2026-11-23):** 100% uptime from 16 locations, 0 host failures, 1.7% average CPU, a verified backup every night, and about $14 a month.
- **Tests in CI:** 309 API and 185 mobile tests, plus hadolint, gitleaks and a Trivy image gate on every change.

## DevOps & Cloud portfolio

**[devops-portfolio →](https://github.com/Joxejaime/devops-portfolio)**: eight components in three projects, each with tests, diagrams and its own CI pipeline. The latest run of every pipeline passes, and every page lists what is proven and what is not.

| Project | What it shows |
|---|---|
| **Delivery platform** | A pipeline that refuses to ship a vulnerable image (Trivy, SBOM, cosign), AWS infrastructure in Terraform deployed with no stored cloud keys (GitHub OIDC, applied for real in Juega App), GitOps promotion by pull request, and error-budget SLO alerting with runbooks |
| **Reliability and recovery** | An LLM gateway that keeps serving through a provider outage, an SRE lab that turns SLOs into alert rules and rehearses failure, and a disaster-recovery autopilot that restores PostgreSQL from verified snapshots |
| **Developer platform** | `platformctl`: one command scaffolds a production-shaped service that already passes every policy guardrail |

## Stack

`AWS` · `Terraform` · `GitHub Actions` · `Docker` · `Kubernetes` · `Argo CD` · `Prometheus` · `Grafana` · `PostgreSQL` · `Python` · `TypeScript`

## Honest status

Proven and running: the Juega App deployment on AWS, its CI and keyless deploy, its alarms and verified backups, and CI on all eight portfolio components. **Not yet proven:** an Argo CD sync on a live cluster, a production environment for Juega App (written, not applied), request-level numbers from real users, and a public store release. The portfolio README lists the rest.

The work is built with Claude Code under my review and control: I decide what is built, review every change, run and debug it, and own the security decisions.

## Looking for

Remote **DevOps, Cloud / AWS, Platform or Infrastructure engineering, and SRE** roles across Latin America.

## Contact

[LinkedIn](https://www.linkedin.com/in/jaime-castillo-araujo) · [castilloajosejaime@gmail.com](mailto:castilloajosejaime@gmail.com)
