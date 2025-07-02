# 🧱 Fundamentos de Git – Conceitos Básicos para Controle de Versão

Este documento apresenta os fundamentos essenciais do **Git**, um sistema de controle de versão distribuído amplamente utilizado no desenvolvimento de software profissional e em projetos open-source.

---

## 📦 O que é Git?

- **Git** é um sistema de controle de versão distribuído criado por Linus Torvalds.
- Permite que múltiplas pessoas trabalhem no mesmo projeto sem sobrescrever as mudanças uns dos outros.
- Todas as alterações no código são **rastreadas**, podendo ser **revertidas**, **comparadas** ou **mescladas**.

---

## 📂 Conceitos Fundamentais

### ✅ Commit
- É o "salvamento" de alterações no histórico do repositório.
- Cada commit representa um **snapshot** (fotografia) do código naquele momento.
- Comando: `git commit -m "mensagem"`

### 🌿 Branch
- Linha separada de desenvolvimento.
- Permite que você trabalhe em features isoladas sem afetar o código principal.
- Comando: `git branch nome-da-branch`

### 🔁 Merge
- Une as alterações de uma branch em outra (geralmente na `main` ou `develop`).
- Comando: `git merge nome-da-branch`

### 🎯 Rebase
- Move uma branch para o final de outra, reescrevendo o histórico.
- Muito útil para manter o histórico linear.
- Comando: `git rebase nome-da-base`

### 🍒 Cherry-pick
- Aplica um commit específico de outra branch na sua branch atual.
- Comando: `git cherry-pick <hash-do-commit>`

---

## 📄 Ciclo Básico de Trabalho com Git

```bash
# Clonar um repositório remoto
git clone https://github.com/usuario/repositorio.git

# Verificar status do repositório local
git status

# Adicionar arquivo ao stage (preparar para commit)
git add arquivo.txt

# Commitar as alterações
git commit -m "Adiciona novo recurso"

# Enviar alterações para o repositório remoto
git push origin nome-da-branch

# Puxar alterações do remoto para local
git pull origin nome-da-branch
```

---

## 🔧 Outras Ações Comuns

- **Criar branch**: `git checkout -b nova-feature`
- **Mudar de branch**: `git checkout nome-da-branch`
- **Listar branches**: `git branch`
- **Ver log de commits**: `git log --oneline --graph`
- **Desfazer último commit (sem perder mudanças)**: `git reset --soft HEAD~1`

---

## 🧠 Boas Práticas

- Commits pequenos e frequentes
- Mensagens de commit claras e no imperativo (ex: "Adiciona botão de login")
- Usar branches para cada feature ou correção
- Atualizar a branch com `git pull` antes de fazer `push`
- Revisar mudanças com `git diff` antes de commitar

---

## 📚 Recursos para Prática

- Simuladores: [https://learngitbranching.js.org](https://learngitbranching.js.org)
- Livro recomendado: *Pro Git* – [https://git-scm.com/book/en/v2](https://git-scm.com/book/en/v2)
- Cheatsheet oficial: [https://education.github.com/git-cheat-sheet-education.pdf](https://education.github.com/git-cheat-sheet-education.pdf)

---

**Douglas Silva de Oliveira** — Desenvolvedor e Explorador de Ferramentas DevOps ⚙️🚀
