# ⚙️ Configurando o Git — Ctrl+Play

> 💡 Siga a seção correspondente à sua situação!

---

## 🏫 Em Sala de Aula (PC compartilhado)

### 1. Instalação

1. Acesse [https://git-scm.com/downloads](https://git-scm.com/downloads) e baixe o instalador
2. Execute e clique **Next** em todas as etapas
3. Ao final, abra o **Git Bash**

### 2. No início de cada aula

Antes de começar, sempre rode estes três comandos com os seus dados:

```bash
git config --global user.name "meu-usuario"
git config --global user.email "meu-email@gmail.com"
git config --global credential.helper ""
```

> ⚠️ Se pular esse passo, o commit pode sair no nome do colega que usou o PC antes de você!

### 3. Gerando o Token

O GitHub não aceita mais senha comum. Você precisa de um **Token**:

1. Acesse o GitHub → clique na sua foto → **Settings**
2. **Developer settings → Personal access tokens → Tokens (classic)**
3. Clique em **Generate new token (classic)**
4. Dê um nome, defina a validade e marque a permissão **repo**
5. Clique em **Generate token** e **copie o token** (ele só aparece uma vez!)

### 4. Na hora do Push 

```bash
git push -u origin main
# Username: meu-usuario
# Password: cole-seu-token-aqui
```
Em caso de clone de repositório: siga o passo-a-passo aqui: [CONTRIBUTING.md](CONTRIBUTING.md)


---

## 🏠 Em Casa (SSH)

### 1. Instalação

**Windows:** Acesse [https://git-scm.com/downloads](https://git-scm.com/downloads), instale e abra o **Git Bash**

**Linux (Ubuntu/Debian):**
```bash
sudo apt update
sudo apt install git -y
```

### 2. Configuração Global

```bash
git config --global user.name "meu-usuario"
git config --global user.email "meu-email@gmail.com"
```

### 3. Gerando a Chave SSH

```bash
ssh-keygen -t ed25519 -C "seu-email@gmail.com"
```

Pressione **Enter** em todas as perguntas.

### 4. Adicionando a Chave no GitHub

Copie a chave pública:

```bash
cat ~/.ssh/id_ed25519.pub
```

O terminal vai exibir uma linha longa, por exemplo:

```
ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAI... seu-email@gmail.com
```

Copie todo esse conteúdo, depois:

1. Acesse o GitHub → **Settings → SSH and GPG keys**
2. Clique em **New SSH key**
3. Dê um nome (ex: `meu-notebook`) e cole a chave
4. Clique em **Add SSH key**

### 5. Testando a Conexão

```bash
ssh -T git@github.com
```

Se aparecer `Hi meu-usuario!`, está tudo certo! ✅

### 6. Clonando e Enviando

Com SSH configurado, clone assim:

```bash
git clone git@github.com:SEU-USUARIO/ctrlplayalm-lab-git.git
```

E o `git push` **não pedirá senha nem token**. 🎉

---
