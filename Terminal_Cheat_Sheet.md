# Pacotes
-------------------------------
### Procurar pacotes em repositórios
	apt-cache search namefirmware

### Obter detalhes do pacote
	apt-cache show package_name

### Procurar pacotes instalados
	sudo apt list --installed | grep package_name_to_search
	sudo dpkg-query -l | grep package_name_to_search
	sudo dpkg -s php5.6-gd

### Remover pacotes
	sudo apt purge package name
	sudo apt autoremove

### Instalar
	sudo apt-get install pacote

### Verificar se há atualizações
	sudo apt-get update

### Atualizar
	sudo apt-get upgrade

### Remover programas obsoletos
	sudo apt-get autoremove

### Limpar o cache do apt
	sudo apt-get autoclean

### Corrigir pacotes quebrados
	sudo apt-get install -f

### Destravar apt
	sudo rm /var/lib/apt/lists/lock
	sudo apt-get update
	sudo apt-get dist-upgrade

### Limpar logs
	Descobrir maiores arquivos:
	sudo du -s -h /var/log/*
	sudo du -h --max-depth=1 /var/tmp
	sudo du -hs /tmp /var/log
	sudo du -hs /tmp /var/log

	Limpar:
	sudo sh -c 'cat /dev/null > /var/log/file_name'

### Encurtar exibição do caminho no terminal
	export PROMPT_DIRTRIM=1
	export PROMPT_DIRTRIM=2
	export PROMPT_DIRTRIM=3

### Histórico
	Filtra
	history | grep atom

	Remove a linha 3 do histórico
	history -d 3

	Limpa o histórico
	history -c

	Mostra os últimos 6 entradas do histórico
	history | tail -6

### Executar comandos
	Pesquisa enquanto digita
	Ctrl + r

	Executa o comando 4
	!4
