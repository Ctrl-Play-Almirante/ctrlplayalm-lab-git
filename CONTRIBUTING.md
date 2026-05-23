# 🤝 Guia de Contribuição — Ctrl+Play

Olá! Seja muito bem-vindo(a) ao seu primeiro passo no mundo open source! 🎉

Este guia foi feito para quem **nunca contribuiu** em um projeto no GitHub antes. Vamos juntos, passo a passo!

---

## 📋 Pré-requisitos

Antes de começar, você precisa ter instalado na sua máquina:

- [Git](https://git-scm.com/downloads)
- Uma conta no [GitHub](https://github.com)
- Um editor de código (recomendamo o [VS Code](https://code.visualstudio.com/))

---

## 🔢 Passo a Passo

### Passo 1 — Faça um Fork

> O **fork** cria uma cópia deste repositório na sua conta do GitHub.

1. No topo desta página, clique no botão **Fork**
2. Clique em **Create fork**
3. Pronto! Agora você tem uma cópia do projeto na sua conta 🎊

---

### Passo 2 — Clone o repositório

> **Clonar** significa baixar o projeto para a sua máquina.

No seu fork (na **sua** conta do GitHub), clique no botão verde **Code** e copie a URL.

Depois, abra o terminal e digite:

```bash
git clone https://github.com/SEU-USUARIO/ctrlplay-lab-opensource.git
```

> ⚠️ Substitua `SEU-USUARIO` pelo seu nome de usuário do GitHub!

Entre na pasta do projeto:

```bash
cd ctrlplay-lab-opensource
```

---

### Passo 3 — Crie uma Branch

> A **branch** é como um "rascunho" isolado para a sua contribuição, sem afetar o projeto principal.

```bash
git checkout -b feat/community/seu-usuario
```

> ⚠️ Substitua `seu-usuario` pelo seu nome de usuário do GitHub!

---

### Passo 4 — Crie o seu arquivo de perfil

Dentro da pasta `community/`, crie um arquivo com o nome do seu usuário do GitHub.

**Exemplo:** `community/maria-silva.md`

Use o modelo abaixo como base:

```markdown
# Olá, eu sou [Seu Nome]! 👋

## Sobre mim
- 🎮 Aluno(a) da Ctrl+Play Young
- 💻 Aprendendo: Git e GitHub
- 🌟 Hobbies: Escutar, música, desenhar...
- 🚀 Estou na Ctrl+Play porque: Quero aprender Python para fazer sites
- Eu 💙 : comida

## Conecte-se comigo
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github)](https://github.com/seu-usuario)

```
---

### Passo 5 — Salve as alterações (Commit)

Após criar seu arquivo, volte ao terminal e execute:

```bash
# Adiciona o arquivo à área de preparo
git add community/seu-usuario.md

# Salva as alterações com uma mensagem descritiva
git commit -m "feat: add seu-usuario profile"
```

---

### Passo 6 — Envie para o GitHub (Push)

```bash
git push origin feat/community/seu-usuario
```

---

### Passo 7 — Abra um Pull Request

1. Acesse o seu fork no GitHub
2. Clique no botão **Compare & pull request** (ele vai aparecer automaticamente)
3. Preencha o título e a descrição
4. Clique em **Create pull request**
5. **Parabéns!** 🎉 Você acabou de abrir o seu primeiro Pull Request!

---

## ✅ Checklist antes de enviar

Antes de abrir o Pull Request, verifique:

- [ ] Meu arquivo está dentro da pasta `community/`
- [ ] O nome do arquivo é meu usuário do GitHub (ex: `maria-silva.md`)
- [ ] Não mexi em nenhum outro arquivo do projeto
- [ ] Minha mensagem de commit começa com `feat:`

---

## ❓ Dúvidas?

Se travar em algum passo, chama a professora ou abre uma [Issue](../../issues) descrevendo sua dúvida. Você não está sozinho(a) 💙

---

<div align="center">
  Feito com 💙 por <strong>Caroline Teixeira</strong>
</div>
