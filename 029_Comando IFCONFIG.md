# Comando IFCONFIG

O comando **ifconfig** (interface configurator) é utilizado para configurar e exibir informações sobre interfaces de rede em sistemas Unix/Linux. Ele permite visualizar endereços IP, configurar interfaces e diagnosticar problemas de rede.

## Sintaxe básica:
```bash
ifconfig [interface] [opções]
```

Se usado sem argumentos, exibe informações sobre todas as interfaces de rede ativas.

## Exibir informações sobre as interfaces de rede:
```bash
ifconfig
```

## Ativar ou desativar uma interface de rede:
| Comando | Descrição |
|---------|------------|
| `ifconfig eth0 up` | Ativa a interface `eth0` |
| `ifconfig eth0 down` | Desativa a interface `eth0` |

## Configurar um endereço IP estático:
```bash
ifconfig eth0 192.168.1.100 netmask 255.255.255.0
```

## Configurar o endereço MAC (requer privilégios de root):
```bash
ifconfig eth0 hw ether 00:1A:2B:3C:4D:5E
```

## Configurar o MTU (Maximum Transmission Unit):
```bash
ifconfig eth0 mtu 1500
```

## Alternativa moderna ao ifconfig
O `ifconfig` faz parte do pacote **net-tools**, que está obsoleto em algumas distribuições Linux. A alternativa moderna é o comando `ip`:
```bash
ip addr show
ip link set eth0 up
ip link set eth0 down
```

## Conclusão
O comando `ifconfig` ainda é útil para configurar e diagnosticar interfaces de rede, mas em muitas distribuições modernas foi substituído pelo comando `ip`.

