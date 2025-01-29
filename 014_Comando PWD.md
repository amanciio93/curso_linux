Aqui está a documentação do comando pwd em formato .md para você copiar e colar:

# Comando `pwd` - Exibir o Diretório Atual no UNIX

O comando `pwd` (Print Working Directory) é utilizado para exibir o diretório atual em que você está no sistema UNIX e em sistemas baseados em Linux.

## Sintaxe

```bash
pwd [opções]

    sem opções: Exibe o caminho completo do diretório atual.

Opções Comuns

    -L ou --logical: Exibe o caminho simbólico do diretório atual (default).
    -P ou --physical: Exibe o caminho físico real, sem seguir links simbólicos.

Exemplos de Uso
1. Exibir o diretório atual

pwd

Exemplo de saída:

/home/usuario

2. Exibir o diretório atual considerando links simbólicos

pwd -L

3. Exibir o diretório atual sem seguir links simbólicos

pwd -P

Observações

    O comando pwd é útil para confirmar sua localização no sistema de arquivos.
    O caminho exibido é absoluto, ou seja, começa desde a raiz /.


Agora você pode copiar e colar este conteúdo em um arquivo `.md`.

