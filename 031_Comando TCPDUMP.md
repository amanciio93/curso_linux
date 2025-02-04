# Comando TCPDUMP

O comando **tcpdump** é uma ferramenta de captura de pacotes de rede usada para diagnosticar e analisar o tráfego em interfaces de rede. Ele permite visualizar pacotes transmitidos e recebidos em tempo real.

## Sintaxe básica:
```bash
tcpdump [opções] [filtro]
```

## Exibir pacotes em tempo real:
```bash
tcpdump
```
Este comando captura pacotes de todas as interfaces disponíveis.

## Capturar pacotes em uma interface específica:
```bash
tcpdump -i eth0
```
Este comando captura pacotes apenas na interface `eth0`.

## Filtrar pacotes por protocolo:
| Protocolo | Comando |
|-----------|----------|
| ICMP | `tcpdump icmp` |
| TCP | `tcpdump tcp` |
| UDP | `tcpdump udp` |

## Capturar pacotes de um host específico:
```bash
tcpdump host 192.168.1.1
```

## Capturar pacotes de uma porta específica:
```bash
tcpdump port 80
```
Captura apenas pacotes relacionados ao tráfego HTTP.

## Capturar e salvar pacotes em um arquivo:
```bash
tcpdump -w captura.pcap
```
Os pacotes são armazenados no arquivo `captura.pcap`, que pode ser analisado posteriormente com ferramentas como Wireshark.

## Ler pacotes de um arquivo:
```bash
tcpdump -r captura.pcap
```

## Exibir pacotes com informações detalhadas:
```bash
tcpdump -vv
```

## Capturar apenas os primeiros bytes de cada pacote:
```bash
tcpdump -s 100
```
Captura apenas os primeiros 100 bytes de cada pacote.

## Conclusão
O `tcpdump` é uma ferramenta essencial para administradores de redes e segurança, permitindo a análise detalhada do tráfego da rede para diagnóstico e monitoramento.