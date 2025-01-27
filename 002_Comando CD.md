# Comando `cd` no Linux

O comando `cd` é usado para **navegar entre diretórios** no terminal. Ele significa **"change directory"** (mudar de diretório). Com ele, você pode se deslocar para diferentes pastas no sistema de arquivos.

---

## Sintaxe básica
```bash
cd [caminho_do_diretório]
```
- `[caminho_do_diretório]` pode ser um caminho absoluto ou relativo.

---

## Caminho absoluto
Um caminho absoluto começa a partir da raiz do sistema (`/`).

### Exemplo:
```bash
cd /home/jonathan/Documents
```
Isso move você diretamente para o diretório `/home/jonathan/Documents`, independentemente de onde você esteja.

---

## Caminho relativo
Um caminho relativo considera o diretório onde você está no momento.

### Exemplo:
Se você está em `/home/jonathan` e digita:
```bash
cd Documents
```
O terminal leva você para `/home/jonathan/Documents`.

---

## Casos especiais do comando `cd`

### 1. **Voltar ao diretório home:**
```bash
cd
```
ou
```bash
cd ~
```
Leva você ao diretório pessoal do seu usuário, por exemplo, `/home/jonathan`.

### 2. **Subir um nível no diretório (diretório pai):**
```bash
cd ..
```
Se você está em `/home/jonathan/Documents`, esse comando o levará para `/home/jonathan`.

### 3. **Voltar ao diretório anterior:**
```bash
cd -
```
Este comando alterna entre o diretório atual e o último acessado.

---

## Dicas úteis
```bash
cd /etc && ls
```
- Combinar o comando cd com outros comandos usando '&&' é possível.

- Para verificar o diretório em que você está atualmente, use o comando `pwd` (print working directory).
- Utilize a tecla **Tab** para completar automaticamente nomes de diretórios ao digitar no terminal.

Agora você está pronto para navegar pelo sistema de arquivos do Linux com o comando `cd`! 😊

