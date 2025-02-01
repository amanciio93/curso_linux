# Comando `tail` no UNIX

O comando `tail` é utilizado para exibir as últimas linhas de um arquivo no UNIX e sistemas baseados em Linux. Ele é muito útil para monitorar arquivos de log e visualizar mudanças em tempo real.

## Sintaxe

```sh
tail [OPÇÕES] [ARQUIVO]
```

Se nenhum arquivo for especificado, o `tail` lê da entrada padrão.

## Exemplos de Uso

### 1. Exibir as 10 últimas linhas (padrão)
```sh
tail arquivo.txt
```

### 2. Especificar o número de linhas a serem exibidas
```sh
tail -n 5 arquivo.txt
```
Isso exibirá as últimas 5 linhas do arquivo.

### 3. Exibir os últimos bytes de um arquivo
```sh
tail -c 20 arquivo.txt
```
Isso exibirá os últimos 20 bytes do arquivo.

### 4. Monitorar um arquivo em tempo real
```sh
tail -f arquivo.log
```
Isso mantém o arquivo aberto e exibe novas linhas conforme são adicionadas.

### 5. Exibir múltiplos arquivos
```sh
tail arquivo1.txt arquivo2.txt
```
Isso mostrará as 10 últimas linhas de cada arquivo, separadas por um cabeçalho com o nome do arquivo.

## Opções Comuns

| Opção  | Descrição |
|--------|-----------|
| `-n`   | Define o número de linhas a serem exibidas (ex: `-n 5`) |
| `-c`   | Exibe um número específico de bytes (ex: `-c 20`) |
| `-f`   | Mantém o arquivo aberto para exibir novas linhas em tempo real |
| `-q`   | Suprime os cabeçalhos ao exibir múltiplos arquivos |
| `-v`   | Mostra sempre o cabeçalho com o nome do arquivo |

## Conclusão

O comando `tail` é uma ferramenta poderosa para visualizar e monitorar arquivos de texto, especialmente logs. Ele é amplamente utilizado por administradores de sistemas e desenvolvedores para depuração e análise de arquivos.

