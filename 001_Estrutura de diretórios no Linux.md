# Estrutura de Diretórios no Linux

A estrutura de diretórios do Linux é hierárquica, organizada em forma de árvore com a raiz (`/`) no topo. Cada diretório tem um propósito específico, o que facilita a organização e o gerenciamento do sistema. Aqui está uma visão geral dos principais diretórios no Linux:

---

## Estrutura básica de diretórios
```plaintext
/
├── bin
├── boot
├── dev
├── etc
├── home
├── lib
├── media
├── mnt
├── opt
├── proc
├── root
├── run
├── sbin
├── srv
├── sys
├── tmp
├── usr
└── var
```

---

## Descrição dos diretórios principais

### **1. `/` (Raiz)**
- É o topo da hierarquia do sistema de arquivos.
- Todos os outros diretórios estão dentro dele.
- **Cuidado:** Alterações imprudentes na raiz podem comprometer o sistema.

### **2. `/bin` (Binários essenciais)**
- Contém programas básicos necessários para o funcionamento do sistema, acessíveis a todos os usuários.
- Exemplos: `ls`, `cp`, `mv`, `cat`, `echo`.

### **3. `/boot`**
- Contém os arquivos necessários para inicializar o sistema.
- Exemplos: Kernel (`vmlinuz`), initramfs e arquivos de configuração do GRUB.

### **4. `/dev` (Dispositivos)**
- Contém arquivos que representam dispositivos de hardware.
- Exemplos:
  - `sda` → Disco rígido principal.
  - `tty` → Terminais.
  - `null` → Dispositivo de descarte.

### **5. `/etc` (Configurações)**
- Armazena arquivos de configuração do sistema e dos aplicativos.
- Exemplos:
  - `/etc/fstab` → Configuração das partições.
  - `/etc/hosts` → Mapeamento de IPs e nomes de host.

### **6. `/home`**
- Diretório pessoal dos usuários.
- Cada usuário tem sua própria pasta em `/home`.
- Exemplo: `/home/jonathan` contém os arquivos e configurações do usuário "jonathan".

### **7. `/lib` (Bibliotecas essenciais)**
- Contém bibliotecas compartilhadas usadas pelos programas em `/bin` e `/sbin`.

### **8. `/media`**
- Monta automaticamente dispositivos externos, como pen drives e discos externos.
- Exemplo: `/media/jonathan/PenDrive`.

### **9. `/mnt`**
- Ponto de montagem manual para dispositivos ou sistemas de arquivos.

### **10. `/opt` (Pacotes opcionais)**
- Contém softwares instalados manualmente pelo usuário ou pacotes adicionais que não fazem parte do sistema padrão.

### **11. `/proc` (Sistema de arquivos virtual)**
- Informações sobre processos e o kernel em tempo real.
- Exemplos:
  - `/proc/cpuinfo` → Informações da CPU.
  - `/proc/meminfo` → Informações de memória.

### **12. `/root`**
- Diretório pessoal do usuário **root** (administrador do sistema).

### **13. `/run`**
- Armazena informações temporárias sobre o sistema e processos em execução desde o boot.

### **14. `/sbin` (Binários de administração)**
- Contém programas administrativos usados pelo root.
- Exemplos: `fsck`, `reboot`, `iptables`.

### **15. `/srv`**
- Contém dados para serviços como servidores web e FTP.

### **16. `/sys`**
- Similar a `/proc`, contém informações do kernel e dispositivos conectados.

### **17. `/tmp` (Arquivos temporários)**
- Armazena arquivos temporários criados por programas e pelo sistema.
- Os dados geralmente são apagados ao reiniciar o sistema.

### **18. `/usr` (Arquivos de usuário)**
- Contém programas, bibliotecas e documentação adicionais.
- Subdiretórios importantes:
  - `/usr/bin` → Programas acessíveis por usuários.
  - `/usr/lib` → Bibliotecas para aplicativos em `/usr/bin`.
  - `/usr/local` → Programas instalados manualmente pelo administrador.

### **19. `/var` (Variáveis)**
- Armazena arquivos que mudam constantemente, como logs, cache e dados de aplicativos.
- Exemplos:
  - `/var/log` → Logs do sistema.
  - `/var/www` → Arquivos de servidores web (como o Apache).

---

## Curiosidades
- A estrutura segue o padrão **FHS** (Filesystem Hierarchy Standard).
- Diretórios como `/proc` e `/sys` são **sistemas de arquivos virtuais**, não armazenam dados no disco, mas sim informações do kernel e hardware.

