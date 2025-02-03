# Guia Completo do Editor de Texto Nano (GNU)

## Introdução
O **Nano** é um editor de texto simples e fácil de usar, disponível na maioria das distribuições Linux. Ele permite edição rápida diretamente no terminal, sendo uma alternativa ao Vi e Vim.

## Instalação
O Nano geralmente vem pré-instalado, mas pode ser instalado manualmente com:

- **Debian/Ubuntu**: `sudo apt install nano`

## Abrindo um Arquivo
Para abrir um arquivo (ou criar um novo, se não existir):
```
nano nome_do_arquivo
```

## Interface Básica
- **Área principal**: Onde o texto é editado.
- **Rodapé**: Mostra comandos úteis. `^` representa a tecla **Ctrl**.

## Comandos Essenciais

### Edição
- `Ctrl + G` → Exibir ajuda
- `Ctrl + X` → Fechar o Nano (solicita salvar se houver alterações)
- `Ctrl + O` → Salvar arquivo (confirma com Enter)
- `Ctrl + K` → Cortar linha
- `Ctrl + U` → Colar linha
- `Ctrl + J` → Justificar texto
- `Alt + U` → Desfazer ação
- `Alt + E` → Refazer ação

### Navegação
- `Ctrl + A` → Ir para o início da linha
- `Ctrl + E` → Ir para o final da linha
- `Ctrl + Y` → Rolar uma página para cima
- `Ctrl + V` → Rolar uma página para baixo
- `Ctrl + _` → Ir para uma linha específica (digite o número e pressione Enter)

### Busca e Substituição
- `Ctrl + W` → Pesquisar no texto
- `Ctrl + R` → Substituir texto (use `Ctrl + W` para buscar e `Ctrl + R` para substituir)

### Manipulação de Arquivos
- `Ctrl + T` → Abrir explorador de arquivos
- `Ctrl + R` → Inserir conteúdo de outro arquivo
- `Ctrl + X` → Sair do Nano (se houver alterações, ele pedirá para salvar)

## Atalhos Avançados
- `Ctrl + 6` → Marcar posição (selecionar texto)
- `Ctrl + Shift + 6` → Copiar texto selecionado
- `Alt + Shift + 3` → Ativar/Desativar quebra automática de linha
- `Ctrl + C` → Exibir posição do cursor

## Configuração do Nano
O arquivo de configuração fica em `/etc/nanorc` (global) ou `~/.nanorc` (usuário). Exemplos de personalização:

```bash
set autoindent  # Ativar indentação automática
set mouse       # Permitir uso do mouse
set tabsize 4   # Definir tabulação como 4 espaços
```

## Conclusão
O Nano é um editor poderoso para usuários que preferem simplicidade sem sacrificar funcionalidades essenciais. Ele é ideal para edição rápida de arquivos em servidores e sistemas Linux.

Para mais detalhes, consulte o manual com:
```
man nano
```
