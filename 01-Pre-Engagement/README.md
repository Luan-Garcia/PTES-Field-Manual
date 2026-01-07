# 1. Pre-engagement Interactions

## 📝 Definition
This is the planning phase. Before any packet is sent, the rules of the game must be established. The goal is to define the scope, legal boundaries, and expectations of the test to avoid legal issues and service disruptions.

## ✅ Scoping Checklist
- [ ] **Target Definition:** precise IP ranges, domains, and subdomains.
- [ ] **Exclusions:** Systems that strictly *cannot* be touched (e.g., legacy production servers, third-party medical devices).
- [ ] **Rules of Engagement (RoE):**
    - Allowed attack types (Social Engineering? Physical? DoS?).
    - Testing window (24/7 or specific hours?).
    - Communication channels (Emergency contact if a server goes down).
- [ ] **Legal:** Signed authorization (Get Out of Jail Free card).

## 🛠️ Key Questions to Ask
1. Is this a Blackbox, Greybox, or Whitebox test?
2. Are we testing in Production or Staging environments?
3. How should critical vulnerabilities be reported immediately?
