
## Resumo das funções das portas da estrutura do x-via

##  Funções das portas de hosts na rede interna:
* `Porta de saída`   do servidor seguro para a rede externa  `TCP  80`
* `Porta de saída`   do servidor seguro para a rede externa  `TCP 443`
* `Porta de saída`   do servidor seguro para a rede externa  `TCP 4001`
* `Porta de saída`   do servidor seguro para a rede externa  `TCP 5500`
* `Porta de saída`   do servidor seguro para a rede externa  `TCP 5577`
* `Porta de saída`   do servidor seguro para a rede externa  `TCP 8888`
* `Porta de saída`   do servidor seguro para a rede externa  `TCP 8899`
* `Porta de saída`   do servidor seguro para a rede interna  `TCP 2080`
## entrada
* `Porta de entrada` da rede externa para o servidor seguro  `TCP 4000`
* `Porta de entrada` da rede externa para o servidor seguro  `TCP 9011`
* `Porta de entrada` da rede externa para o servidor seguro  `TCP 2080`

## Especificações de portas:
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
                   
                   
