GERENCIAMENTO DE PACOTES
	- INSTALAR
	- ATUALIZAR
	- REMOVER
	- ATUALIZAR O SISTEMA
	
* Atualizando repositórios:
	sudo apt update - Atualiza os endereços dos pacotes nos repositórios atualizados;
	sudo apt upgrade - Atualiza os pacotes pelas novas versões;
	
* Instalando pacotes (Aplicativos):
	sudo apt install <pacote> - Instala o pacote escolhido;
	sudo apt show <pacote> - Exibe informações do pacote desejado;
	
* Deletando pacotes (Aplicativos):
	sudo apt remove ou purge <pacote> - Remove do seu sistema o pacote (Aplicativo);
	
* Atualizando o sistema Linux:
	sudo apt dist-upgrade
	
* Limpando pacotes e arquivos desnecessários:
	sudo apt autoremove
	sudo apt autoclean
	
* Buscando pacotes e aplicativos>
	sudo apt cache search <pacote>
