Aqui está a documentação do comando mv em formato .md para você copiar e colar:

# Comando `mv` - Mover ou Renomear Arquivos e Diretórios no UNIX

O comando `mv` é utilizado para mover ou renomear arquivos e diretórios no sistema UNIX e em sistemas baseados em Linux.

## Sintaxe

```bash
mv [opções] origem destino

    origem: O arquivo ou diretório que você deseja mover ou renomear.
    destino: O local de destino para onde o arquivo ou diretório será movido ou o novo nome que será atribuído.

Opções Comuns

    -i ou --interactive: Solicita confirmação antes de sobrescrever arquivos existentes.
    -f ou --force: Força a movimentação sem pedir confirmação, sobrescrevendo arquivos existentes.
    -u ou --update: Move os arquivos apenas se a origem for mais recente que o destino.
    -v ou --verbose: Exibe detalhes do processo de movimentação.

Exemplos de Uso
1. Mover um arquivo para outro diretório

mv arquivo.txt /caminho/do/destino/

2. Renomear um arquivo

mv arquivo_antigo.txt arquivo_novo.txt

3. Mover e renomear um arquivo

mv arquivo.txt /caminho/do/destino/arquivo_novo.txt

4. Mover um diretório recursivamente

mv diretorio /caminho/do/destino/

5. Mover com confirmação antes de sobrescrever

mv -i arquivo.txt /caminho/do/destino/

6. Forçar a movimentação e sobrescrever sem confirmação

mv -f arquivo.txt /caminho/do/destino/

Observações

    Caso o destino seja um diretório, o arquivo ou diretório de origem será movido para dentro do diretório de destino.
    O comando mv pode sobrescrever arquivos de destino sem aviso, a menos que a opção -i seja usada.
    O comando também pode ser usado para renomear arquivos ou diretórios dentro do mesmo diretório.


Agora você pode copiar esse texto e colar em um arquivo `.md`.