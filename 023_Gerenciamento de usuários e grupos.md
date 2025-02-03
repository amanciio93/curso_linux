# Gerenciamento de Usuários e Grupos no Linux

O gerenciamento de usuários e grupos no Linux é essencial para controle de acesso e segurança do sistema. Este guia apresenta os principais comandos para criar, deletar e gerenciar usuários e grupos.

## 📌 Criar Usuários
Para criar um novo usuário, utilize o comando `useradd`:
```bash
sudo useradd nome_do_usuario
```
Criar um usuário e definir a senha:
```bash
sudo useradd -m nome_do_usuario
sudo passwd nome_do_usuario
```
Explicação:
- `-m`: Cria um diretório home automaticamente.
- `passwd`: Define uma senha para o usuário.

Criar um usuário com um shell específico:
```bash
sudo useradd -m -s /bin/bash nome_do_usuario
```

Criar um usuário e atribuir a um grupo específico:
```bash
sudo useradd -m -G grupo nome_do_usuario
```

## 🗑️ Deletar Usuários
Para remover um usuário:
```bash
sudo userdel nome_do_usuario
```
Para remover um usuário e seu diretório home:
```bash
sudo userdel -r nome_do_usuario
```

## 👥 Criar e Deletar Grupos
Criar um grupo:
```bash
sudo groupadd nome_do_grupo
```

Adicionar um usuário a um grupo:
```bash
sudo usermod -aG nome_do_grupo nome_do_usuario
```

Remover um usuário de um grupo:
```bash
sudo gpasswd -d nome_do_usuario nome_do_grupo
```

Remover um grupo:
```bash
sudo groupdel nome_do_grupo
```

## 🔄 Alterar Nome do Usuário e Diretório Home
Para mudar o nome de um usuário:
```bash
sudo usermod -l novo_nome antigo_nome
```

Para mudar o diretório home do usuário:
```bash
sudo usermod -d /novo/caminho/home -m nome_do_usuario
```
Explicação:
- `-l`: Muda o nome do usuário.
- `-d`: Define um novo diretório home.
- `-m`: Move os arquivos do diretório antigo para o novo.

## 🚫 Desabilitar/Habilitar Usuários
Para desabilitar um usuário (impedir login):
```bash
sudo usermod -L nome_do_usuario
```

Para habilitar um usuário novamente:
```bash
sudo usermod -U nome_do_usuario
```

Para expirar uma conta imediatamente:
```bash
sudo passwd -l nome_do_usuario
```

Para desbloquear a conta:
```bash
sudo passwd -u nome_do_usuario
```

---
Este guia fornece os comandos essenciais para gerenciar usuários e grupos no Linux. Para mais detalhes, consulte:
```bash
man useradd
man userdel
man usermod
man groupadd
```