# Planilha de Definição de Escopo

> Este documento define as fronteiras técnicas do trabalho. Por favor, liste todos os ativos a serem testados.

## 1. Informações do Alvo

### A. Aplicações Web / URLs
| Nome da Aplicação | URL | Ambiente (Prod/Homolog) | Precisa de Login? (Admin/User) |
| :--- | :--- | :--- | :--- |
| ex: Portal Principal | https://portal.empresa.com.br | Homologação | Sim, 2 perfis |
| | | | |

### B. Faixas de IP / Rede
| Descrição | Endereço IP / CIDR | Provedor (AWS/Azure/Local) |
| :--- | :--- | :--- |
| ex: VPN Gateway | 200.100.x.x | Local |
| | | |

## 2. Exclusões (Não Atacar)
*Liste qualquer IP ou subdomínio específico que estritamente NÃO pode ser testado.*
1. __________________________
2. __________________________

## 3. Restrições Técnicas
* **WAF/IPS:** Existe firewall ativo? (Sim/Não)
    * *Se Sim, devemos colocar o IP do Pentester na Whitelist?* (Sim/Não)
* **Cloud:** Precisamos notificar o provedor de Cloud? (Sim/Não)

## 4. Objetivos (Flags)
Qual o objetivo principal?
- [ ] Encontrar o maior número possível de vulnerabilidades.
- [ ] Provar acesso a um banco de dados específico (Dados sensíveis).
- [ ] Testar a capacidade de detecção do Blue Team.
