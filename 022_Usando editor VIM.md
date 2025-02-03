# Guia Completo do Editor de Texto Vim

## Introdução
O **Vim** (Vi IMproved) é um editor de texto altamente configurável e poderoso, amplamente utilizado por desenvolvedores e administradores de sistemas. Ele oferece modos distintos de operação e uma vasta gama de comandos eficientes.

## Instalação
Caso não esteja instalado, utilize os seguintes comandos:

- **Debian/Ubuntu**: `sudo apt install vim`
- **Fedora**: `sudo dnf install vim`
- **Arch Linux**: `sudo pacman -S vim`

## Modos do Vim
O Vim possui três modos principais:
- **Modo Normal**: Para navegação e manipulação de texto.
- **Modo Inserção**: Para digitação de texto (`i`, `a`, `o` para entrar neste modo).
- **Modo Comando**: Para executar comandos (`:` para entrar neste modo).

## Comandos Essenciais

### Navegação
- `h` → Esquerda
- `l` → Direita
- `j` → Baixo
- `k` → Cima
- `gg` → Ir para o início do arquivo
- `G` → Ir para o final do arquivo
- `Ctrl + d` → Rolar metade da página para baixo
- `Ctrl + u` → Rolar metade da página para cima

### Inserção de Texto
- `i` → Inserir antes do cursor
- `a` → Inserir após o cursor
- `o` → Nova linha abaixo
- `O` → Nova linha acima
- `Esc` → Sair do modo de inserção

### Edição
- `x` → Apagar caractere
- `dd` → Apagar linha
- `yy` → Copiar linha
- `p` → Colar
- `u` → Desfazer
- `Ctrl + r` → Refazer

### Busca e Substituição
- `/texto` → Buscar "texto" no arquivo
- `n` → Próxima ocorrência
- `N` → Ocorrência anterior
- `:%s/antigo/novo/g` → Substituir "antigo" por "novo" norquivo inteiro

### Manipulação de Arquivos
- `:w` → Salvar
- `:q` → Sair
- `:wq` → Salvar e sair
- `:q!` → Sair sem salvar
- `:e nome_arquivo` → Abrir outro arquivo

### Trabalhando com Múltiplos Arquivos
- `:split nome_arquivo` → Abrir arquivo em painel dividido
- `:vsplit nome_arquivo` → Abrir em painel vertical
- `Ctrl + w + w` → Alternar entre painéis

## Personalização do Vim
O arquivo de configuração do Vim fica em `~/.vimrc`. Exemplo de personalização:
```vim
set number       " Exibir números das linhas
set autoindent   " Indentação automática
set tabstop=4    " Definir tabulação como 4 espaços
syntax on        " Ativar realce de sintaxe
```

## Conclusão
O Vim é um editor altamente eficiente, ideal para usuários avançados que buscam produtividade. Com prática, torna-se uma ferramenta poderosa para manipulação de textos e código.

Para mais informações, consulte o manual:
```
:help
```

