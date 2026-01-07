# Regras de Engajamento (Rules of Engagement - RoE)

**Cliente:** [Nome da Empresa]
**Consultor/Pentester:** [Seu Nome]
**Data:** [DD/MM/AAAA]

---

## 1. Janela de Testes
Definição dos horários permitidos para a execução dos testes.

- [ ] **24/7:** Testes permitidos a qualquer horário.
- [ ] **Horário Comercial:** Apenas das 09:00 às 18:00 (Seg-Sex).
- [ ] **Fora do Horário Comercial:** Apenas após às 19:00 ou finais de semana.
- [ ] **Outro:** ________________________

## 2. Técnicas de Exploração
O que é permitido e o que é estritamente proibido durante o teste.

| Técnica | Permitido? | Observações |
| :--- | :---: | :--- |
| **Exploração Ativa** | SIM / NÃO | Rodar exploits que podem travar serviços. |
| **Engenharia Social** | SIM / NÃO | Phishing, Vishing, SMS. |
| **Acesso Físico** | SIM / NÃO | Tentar entrar no escritório/sala de servidores. |
| **DoS / Stress Test** | SIM / NÃO | Negação de Serviço (Derrubar o site). |
| **Bypass de WAF/IPS** | SIM / NÃO | Tentar evasão de firewall. |
| **Exfiltração de Dados** | SIM / NÃO | Retirar dados reais (PII) para prova de conceito. |

## 3. Comunicação e Emergência
Caso um serviço crítico caia ou uma invasão seja detectada pelo Blue Team.

* **Ponto de Contato Principal (Cliente):**
    * Nome: __________________
    * Telefone (24h): __________________
    * Email: __________________

* **Ponto de Contato (Pentester):**
    * Nome: [Seu Nome]
    * Telefone: [Seu Telefone]

## 4. Manipulação de Evidências
* Screenshots de dados sensíveis devem ser anonimizados no relatório final? (Sim/Não)
* Dados extraídos (dump de banco) devem ser deletados imediatamente após a confirmação? (Sim/Não)

## 5. Limpeza (Post-Engagement)
O consultor compromete-se a remover:
* Shells/Backdoors instalados.
* Usuários criados para teste.
* Arquivos temporários ou scripts de teste.

---
**Assinaturas:**

__________________________
[Nome do Responsável - Cliente]

__________________________
[Seu Nome - Pentester]
