# Comando `head` no UNIX

O comando `head` é usado para exibir as primeiras linhas de um arquivo no UNIX e sistemas baseados em Linux. Ele é útil para visualizar rapidamente o início de um arquivo sem precisar abri-lo completamente.

## Sintaxe

```sh
head [OPÇÕES] [ARQUIVO]
```

Se nenhum arquivo for especificado, o `head` lê da entrada padrão.

## Exemplos de Uso

### 1. Exibir as 10 primeiras linhas (padrão)
```sh
head arquivo.txt
```

### 2. Especificar o número de linhas a serem exibidas
```sh
head -n 5 arquivo.txt
```

### 3. Exibir os primeiros bytes de um arquivo
```sh
head -c 20 arquivo.txt
```
Isso exibirá os primeiros 20 bytes do arquivo.

### 4. Usar `head` com `cat` para visualizar um arquivo grande
```sh
cat arquivo.txt | head -n 15
```

### 5. Exibir múltiplos arquivos
```sh
head arquivo1.txt arquivo2.txt
```
Isso mostrará as 10 primeiras linhas de cada arquivo, separadas por um cabeçalho com o nome do arquivo.

## Opções Comuns

| Opção  | Descrição |
|--------|-----------|
| `-n`   | Define o número de linhas a serem exibidas (ex: `-n 5`) |
| `-c`   | Exibe um número específico de bytes (ex: `-c 20`) |
| `-q`   | Suprime os cabeçalhos ao exibir múltiplos arquivos |
| `-v`   | Mostra sempre o cabeçalho com o nome do arquivo |

## Conclusão

O comando `head` é uma ferramenta simples e eficiente para visualizar rapidamente o conteúdo inicial de arquivos de texto. Ele é frequentemente usado em conjunto com outros comandos para análise de dados e depuração de arquivos de log.

