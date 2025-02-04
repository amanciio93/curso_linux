# Comando NETSTAT

O comando **netstat** (network statistics) é utilizado para exibir informações sobre conexões de rede, tabelas de roteamento, estatísticas de interface e muito mais. Ele é uma ferramenta essencial para diagnóstico e monitoramento de redes.

## Sintaxe básica:
```bash
netstat [opções]
```

## Opções comuns:
| Opção | Descrição |
|--------|------------|
| `-a` | Exibe todas as conexões e portas de escuta |
| `-t` | Mostra apenas conexões TCP |
| `-u` | Mostra apenas conexões UDP |
| `-n` | Exibe endereços e portas numericamente |
| `-p` | Exibe o processo associado a cada conexão |
| `-r` | Mostra a tabela de roteamento |
| `-i` | Exibe estatísticas das interfaces de rede |

## Exemplos de uso:

1. **Listar todas as conexões ativas:**
```bash
netstat -a
```

2. **Exibir conexões TCP ativas:**
```bash
netstat -t
```

3. **Exibir conexões UDP ativas:**
```bash
netstat -u
```

4. **Exibir conexões com endereços numéricos:**
```bash
netstat -n
```

5. **Mostrar processos associados às conexões:**
```bash
netstat -p
```

6. **Exibir a tabela de roteamento:**
```bash
netstat -r
```

7. **Monitorar conexões ativas continuamente:**
```bash
watch netstat -an
```

## Alternativas modernas ao netstat
O `netstat` foi substituído em algumas distribuições Linux pelo comando `ss` (socket statistics), que oferece informações semelhantes com mais eficiência:
```bash
ss -tulnp
```

## Conclusão
O comando `netstat` é uma ferramenta útil para análise de conexões e diagnósticos de rede. Embora esteja sendo gradualmente substituído pelo `ss`, ele ainda é amplamente utilizado por administradores de sistemas e redes.