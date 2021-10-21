# Requerimento servidores seguro em Orgãos

Ambiente recomendado  para servidores seguro

### Obs: Haproxy para fazer o balanceamento de carga tcp Layer 4. 

* `HAPROXY  2 vCPU [ 4 GB de RAM ] [50 GB]`    `dominio`  xvia.xxx.mt.gov.br  
* `PRODUÇÃO 2 vCPU [ 4 GB de RAM ] [200 GB]`   `dominio`  xvia.xxx.mt.gov.br  
* `PRODUÇÃO 2 vCPU [ 4 GB de RAM ] [200 GB]`   `dominio`  xvia.xxx.mt.gov.br 
* `DESENV   2 vCPU [ 4 GB de RAM ]  [100 GB]`  `dominio`  xvia-dev.xxx.mt.gov.br
    
	O orgão deverá disponibilizar os dns conforme exemplo acima e equipamentos com recursos e portas liberadas na rede interna:
	
	     Ingresso das portas: tcp:22; tcp:80; tcp:443; tcp:4001; tcp:5500; tcp:5577; tcp:8888; tcp:8899   IN 	
	     Ingresso das portas: tcp:22; tcp:80; tcp:443; tcp:4001; tcp:5500; tcp:5577; tcp:8888; tcp:8899   OUT
		
	
	Comunicação dos servidores seguro entre orgãos utilizando ip externo:
	
		DNS: xvia.xxx.mt.gov.br - IP 201.49.XXX.XX Ingresso  - tcp:5500 tcp:5577
		DNS: xvia-dev.xxxx.mt.gov.br - IP 201.49.XXX.XX Ingresso - tcp:5500 tcp:5577	
		
#  Funções das portas de hosts na rede interna:
* `Porta de saída`   do servidor seguro para a rede externa  `TCP  80`
* `Porta de saída`   do servidor seguro para a rede externa  `TCP 443`
* `Porta de saída`   do servidor seguro para a rede externa  `TCP 4001`
* `Porta de saída`   do servidor seguro para a rede externa  `TCP 5500`
* `Porta de saída`   do servidor seguro para a rede externa  `TCP 5577`
* `Porta de saída`   do servidor seguro para a rede externa  `TCP 8888`
* `Porta de saída`   do servidor seguro para a rede externa  `TCP 8899`
* `Porta de saída`   do servidor seguro para a rede interna  `TCP 2080`
# entrada
* `Porta de entrada` da rede externa para o servidor seguro  `TCP 4000`
* `Porta de entrada` da rede externa para o servidor seguro  `TCP 9011`
* `Porta de entrada` da rede externa para o servidor seguro  `TCP 2080`

# Especificações de portas:
* `Porta de entrada TCP 80 ` Conexão com o sistema de informação                
* `Porta de entrada TCP 443  ` Conexão com o sistema de informação SSL         
* `Porta de entrada TCP 5577 ` Consulta ao cache das respostas de OCSP seguros   
* `Porta de entrada TCP 4001 ` Comunicação com o servidor central
* `Porta de entrada TCP 4000 ` Porta de comunicação da interface da aplicação web                
* `Porta de entrada TCP 5500 ` Troca de mensagens entre os servidores seguros   
* `Porta de entrada TCP 8888 ` Serviços de OCSP e carimbo de tempo mais comuns    
* `Porta de entrada TCP 8899 ` Serviços de OCSP e carimbo de tempo mais comuns   
* `Porta de monitoramento operacional TCP 2080` localhost por padrão             

	
  O objetivo:
  Manter as bases segura através de API's cadastrada e gerenciadas pelo gestor do orgão:
    
     Objetivo:    * Validar acesso internos;   
                  * Gerenciar os acessos seguro;
                  * Validar os dns públicos;
                  * Validar os ips públicos  
                  * Validar URL'S produção Homolgação
                   
                   
