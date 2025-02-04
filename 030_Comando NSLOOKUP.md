# Comando NSLOOKUP

O comando **nslookup** (Name Server Lookup) é uma ferramenta utilizada para consultar servidores DNS e obter informações sobre domínios e endereços IP. Ele é amplamente utilizado para diagnosticar problemas de resolução de nomes na rede.

## Sintaxe básica:
```bash
nslookup [opções] [domínio/IP]
```

## Consultar o IP de um domínio:
```bash
nslookup google.com
```
Saída esperada:
```
Server:  8.8.8.8
Address: 8.8.8.8#53

Non-authoritative answer:
Name:    google.com
Address: 142.250.217.78
```

## Consultar o domínio de um IP (Reverse Lookup):
```bash
nslookup 8.8.8.8
```

## Definir um servidor DNS específico para consulta:
```bash
nslookup google.com 8.8.8.8
```

## Entrar no modo interativo:
```bash
nslookup
```
No modo interativo, é possível realizar diversas consultas DNS sem precisar chamar o comando novamente. Alguns comandos úteis no modo interativo:
- **`server [IP]`** – Define um servidor DNS específico.
- **`set type=[registro]`** – Define o tipo de consulta (A, MX, TXT, etc.).
- **`exit`** – Sai do modo interativo.

Exemplo de consulta de registros MX (servidores de e-mail de um domínio):
```bash
nslookup
> set type=MX
> google.com
```

## Consultar registros específicos:
| Tipo de Registro | Descrição |
|-----------------|------------|
| `A` | Endereço IPv4 do domínio |
| `AAAA` | Endereço IPv6 do domínio |
| `MX` | Servidores de e-mail do domínio |
| `NS` | Servidores de nome do domínio |
| `TXT` | Registros de texto (SPF, DKIM, etc.) |
| `CNAME` | Nome canônico do domínio |

## Alternativas modernas ao nslookup
Embora o `nslookup` ainda seja amplamente utilizado, ferramentas modernas como `dig` e `host` oferecem recursos adicionais:
- **`dig google.com`** – Exibe informações detalhadas sobre o DNS.
- **`host google.com`** – Retorna rapidamente o IP do domínio.

## Conclusão
O comando `nslookup` é uma ferramenta poderosa para diagnóstico de problemas DNS, permitindo resolver nomes de domínio e consultar registros específicos de maneira simples e eficaz.