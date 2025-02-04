# Compactar e Descompactar Arquivos no Linux

Neste documento, vamos abordar o uso dos comandos **tar** e **zip** para compactar e descompactar arquivos no Linux.

## 📌 Usando o `tar`
O comando **tar** é amplamente utilizado para arquivar múltiplos arquivos em um único arquivo compactado ou não.

### 📂 Criar um arquivo `.tar`
```bash
tar -cvf arquivo.tar diretorio/
```
- `c` – Cria um novo arquivo.
- `v` – Mostra detalhes da operação.
- `f` – Especifica o nome do arquivo de saída.

### 📦 Criar um arquivo `.tar.gz` (compactado com gzip)
```bash
tar -czvf arquivo.tar.gz diretorio/
```
- `z` – Comprime usando `gzip`.

### 🗜️ Criar um arquivo `.tar.bz2` (compactado com bzip2)
```bash
tar -cjvf arquivo.tar.bz2 diretorio/
```
- `j` – Comprime usando `bzip2`.

### 🔍 Listar arquivos dentro de um `.tar`
```bash
tar -tvf arquivo.tar
```

### 📂 Extrair um `.tar`
```bash
tar -xvf arquivo.tar
```

### 📦 Extrair um `.tar.gz`
```bash
tar -xzvf arquivo.tar.gz
```

### 🗜️ Extrair um `.tar.bz2`
```bash
tar -xjvf arquivo.tar.bz2
```

## 📌 Usando o `zip`
O comando **zip** permite compactar arquivos em um formato amplamente utilizado em diferentes sistemas operacionais.

### 📂 Compactar arquivos em `.zip`
```bash
zip arquivo.zip arquivo1 arquivo2 diretorio/
```

### 🗜️ Compactar com nível máximo de compressão (0 a 9)
```bash
zip -9 arquivo.zip arquivo1 arquivo2
```

### 🔍 Listar arquivos dentro de um `.zip`
```bash
unzip -l arquivo.zip
```

### 📂 Extrair arquivos de um `.zip`
```bash
unzip arquivo.zip
```

### 📦 Extrair para um diretório específico
```bash
unzip arquivo.zip -d meu_diretorio/
```

### VER ARQUIVOS COMPACTADOS
```bash
tar -tvf <name_file>
```

## Conclusão
Os comandos `tar` e `zip` são essenciais para arquivamento e compactação no Linux. O `tar` é mais usado em sistemas Linux/Unix, enquanto o `zip` é útil para compatibilidade com Windows. Escolha o que melhor se adequa às suas necessidades!