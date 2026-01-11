# OpSec & Anonymity (How not to get burned)

> **Concept:** Operational Security (OpSec) prevents the target from knowing they are being investigated.
> **Rule:** Never do OSINT from your personal accounts or raw IP address.

<div align="center">
  <a href="#-english-version">🇺🇸 English Version</a> | 
  <a href="#-versão-em-português">🇧🇷 Versão em Português</a>
</div>

---

## 🇺🇸 English Version

### 1. The "Sock Puppet" (Fake Accounts)
You cannot view LinkedIn, Instagram, or Facebook profiles anonymously. You need a fake persona.

* **Identity:** Create a realistic persona. Give them a name, a fake AI-generated face ([ThisPersonDoesNotExist](https://thispersondoesnotexist.com)), and a job title (e.g., "Recruiter" or "Freelancer").
* **Aging:** Do not create an account and start spying immediately. Platforms ban new accounts that act aggressively. create it weeks in advance.
* **Isolation:** Use a dedicated browser container (e.g., Firefox Multi-Account Containers) or a separate Virtual Machine for these accounts. Never log in to your personal email in the same session.

### 2. Network Anonymity
* **VPN is minimum:** Never use your home IP.
* **Tor Browser:** Use for sensitive searches or when accessing onion sites, but be aware that Tor exit nodes are often blocked by Google/Cloudflare.
* **User-Agent Rotation:** Automated tools often use default headers (e.g., `python-requests/2.0`). Change your User-Agent to look like a standard Chrome browser on Windows.

### 3. Browser Fingerprinting
Sites track more than just cookies; they track your screen resolution, fonts, and battery level.
* **Tool:** Test your browser at [Cover Your Tracks](https://coveryourtracks.eff.org/).
* **Mitigation:** Use privacy-focused browsers like **LibreWolf** or **Brave**.

---

## 🇧🇷 Versão em Português

### 1. O "Sock Puppet" (Contas Falsas)
Você não consegue ver perfis no LinkedIn, Instagram ou Facebook anonimamente. Você precisa de uma persona falsa.

* **Identidade:** Crie uma persona realista. Dê um nome, uma foto gerada por IA ([ThisPersonDoesNotExist](https://thispersondoesnotexist.com)) e um cargo (ex: "Recrutador" ou "Consultor").
* **Envelhecimento (Aging):** Não crie a conta e comece a espiar imediatamente. As plataformas banem contas novas com comportamento agressivo. Crie semanas antes.
* **Isolamento:** Use containers no navegador (ex: Firefox Multi-Account Containers) ou uma Máquina Virtual separada. Nunca logue no seu e-mail pessoal na mesma sessão.

### 2. Anonimato de Rede
* **VPN é o mínimo:** Nunca use o IP da sua casa.
* **Tor Browser:** Use para buscas sensíveis, mas saiba que muitos nós de saída do Tor são bloqueados por Google e Cloudflare.
* **Rotação de User-Agent:** Ferramentas automatizadas usam cabeçalhos padrão (ex: `python-requests/2.0`). Mude seu User-Agent para parecer um navegador Chrome comum.

### 3. Fingerprinting do Navegador
Sites rastreiam mais que apenas cookies; eles rastreiam sua resolução de tela, fontes instaladas e bateria.
* **Ferramenta:** Teste seu navegador no [Cover Your Tracks](https://coveryourtracks.eff.org/).
* **Mitigação:** Use navegadores focados em privacidade como **LibreWolf** ou **Brave**.
