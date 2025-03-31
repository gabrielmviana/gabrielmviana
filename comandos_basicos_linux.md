# 📖 Guia de Comandos Linux

## 1️⃣ Gerenciamento de Arquivos

### 📂 Listar Arquivos
- `ls` → Lista arquivos e diretórios.
- `ls -l` → Lista arquivos em formato detalhado.
- `ls -a` → Mostra arquivos ocultos.

### 📂 Copiar, Mover e Remover Arquivos
- `cp arquivo.txt /caminho/destino/` → Copia um arquivo.
- `mv arquivo.txt /novo_destino/` → Move um arquivo.
- `rm arquivo.txt` → Remove um arquivo.

## 2️⃣ Gerenciamento de Processos

### 🖥️ Monitoramento
- `ps aux` → Lista processos ativos.
- `top` → Monitora processos em tempo real.

### 🔪 Finalizar Processos
- `kill -9 <PID>` → Mata um processo pelo ID.
- `pkill nome_do_processo` → Mata todos os processos com determinado nome.

## 3️⃣ Redes e Conectividade

### 🌐 Configuração de Rede
- `ip addr show` → Exibe os endereços IP da máquina.
- `ping <host>` → Testa conectividade com um host.
- `netstat -tulnp` → Lista conexões ativas.

### 📡 Manipulação de Rotas
- `route -n` → Exibe a tabela de rotas.
- `sudo route add -net 192.168.0.0 netmask 255.255.255.0 dev eth0` → Adiciona uma rota estática.

## 4️⃣ Gerenciamento de Usuários e Permissões

### 👤 Gerenciamento de Usuários
- `whoami` → Exibe o usuário atual.
- `id` → Mostra detalhes do usuário.
- `passwd` → Altera a senha.

### 🔑 Permissões de Arquivo
- `chmod 755 arquivo.txt` → Altera permissões.
- `chown usuario:grupo arquivo.txt` → Modifica dono e grupo.

## 5️⃣ Manipulação de Arquivos e Texto

### 📜 Exibir Conteúdo de Arquivos
- `cat arquivo.txt` → Exibe o conteúdo de um arquivo.
- `tac arquivo.txt` → Exibe o conteúdo ao contrário.
- `less arquivo.txt` → Permite rolar o conteúdo de um arquivo.

### 🔍 Buscar Texto em Arquivos
- `grep "palavra" arquivo.txt` → Busca uma palavra em um arquivo.
- `grep -r "palavra" /caminho/do/diretorio/` → Busca recursivamente.

## 6️⃣ Arquivamento e Compressão

### 📦 Compactação
- `tar -czvf backup.tar.gz /caminho/dos/arquivos` → Cria um arquivo `.tar.gz`.
- `tar -xzvf backup.tar.gz` → Extrai um arquivo `.tar.gz`.

## 7️⃣ Segurança e Firewall

### 🔥 Firewall com IPTables
- `iptables -A INPUT -m conntrack --ctstate RELATED,ESTABLISHED -j ACCEPT` → Permite conexões estabelecidas.
- `iptables -A INPUT -p tcp --dport 22 -j ACCEPT` → Libera a porta SSH.

## 8️⃣ Edição e Personalização

### ✏️ Editores de Texto
- `nano arquivo.txt` → Abre o arquivo no editor Nano.
- `vim arquivo.txt` → Abre o arquivo no editor Vim.

### 🛠️ Personalização do Terminal
- `echo "alias ll='ls -l'" >> ~/.bashrc && source ~/.bashrc` → Cria um alias para `ls -l`.

---