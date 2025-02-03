# Gerenciamento de Permissões no Linux

O sistema de permissões do Linux é fundamental para garantir a segurança e o controle de acesso a arquivos e diretórios. Este guia cobre os conceitos básicos, como modificar permissões e alterar a propriedade de arquivos e diretórios.

## 📌 Como Funcionam as Permissões no Linux
Cada arquivo e diretório no Linux possui três tipos de permissões:

- **Leitura (r - read)**: Permite visualizar o conteúdo do arquivo.
- **Escrita (w - write)**: Permite modificar ou excluir o arquivo.
- **Execução (x - execute)**: Permite executar o arquivo (caso seja um programa ou script).

As permissões são definidas para três categorias de usuários:

1. **Usuário (owner)**: O dono do arquivo.
2. **Grupo (group)**: Um grupo de usuários que pode ter permissões específicas.
3. **Outros (others)**: Todos os demais usuários do sistema.

Exemplo de listagem de permissões com `ls -l`:
```bash
ls -l arquivo.txt
-rw-r--r-- 1 usuario grupo 1234 Jan 1 12:34 arquivo.txt
```

Explicação:
- `-rw-r--r--` → Representa as permissões.
- `1` → Número de links.
- `usuario` → Dono do arquivo.
- `grupo` → Grupo ao qual o arquivo pertence.
- `1234` → Tamanho do arquivo em bytes.
- `Jan 1 12:34` → Data e hora da última modificação.
- `arquivo.txt` → Nome do arquivo.

## 🔧 Como Alterar Permissões
As permissões podem ser alteradas usando o comando `chmod`.

### Utilizando Notação Simbólica
A notação simbólica usa letras para definir permissões:
```bash
chmod u+x arquivo.sh  # Adiciona permissão de execução para o dono
chmod g-w arquivo.txt # Remove permissão de escrita do grupo
chmod o+r arquivo.txt # Adiciona permissão de leitura para outros
chmod ugo=r arquivo.txt # Define permissões exatas para todos
```

### Utilizando Notação Octal
A notação octal representa permissões em números:
- `4` → Leitura (r)
- `2` → Escrita (w)
- `1` → Execução (x)

Cada conjunto de permissões é somado e representado por três números:
```bash
chmod 755 script.sh  # Permissões: rwxr-xr-x
chmod 644 arquivo.txt # Permissões: rw-r--r--
```

## 🔄 Alterando o Dono e Grupo de Arquivos
### Alterar o Dono do Arquivo
O comando `chown` permite alterar o dono de um arquivo:
```bash
sudo chown novo_usuario arquivo.txt
```

### Alterar o Grupo do Arquivo
Para alterar apenas o grupo:
```bash
sudo chown :novo_grupo arquivo.txt
```

### Alterar o Dono e o Grupo ao Mesmo Tempo
```bash
sudo chown novo_usuario:novo_grupo arquivo.txt
```

### Aplicar Mudanças Recursivamente em Diretórios
Para alterar permissões ou donos em todos os arquivos de um diretório:
```bash
sudo chmod -R 755 /caminho/do/diretorio
sudo chown -R usuario:grupo /caminho/do/diretorio
```

---
Este guia cobre os fundamentos do gerenciamento de permissões no Linux. Para mais informações, consulte os manuais:
```bash
man chmod
man chown
man ls
```