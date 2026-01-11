# Business Intelligence / Inteligência de Negócio

> **Goal:** Expand the scope horizontally. Find subsidiaries, acquisitions, and netblocks owned by the target.
> **Golden Rule:** "A chain is only as strong as its weakest link (usually a recently acquired subsidiary)."

<div align="center">
  <a href="#-english-version">🇺🇸 English Version</a> | 
  <a href="#-versão-em-português">🇧🇷 Versão em Português</a>
</div>

---

## 🇺🇸 English Version

### Overview
Before scanning a single IP, you must understand **who** you are attacking. Large corporations are not monolithic; they are a web of acquisitions, partners, and forgotten assets. 

This phase is about **Horizontal Reconnaissance**: Instead of going deep into one domain, we go wide to find *all* domains and IP ranges owned by the organization.

### Workflow: Scope Expansion

```mermaid
graph TD
    A[Target: Main Brand] --> B{Discovery Phase}
    B --> C[Acquisitions & Subsidiaries]
    B --> D[ASN & IP Ranges]
    B --> E[Reverse Whois]
    
    C --> F[New Domains (Scope +)]
    D --> G[Shadow IT / Dev Servers]
    E --> H[Marketing/Campaign Sites]
    
    style F fill:#d4edda,stroke:#28a745
    style G fill:#d4edda,stroke:#28a745
    style H fill:#d4edda,stroke:#28a745
```

### Key Objectives
1.  **Identify Subsidiaries:** Companies bought by the target often have weaker security policies but trusted network connections (VPNs) to the main HQ.
2.  **Map IP Ranges (ASN):** Find servers that do not have a domain name associated (Direct IP access).
3.  **Uncover Shadow IT:** Find cloud tenants and domains registered by developers using corporate emails but outside standard IT governance.

---

## 🇧🇷 Versão em Português

### Visão Geral
Antes de escanear um único IP, você deve entender **quem** está atacando. Grandes corporações não são monolíticas; elas são uma teia de aquisições, parceiros e ativos esquecidos.

Esta fase é sobre **Reconhecimento Horizontal**: Em vez de se aprofundar em um domínio, vamos ampliar para encontrar *todos* os domínios e faixas de IP pertencentes à organização.

### Fluxo de Trabalho: Expansão de Escopo

```mermaid
graph TD
    A[Alvo: Marca Principal] --> B{Fase de Descoberta}
    B --> C[Aquisições e Subsidiárias]
    B --> D[ASN e Faixas de IP]
    B --> E[Whois Reverso]
    
    C --> F[Novos Domínios (Escopo +)]
    D --> G[Shadow IT / Servidores Dev]
    E --> H[Sites de Marketing/Campanha]
    
    style F fill:#d4edda,stroke:#28a745
    style G fill:#d4edda,stroke:#28a745
    style H fill:#d4edda,stroke:#28a745
```

### Objetivos Chave
1.  **Identificar Subsidiárias:** Empresas compradas pelo alvo geralmente têm políticas de segurança mais fracas, mas conexões de rede confiáveis (VPNs) para a matriz.
2.  **Mapear Faixas de IP (ASN):** Encontrar servidores que não possuem um nome de domínio associado (Acesso direto via IP).
3.  **Descobrir Shadow IT:** Encontrar tenants de nuvem e domínios registrados por desenvolvedores usando e-mails corporativos, mas fora da governança padrão de TI.
