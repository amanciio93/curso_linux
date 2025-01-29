# Comando `rmdir` no Linux

O comando `rmdir` (**remove directory**) é usado para **remover diretórios vazios** no Linux. Ele é uma alternativa ao comando `rm -d`, mas possui a limitação de apenas funcionar com diretórios que não contenham arquivos ou subdiretórios.

---

## Sintaxe
```bash
rmdir [opções] [nome_do_diretório]
```
- `[nome_do_diretório]` → Diretório vazio que será removido.
- `[opções]` → Parâmetros opcionais para modificar o comportamento do comando.

---

## Exemplos de uso

### 1. **Remover um diretório vazio**
```bash
rmdir pasta_vazia
```
Remove o diretório `pasta_vazia`, desde que esteja vazio.

### 2. **Remover múltiplos diretórios vazios**
```bash
rmdir dir1 dir2 dir3
```
Remove os diretórios `dir1`, `dir2` e `dir3`, caso todos estejam vazios.

### 3. **Remover diretórios vazios aninhados**
```bash
rmdir -p pasta1/pasta2/pasta3
```
Remove a estrutura de diretórios `pasta3`, `pasta2` e `pasta1`, desde que todos estejam vazios. A opção `-p` remove os diretórios pais de forma recursiva.

---

## Opções comuns

| Opção  | Descrição                                                     |
|--------|---------------------------------------------------------------|
| `-p`   | Remove diretórios pais vazios junto com o diretório especificado. |
| `--ignore-fail-on-non-empty` | Ignora falhas caso o diretório não esteja vazio (não remove o conteúdo). |

---

## Dicas
- Caso o diretório contenha arquivos ou subdiretórios, utilize o comando `rm -r` para removê-lo com todo o conteúdo.
- Use `rmdir` quando quiser garantir que apenas diretórios vazios sejam excluídos.
- Combine com `ls` para verificar se o diretório está realmente vazio antes de tentar removê-lo.

Com o comando `rmdir`, é possível remover diretórios vazios de maneira simples e direta! 🚀