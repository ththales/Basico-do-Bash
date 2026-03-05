# Lista de Comandos básicos terminal
- clear: limpa o terminal

- ctrl + l: limpa o terminal

- history: exibe o histórico de comandos digitados no terminal
	- history -c: limpa o histórico de comandos

- pwd: mostra o caminho do diretório atual

- ls: lista o conteúdo de uma pasta
	- lscpu: mostra informações relacionadas ao processador
   	- lsusb: mostra informações relacionadas aos dispositivos usb
	- lspci: mostra informações relacionadas as linhas PCI
	- lsblk: mostra informações relacionadas ao disco

- cd: muda o diretório atual para o selecionado
	- Ex: cd "Nome da pasta"
	- cd .. : volta uma pasta
	- cd / : volta para o diretório home

- mkdir: cria diretórios
	- Ex: mkdir "Nome da pasta"

- touch: cria arquivos
  	- Ex: touch exemplo.txt

- rm: apaga arquivos
	- Ex: rm exemplo.txt
	- rm -rf: apaga pastas com arquivos

- rmdir: apaga pastas vazias
	- Ex: rm diretorioExemplo

- mv: renomeia arquivos
	- Ex: mv exemplo.txt novoNome.txt

- cp: copia arquivos
	- Ex: cp arquivoDeOrigem arquivoDeDestino

- find: procura por arquivos
	- Ex: find pontoDeOrigem -name nomeDoArquivo

- nano: abre um arquivo no editor de texto
	- Ex: nano exemplo.txt

- cat: concatena ou exibe/lê conteúdo de arquivos
	- cat < arquivo: concatena ou exibe/lê conteúdo de arquivos
   	- Ex: cat exemplo.txt

- whoami: exibe o nome de usuário, data e horário local da máquina

- sudo: permite usuarios rodar comandos com privilégios de administrador
	- sudo su
	- Ex: sudo apt-get update

- informaçãoASerPassada >> arquivoDeTexto.txt: copia informações de um comando para um arquivo de texto
	- Ex: whoami >> info.txt

- head: exibe as primeiras linhas de um arquivo
	- Ex: head exemplo.txt

- tail: exibe as últimas linhas de um arquivo
  	- Ex: tail exemplo.txt

- less: exibe o conteúdo de um arquivo gradativamente
	- Ex: less exemplo.txt

- hostname: exibe o nome da máquina
	- hostname -I: lista todas as interfaces de IP da máquina
        
- ip a: lista todas as informações de cada endereço de IP da máquina
	- ip a | grep inet: filtra todas as informações que contenha apenas interfaces de rede (inet)

- ping: mostra a latência da sua internet com algum servidor/site
	- Ex: ping google.com

- free -h: lista a quantidade de memória RAM consumida (notação humana)

- free -m: lista a quantidade de memória RAM consumida (notação de máquina)

- top: gerenciador de tarefas/monitor do sistema e recursos (quantidade de processos e % de uso de CPU, GPU E MEM)

- htop: gerenciador de tarefas/monitor do sistema e recursos (quantidade de processos e % de uso de CPU, GPU E MEM)

- ps: exibe instâncias rodando no terminal atual
	- ps aux: lista de processos rodando no terminal atual
	- ps aux | grep nomeDoProcesso: lista o processo desejado

- pgrep nomeDoProcesso: lista o PID do processo desejado

- kill PID: finaliza o processo desejado

- df -h: mostra o armazenamento usado e disponível da máquina

- ncdu: gerenciador de disco

- dpkg -l: lista todos os programas instalados na máquina

- uname: informações do kernel do sistema
	- uname -r: versão em específica do kernel

**DICAS EXTRA:**  
- usuário normal: ~  
- usuário root: #  
- para ter um manual para cada comando, basta escrever **man nomeDoComando** ou **nomeDoComando --help**  
- apertar tab autocompleta as informações sugeridas  
- 'Q' fecha abas específicas do terminal  
- CTRL + C cancela qualquer comando do terminal  
- sudo apt install htop: instala o comando htop para monitorar recursos do sistema  
- sudo apt install ncdu: instala o comando ncdu para gerenciar o disco  
