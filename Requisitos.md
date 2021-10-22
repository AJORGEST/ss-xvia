# Requerimento servidores seguro em Orgãos

Ambiente recomendado para servidores seguro em orgãos

### Haproxy para fazer o balanceamento de carga tcp Layer 4. 

1. LoadBalancer  `2 vCPU [ 4 GB de RAM ] disk 50 GB`     IP externo  DNS  xvia.xxx.mt.gov.br` 
*  Master   `2 vCPU [ 4 GB de RAM ] disk 100 GB`         IP interno       
*  Slave    `2 vCPU [ 4 GB de RAM ] disk 100 GB`         IP interno 
*  BD Postgres   `2 vCPU [ 4 GB de RAM ]  disk 200 GB`   IP interno 
    
	O orgão deverá disponibilizar os equipamentos com ingressos na rede interna abaixo:
	
	     portas: tcp:22; tcp:80; tcp:443; tcp:4001; tcp:5500; tcp:5577; tcp:8888; tcp:8899   IN 	
	     portas: tcp:22; tcp:80; tcp:443; tcp:4001; tcp:5500; tcp:5577; tcp:8888; tcp:8899   OUT
		
	
	Comunicação entre orgãos diferente, utilizando ip externo, dns e portas de entrada e saída criptografadas:
	
		DNS: xvia.xxx.mt.gov.br - IP 201.49.XXX.XX Ingresso  - tcp:5500 tcp:5577
		
		
