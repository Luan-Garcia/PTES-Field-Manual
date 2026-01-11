# Data Analysis & Pivoting / Análise e Pivoteamento

> **Concept:** Data is useless without action. This guide maps "Findings" to "Attack Vectors".
> **Context:** Before starting active scanning or exploitation, use this checklist to plan your attack path.

<div align="center">
  <a href="#-english-version">🇺🇸 English Version</a> | 
  <a href="#-versão-em-português">🇧🇷 Versão em Português</a>
</div>

---

## 🇺🇸 English Version

### 1. From Finding to Vector
What to do with the specific data you collected?

| If you found... | Your Next Step (The Vector) |
| :--- | :--- |
| **Email List** (`john.doe@target.com`) | **Password Spraying:** Try one password (`Summer2024!`) against all users. <br> **Phishing:** Create a targeted campaign. <br> **Credential Hunting:** Check *DeHashed/HaveIBeenPwned* for old passwords. |
| **Documents** (PDF, DOCX) | **Metadata Analysis:** Extract "Author" names for usernames. Extract software versions (e.g., "PDF created by VulnerableLib v1.0"). |
| **Cloud Buckets** (S3, Azure Blob) | **Content Inspection:** Download everything. Look for `.env` files, backups, and database dumps. <br> **Write Test:** Check if you can upload files (Malware hosting). |
| **Subdomains** (`dev.`, `stg.`) | **Tech Stack Analysis:** These often run debug mode or have no WAF. Look for verbose error messages. |
| **Source Code** (GitHub Leaks) | **Secret Scanning:** Grep for `api_key`, `access_token`, `jdbc`. <br> **Logic Review:** Read the code to find hidden API endpoints not documented. |
| **Employee Photos** (Badges/Desk) | **Physical/Social:** Clone the ID badge layout. Read sticky notes on monitors in the background (passwords are often there). |

### 2. The "Pivot" Logic
How to connect two unrelated pieces of information.

* **Email + LinkedIn Job Post:**
    * *Info:* Job post says "We use Jenkins and Jira".
    * *Info:* Email is `j.smith`.
    * *Pivot:* Try logging into Jenkins/Jira portals (found via Google Dorks) with `j.smith`.
* **Subdomain + Tech Stack:**
    * *Info:* `blog.target.com` runs WordPress 4.2.
    * *Info:* Main site `target.com` is secure.
    * *Pivot:* Exploit the old WordPress on the subdomain to get a shell, then pivot laterally to the main network.

### 3. Preparation for Phase 2 (Scanning)
Filter your target list before loading it into Nessus/Nmap.
* **Ignore:** CDN IPs (Cloudflare/Akamai). You cannot scan them.
* **Prioritize:** IPs with "Self-Signed Certificates" (usually internal/forgotten infrastructure).

---

## 🇧🇷 Versão em Português

### 1. Do Dado ao Vetor de Ataque
O que fazer com o dado específico que você coletou?

| Se você encontrou... | Seu Próximo Passo (O Vetor) |
| :--- | :--- |
| **Lista de E-mails** (`joao.silva@alvo.com`) | **Password Spraying:** Tentar uma senha fraca (`Empresa2024!`) contra todos os usuários. <br> **Phishing:** Criar campanha direcionada. <br> **Caça de Credenciais:** Verificar *DeHashed* por senhas vazadas antigas. |
| **Documentos** (PDF, DOCX) | **Análise de Metadados:** Extrair nomes de "Autor" para gerar usuários. Extrair versões de software (ex: "PDF criado por LibVulneravel v1.0"). |
| **Buckets de Cloud** (S3, Azure) | **Inspeção de Conteúdo:** Baixar tudo. Buscar por arquivos `.env`, backups e dumps de banco. <br> **Teste de Escrita:** Verificar se você pode upar arquivos (Hospedagem de malware). |
| **Subdomínios** (`dev.`, `homolog.`) | **Análise de Stack:** Geralmente rodam em modo debug ou sem WAF. Procure por mensagens de erro detalhadas. |
| **Código Fonte** (Vazamento GitHub) | **Scan de Segredos:** Buscar por `api_key`, `access_token`, `db_password`. <br> **Review de Lógica:** Ler o código para achar endpoints de API ocultos. |
| **Fotos de Funcionários** (Crachás/Mesa) | **Físico/Social:** Clonar o layout do crachá. Ler post-its nos monitores ao fundo (senhas frequentemente estão lá). |

### 2. A Lógica de "Pivoteamento"
Como conectar duas peças de informação não relacionadas.

* **E-mail + Vaga no LinkedIn:**
    * *Info:* Vaga diz "Usamos Jenkins e Jira".
    * *Info:* E-mail é `j.silva`.
    * *Pivô:* Tentar logar nos portais Jenkins/Jira (achados via Google Dorks) com o usuário `j.silva`.
* **Subdomínio + Tecnologia:**
    * *Info:* `blog.alvo.com` roda WordPress 4.2 (Antigo).
    * *Info:* Site principal `alvo.com` é seguro.
    * *Pivô:* Explorar o WordPress antigo no subdomínio para pegar uma shell, e depois pivotar lateralmente para a rede principal.

### 3. Preparação para Fase 2 (Scanning)
Filtre sua lista de alvos antes de colocar no Nessus/Nmap.
* **Ignorar:** IPs de CDN (Cloudflare/Akamai). Você não pode escaneá-los.
* **Priorizar:** IPs com "Certificados Auto-assinados" (geralmente infraestrutura interna ou esquecida).
