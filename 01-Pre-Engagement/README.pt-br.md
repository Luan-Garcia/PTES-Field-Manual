# 1. Interações Pré-Engajamento (Pre-engagement)

## 📝 Definição
Esta é a fase de planejamento. Antes de qualquer pacote ser enviado, as regras do jogo devem ser estabelecidas. O objetivo é definir o escopo, limites legais e expectativas do teste para evitar problemas jurídicos e interrupções de serviço.

**Lembre-se:** A diferença entre um pentest e um crime cibernético é a **permissão**. Nunca pule esta etapa.

## ✅ Checklist de Escopo
- [ ] **Definição do Alvo:** lista precisa de faixas de IP, domínios e subdomínios.
- [ ] **Exclusões:** Sistemas que estritamente *não podem* ser tocados (ex: servidores de produção legados, dispositivos médicos, sistemas de terceiros/SaaS sem permissão).
- [ ] **Regras de Engajamento (RoE):**
    - Tipos de ataque permitidos (Engenharia Social? Físico? Negação de Serviço/DoS?).
    - Janela de teste (24/7 ou apenas horário comercial/noturno?).
    - Canais de comunicação (Contato de emergência caso um servidor caia).
- [ ] **Legal:** Autorização formal assinada (Carta de permissão).

## 🛠️ Perguntas Chave para o Cliente
1. **Tipo de Teste:** Será Blackbox (sem info), Greybox (usuário comum) ou Whitebox (código fonte/admin)?
2. **Ambiente:** Testaremos em Produção (Real) ou Staging (Homologação)?
3. **Riscos:** Existe algum sistema crítico que, se cair, causa prejuízo financeiro imediato?
4. **Reporte:** Como vulnerabilidades críticas (RCE/SQLi) devem ser reportadas? (Imediatamente ou no relatório final?)

## 📂 Arquivos nesta pasta
* `Scope_Worksheet.md`: Modelo para definir o escopo técnico.
* `Rules_of_Engagement.md`: Template das regras de conduta do teste.
* `Authorization_Letter.md`: Modelo de carta de autorização formal.
