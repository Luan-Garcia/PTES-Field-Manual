# Google Hacking (Dorks) Cheatsheet

> **Concept:** Advanced search operators to uncover sensitive data exposed by misconfigured servers.
> **Warning:** Excessive automated searching may trigger CAPTCHAs or temporary IP bans from Google.

<div align="center">
  <a href="#-english-version">🇺🇸 English Version</a> | 
  <a href="#-versão-em-português">🇧🇷 Versão em Português</a>
</div>

---

## 🇺🇸 English Version

### 1. Finding Exposed Files & Secrets
Targeting files that should not be public.

| Description | Dork Command |
| :--- | :--- |
| **Config Files** | `site:target.com ext:xml OR ext:conf OR ext:cnf OR ext:reg OR ext:inf OR ext:rdp OR ext:cfg OR ext:txt OR ext:ora OR ext:ini` |
| **Database Files** | `site:target.com ext:sql OR ext:dbf OR ext:mdb` |
| **Log Files** | `site:target.com ext:log` |
| **Backup Files** | `site:target.com ext:bkf OR ext:bkp OR ext:bak OR ext:old OR ext:backup` |
| **Sensitive Docs** | `site:target.com ext:doc OR ext:docx OR ext:odt OR ext:pdf OR ext:rtf OR ext:sxw OR ext:psw OR ext:ppt OR ext:pptx OR ext:pps OR ext:csv` |
| **Env Variables** | `site:target.com intext:"DB_PASSWORD" OR intext:"API_KEY"` |

### 2. Login Portals & Admin Panels
Finding entry points for employees.

| Description | Dork Command |
| :--- | :--- |
| **Admin Portals** | `site:target.com inurl:admin OR inurl:login OR inurl:adminlogin OR inurl:cpanel OR inurl:manager` |
| **Intranet/VPN** | `site:target.com inurl:intranet OR inurl:vpn OR inurl:portal` |
| **Jira/Trello** | `site:trello.com "target_name" OR site:jira.com "target_name"` |
| **S3 Buckets** | `site:s3.amazonaws.com "target_name"` |

### 3. Directory Listing
Finding servers that allow browsing files like a folder.

```text
site:target.com intitle:"index of"
```

---

## 🇧🇷 Versão em Português

### 1. Arquivos Expostos e Segredos
Focando em arquivos que não deveriam ser públicos.

| Descrição | Comando Dork |
| :--- | :--- |
| **Arquivos de Config** | `site:alvo.com ext:xml OR ext:conf OR ext:cnf OR ext:reg OR ext:inf OR ext:rdp OR ext:cfg OR ext:txt OR ext:ora OR ext:ini` |
| **Banco de Dados** | `site:alvo.com ext:sql OR ext:dbf OR ext:mdb` |
| **Arquivos de Log** | `site:alvo.com ext:log` |
| **Backups** | `site:alvo.com ext:bkf OR ext:bkp OR ext:bak OR ext:old OR ext:backup` |
| **Docs Sensíveis** | `site:alvo.com ext:doc OR ext:docx OR ext:odt OR ext:pdf OR ext:rtf OR ext:sxw OR ext:psw OR ext:ppt OR ext:pptx OR ext:pps OR ext:csv` |
| **Variáveis de Ambiente** | `site:alvo.com intext:"DB_PASSWORD" OR intext:"API_KEY"` |

### 2. Portais de Login e Admin
Encontrando pontos de entrada para funcionários.

| Descrição | Comando Dork |
| :--- | :--- |
| **Portais Admin** | `site:alvo.com inurl:admin OR inurl:login OR inurl:adminlogin OR inurl:cpanel OR inurl:manager` |
| **Intranet/VPN** | `site:alvo.com inurl:intranet OR inurl:vpn OR inurl:portal` |
| **Jira/Trello** | `site:trello.com "nome_alvo" OR site:jira.com "nome_alvo"` |
| **Buckets S3** | `site:s3.amazonaws.com "nome_alvo"` |

### 3. Listagem de Diretórios (Directory Listing)
Encontrando servidores que permitem navegar nos arquivos como pastas.

```text
site:alvo.com intitle:"index of"
```
