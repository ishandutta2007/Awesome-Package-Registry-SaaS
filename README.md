# Awesome-Package-Registry-SaaS

## Top Package Registry SaaS Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Private Package Hosting, Artifact Repositories, Multi-Format Registries & Secure Software Distribution*

**Last updated: September 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Package Registries / Artifact Repositories**. These systems host, proxy, cache, and distribute private packages and binaries across formats such as npm, Maven, PyPI, NuGet, Docker/OCI, Go, Helm, RubyGems, and more.



**Examples** include Cloudsmith, GitHub Packages, GitLab Package Registry, AWS CodeArtifact, Azure Artifacts, Packagecloud, ProGet, Bytesafe, CloudRepo, and Gemfury (the category leaders).



**Open-source emphasis**: Package registry tooling has strong open options. **Harbor**, **Verdaccio**, **Nexus Repository OSS**, **Pulp**, and emerging multi-format projects provide production-ready self-hosted alternatives. This section is heavily expanded with these tools.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-products)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms

| Product | Description | Pricing | Free Tier Limits |
| :--- | :--- | :--- | :--- |
| **[Cloudsmith](https://cloudsmith.com/)** | Cloud-native, fully managed multi-format package registry focused on secure distribution, upstream proxying, and enterprise features across many ecosystems. | Core Plan: Free<br>Pro Plan: Starts at $149/month | Core Plan: 500 MB storage, 1 GB/month download bandwidth |
| **[GitHub Packages](https://github.com/features/packages)** | Integrated package registry tightly coupled with GitHub repositories and Actions, supporting npm, Maven, NuGet, Docker, RubyGems, and more. | Free for public packages<br>GitHub Pro: $4/user/month<br>GitHub Team: $4/user/month | GitHub Free (Private): 500 MB storage, 1 GB/month data transfer |
| **[GitLab Package Registry](https://docs.gitlab.com/ee/user/packages/)** | Built-in package and container registry within GitLab, supporting multiple formats and seamless CI/CD integration. | Free Tier: $0/user/month<br>GitLab Premium: $29/user/month | Free Tier: 10 GiB storage limit per project (up to 5 users/namespace) |
| **[AWS CodeArtifact](https://aws.amazon.com/codeartifact/)** | Fully managed artifact repository service compatible with npm, Maven, PyPI, NuGet, and other popular package managers, with upstream proxying. | Pay-as-you-go:<br>$0.05 per GB-month storage<br>$0.05 per 10,000 requests | AWS Free Tier: 2 GB storage, 100,000 requests per month |
| **[Azure Artifacts](https://azure.microsoft.com/en-us/products/devops/artifacts)** | Azure DevOps package management service supporting NuGet, npm, Maven, Python, and Universal Packages with feed views and upstream sources. | First 2 GiB free<br>Next 2–10 GiB: $2/GiB/month | 2 GiB free storage per organization |
| **[Packagecloud](https://packagecloud.io/)** | Hosted package repository service supporting multiple formats with simple distribution and access control. | Free Plan: $0<br>Starter Plan: Starts at $89/month | Free Plan: 2 GB storage, 10 GB/month bandwidth (public repositories) |
| **[ProGet](https://inedo.com/proget)** | Package and container management platform (self-hosted and cloud options) with vulnerability scanning, feeds, and broad format support. | Free Edition: $0<br>Basic Plan: Starts at $2,395/year | Free Edition: Unlimited feeds & users (limited to 10 API deletes/hour) |
| **[Bytesafe](https://bytesafe.dev/)** | Security-focused package management and supply-chain platform for private registries and dependency protection. | Cloud Plan: Starts at €99/month | 14-day free trial (Full feature access, no credit card required) |
| **[CloudRepo](https://cloudrepo.com/)** | Managed private Maven and Python package repositories with straightforward hosting and access controls. | Starter Plan: Starts at $199/month | 14-day free trial (No credit card required) |
| **[Gemfury](https://gemfury.com/)** | Private cloud package repository supporting multiple language ecosystems with simple push and install workflows. | Personal Plan: Starts at $9/month | Public Plan: Free for unlimited public packages |



## Open-Source GitHub Projects

- **[Harbor](https://github.com/goharbor/harbor)**  

  CNCF open-source cloud-native registry that stores, signs, and scans container images and Helm charts, with replication, RBAC, and vulnerability scanning.



- **[Verdaccio](https://github.com/verdaccio/verdaccio)**  

  Lightweight, popular open-source private npm proxy registry — easy to self-host, cache public packages, and publish private modules.



- **[Nexus Repository OSS](https://github.com/sonatype/nexus-public)**  

  Open-source edition of Sonatype Nexus Repository supporting multiple formats (Maven, npm, Docker, PyPI, NuGet, and more) with hosted, proxy, and group repositories.



- **[Pulp](https://github.com/pulp)**  

  Flexible open-source content and package management platform with plugins for RPM, Debian, Python, npm, containers, Maven, and other formats; strong at proactive syncing.



- **[kkRepo](https://github.com/klboke/kkRepo)**  

  Community-driven, Nexus-compatible open-source artifact repository supporting a wide range of formats (Maven, npm, PyPI, Go, Helm, Docker, Cargo, NuGet, etc.) with migration support.



- **[Gitea / Forgejo Package Registry](https://github.com/go-gitea/gitea)**  

  Built-in package registry features in the open-source Git forges, supporting multiple package types alongside Git hosting.



- **[BaGet](https://github.com/loic-sharma/BaGet)**  

  Open-source NuGet server implementation for hosting private .NET packages.



- **[devpi](https://github.com/devpi/devpi)**  

  Powerful open-source PyPI-compatible server and caching proxy for Python packages.



- **[Athens](https://github.com/gomods/athens)**  

  Open-source Go module proxy and registry for private and cached public modules.



- **[Artifact Keeper and similar full-featured open registries](https://github.com/)**  

  Emerging self-hosted multi-format artifact repositories aiming for broad protocol support and enterprise features without feature gates.



### Additional Strong Open-Source Options

- Using **Harbor** as the standard for container and Helm registries with security scanning.

- Deploying **Verdaccio** for lightweight private npm needs or CI caching.

- Choosing **Nexus OSS** or **Pulp** for multi-format artifact management in self-hosted environments.

- Leveraging **Gitea/Forgejo** packages when you already run an open-source Git forge.

- Combining format-specific open registries (BaGet, devpi, Athens) for targeted language ecosystems.

- Accepting that fully managed multi-tenant SaaS convenience, global CDN distribution, advanced supply-chain security features, and enterprise SLAs still favor commercial platforms (Cloudsmith, CodeArtifact, Azure Artifacts, GitHub Packages, etc.).



**Frameworks for building custom systems**: Deploy Harbor (containers) + Verdaccio/Nexus/Pulp (language packages) → configure upstream proxies and private hosted repos → integrate with CI/CD for publish and consume → apply RBAC and vulnerability scanning → mirror or replicate as needed. This stack is fully open and production-proven. Commercial SaaS registries remain the practical choice when teams want zero-ops managed hosting, broad format support out of the box, and integrated security/compliance features.



## How to Contribute

1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.

- Package registries are critical to software supply-chain security. Misconfigured access controls, unsigned packages, or unpatched vulnerabilities can introduce serious risk. Self-hosted open-source solutions require proper authentication, authorization, backup, monitoring, and update practices. Always follow organizational security and compliance policies. This list is not security or compliance advice.



---

**Made for DevOps, platform, and engineering teams who need reliable private package distribution.**

Let's keep artifact management secure, performant, and as open as practical.
