# Comando `mkdir` no Linux

O comando `mkdir` (**make directory**) é utilizado para **criar diretórios** no Linux. Ele permite a criação de um ou vários diretórios ao mesmo tempo e oferece opções para configurar permissões e estruturas hierárquicas.

---

## Sintaxe
```bash
mkdir [opções] [nome_do_diretório]
```
- `[nome_do_diretório]` → Nome do diretório a ser criado.
- `[opções]` → Parâmetros opcionais para modificar o comportamento do comando.

---

## Exemplos de uso

### 1. **Criar um único diretório**
```bash
mkdir projeto
```
Cria um diretório chamado `projeto` no diretório atual.

### 2. **Criar múltiplos diretórios ao mesmo tempo**
```bash
mkdir pasta1 pasta2 pasta3
```
Cria três diretórios (`pasta1`, `pasta2` e `pasta3`) dentro do diretório atual.

### 3. **Criar um diretório dentro de outro diretório inexistente**
```bash
mkdir -p documentos/trabalho
```
Cria os diretórios `documentos` e `trabalho`, caso não existam. A opção `-p` permite a criação de diretórios pai que ainda não existem.

### 4. **Definir permissões ao criar um diretório**
```bash
mkdir -m 755 public
```
Cria o diretório `public` com permissões `755` (leitura e execução para todos, escrita apenas para o dono).

---

## Opções comuns

| Opção  | Descrição                                                |
|--------|----------------------------------------------------------|
| `-p`   | Cria diretórios pai, se ainda não existirem.             |
| `-m`   | Define permissões para o diretório criado.               |
| `-v`   | Exibe mensagens detalhadas sobre a criação dos diretórios. |

---

## Dicas
- Para garantir que os diretórios sejam criados sem erro, combine `mkdir -p` com estruturas complexas.
- Utilize `ls -l` para verificar se o diretório foi criado corretamente e conferir suas permissões.

Agora você já sabe como criar diretórios de maneira eficiente no Linux! 🚀