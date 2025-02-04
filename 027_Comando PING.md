# Comando PING

O comando **ping** é utilizado para testar a conectividade entre dois dispositivos em uma rede. Ele envia pacotes ICMP (Internet Control Message Protocol) para um host remoto e mede o tempo que leva para receber uma resposta.

## Como funciona?
1. O comando envia um **pacote ICMP Echo Request** para o destino.
2. Se o destino estiver acessível, ele responde com um **pacote ICMP Echo Reply**.
3. O ping mede o tempo entre o envio e o recebimento da resposta (latência).
4. Se não houver resposta, isso pode indicar que o destino está inacessível ou bloqueando ICMP.

## Sintaxe básica:
```bash
ping [opções] destino
```
Exemplo:
```bash
ping google.com
```
Saída esperada:
```
PING google.com (142.250.217.78): 56 data bytes
64 bytes from 142.250.217.78: icmp_seq=1 ttl=118 time=12.5 ms
64 bytes from 142.250.217.78: icmp_seq=2 ttl=118 time=12.3 ms
```

## Opções úteis:
| Opção | Descrição |
|--------|------------|
| `-c <n>` | Define o número de pacotes a serem enviados (ex.: `ping -c 4 google.com`) |
| `-i <segundos>` | Define o intervalo entre os pacotes enviados (ex.: `ping -i 2 google.com`) |
| `-s <bytes>` | Define o tamanho do pacote enviado (ex.: `ping -s 128 google.com`) |
| `-t` | No Windows, faz o ping rodar continuamente até ser interrompido |
| `-w <tempo>` | Define um tempo limite para a execução do ping |

## Para interromper o PING
- No Linux e MacOS: **CTRL + C**
- No Windows: **CTRL + Break** ou **CTRL + C**

## Diagnóstico com PING
- **Resposta bem-sucedida**: Indica que o destino está acessível.
- **Request timed out**: O destino não respondeu (pode estar offline ou bloqueando ICMP).
- **Unknown host**: Nome do host não pode ser resolvido (DNS pode estar configurado incorretamente).
- **Destination host unreachable**: O destino não pode ser alcançado (problema na rota de rede).

## Conclusão
O comando `ping` é uma ferramenta essencial para diagnóstico de redes, permitindo verificar a conectividade entre dispositivos, testar latência e identificar problemas de conexão.

