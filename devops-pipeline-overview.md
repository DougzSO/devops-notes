# Conceitos Fundamentais de CI/CD e DevOps

## ✅ O que é CI/CD?

**CI (Continuous Integration)**  
Integração contínua de código. Cada vez que um desenvolvedor envia código novo (commit), o sistema:
- Verifica formatação e lint (ex: com Git Hooks)
- Faz build automático do projeto
- Executa testes unitários e de integração
- Gera **feedback rápido** sobre o que quebrou

**CD (Continuous Delivery/Deployment)**  
Entrega contínua do código aprovado para ambientes de **staging ou produção**, podendo ser:
- **Delivery**: requer aprovação manual para ir para produção.
- **Deployment**: vai direto para produção, sem intervenção humana.

## 🔁 Fluxo da Pipeline CI/CD

```
1. Code > 
2. Lint / Format > 
3. Commit (Git) > 
4. Build (Docker, NPM, etc.) > 
5. Test (Unit/Integration) > 
6. Deploy (Staging/Prod) > 
7. Monitor (Logs, Errors) 
```

## 🔧 Ferramentas Comuns em Cada Etapa

| Etapa         | Ferramentas comuns                                |
|---------------|----------------------------------------------------|
| **Planejar**  | JIRA, Trello, Confluence                          |
| **Codar**     | Git, GitHub, GitLab, Bitbucket, AWS CodeCommit   |
| **Buildar**   | Docker, Gradle, NPM                               |
| **Testar**    | Mocha, Selenium, Cucumber                         |
| **Deployar**  | Jenkins, GitHub Actions, AWS CodeDeploy          |
| **Operar**    | Kubernetes, AWS ECS, Amazon EKS                  |
| **Monitorar** | Datadog, Splunk, Amazon CloudWatch               |

## 🛠️ Jenkins – Visão Geral

- **Ferramenta CI/CD open source**
- Escrito em Java, mas roda qualquer linguagem
- Suporta:
  - Scripts shell
  - Webhooks de GitHub/GitLab
  - Plugins para Docker, Slack, AWS, etc.
- Pipeline configurada por arquivo `Jenkinsfile` (em Groovy)

## 🧠 Agile vs Waterfall

**Waterfall (Modelo Cascata)**  
Processo sequencial, antigo:  
1. Requisitos > 2. Análise > 3. Design > 4. Construção > 5. Validação > 6. Entrega

**Agile (Ágil)**  
Iterativo e incremental:
- Sprints semanais ou diários
- Feedback constante
- Melhor adaptação às mudanças

## 📌 Resumo Final

- CI/CD = automatização total da integração, testes e deploy
- Jenkins = ferramenta central no DevOps
- Agilidade e automação trazem **velocidade, qualidade e controle**
- Ideal para equipes que querem fazer deploy com frequência

---

## 🔁 Como Revisar e Não Esquecer

1. Leia o resumo hoje e tente explicar para si mesmo
2. Releia no Dia 1 e 3
3. Dia 7: veja outro conteúdo (vídeo) sobre CI/CD e compare
4. Dia 15: tente criar um mini projeto com CI/CD
