# Comando `grep` no UNIX

O comando `grep` é utilizado para buscar padrões dentro de arquivos de texto no UNIX e sistemas baseados em Linux. Ele é amplamente utilizado para filtrar e localizar informações específicas em arquivos.

## Sintaxe

```sh
grep [OPÇÕES] PADRÃO [ARQUIVO]
```

Se nenhum arquivo for especificado, o `grep` lê da entrada padrão.

## Exemplos de Uso

### 1. Buscar uma palavra específica em um arquivo
```sh
grep "erro" arquivo.log
```
Isso exibirá todas as linhas do arquivo `arquivo.log` que contêm a palavra "erro".

### 2. Buscar de forma insensível a maiúsculas e minúsculas
```sh
grep -i "aviso" arquivo.log
```
Isso encontrará ocorrências da palavra "aviso" independentemente de letras maiúsculas ou minúsculas.

### 3. Buscar um padrão em múltiplos arquivos
```sh
grep "falha" *.log
```
Isso procurará a palavra "falha" em todos os arquivos com extensão `.log` no diretório atual.

### 4. Exibir o número da linha das correspondências
```sh
grep -n "sucesso" arquivo.txt
```
Isso mostrará cada linha que contém "sucesso" junto com o número da linha correspondente.

### 5. Exibir apenas as correspondências exatas
```sh
grep -o "[0-9]\{4\}" arquivo.txt
```
Isso exibirá todas as sequências de exatamente quatro dígitos encontradas no arquivo.

### 6. Inverter a busca (exibir linhas que **não** contêm o padrão)
```sh
grep -v "erro" arquivo.log
```
Isso exibirá todas as linhas do arquivo que **não** contêm a palavra "erro".

### 7. Buscar recursivamente em diretórios
```sh
grep -r "token" /var/log
```
Isso procurará a palavra "token" em todos os arquivos dentro do diretório `/var/log` e seus subdiretórios.

### 8. Usar expressões regulares avançadas
```sh
grep -E "(falha|erro|crítico)" arquivo.log
```
Isso buscará qualquer uma das palavras "falha", "erro" ou "crítico" no arquivo.

## Opções Comuns

| Opção  | Descrição |
|--------|-----------|
| `-i`   | Ignora maiúsculas e minúsculas na busca |
| `-n`   | Exibe o número da linha das correspondências |
| `-v`   | Inverte a busca, mostrando linhas que **não** contêm o padrão |
| `-c`   | Exibe apenas a contagem de linhas que correspondem ao padrão |
| `-o`   | Exibe apenas as correspondências exatas do padrão |
| `-r`   | Busca recursivamente em diretórios |
| `-E`   | Usa expressões regulares estendidas |

## Conclusão

O comando `grep` é uma ferramenta poderosa para busca e filtragem de texto. Ele é frequentemente usado em conjunto com outros comandos para análise de logs, manipulação de arquivos e extração de informações relevantes.

