#### REQUISITOS TÉCNICOS PARA INSTALAÇÃO DO DO SERVIDOR SEGURO

### 1. Plataformas suportada

Sistema operacional Ubuntu Server 18.04 Long-Term Support (LTS) em uma plataforma 64-bit. VM'S LINUX

O software do servidor central pode ser instalado tanto em hardware físico quanto virtualizado (até o momento, Xen e Oracle VirtuaBox não foram testados).


### 2. Dados de referência

Ambiente de desenvolvimento

* `Ubuntu  18.04, 64-bit 3 GB RAM, 50 GB de disco livre`  

Ambiente de Produção

* `Ubuntu  18.04, 64-bit 4 GB RAM, 200 GB de disco livre`

Ambiente de produção é necessário termos vm's, ou máquinas de cluster de bancos, vm's para o servidor central, servidor seguro, AC, e servidor de gerenciamento. 

Obs: A máquina de AC é responsável pela geração e validação de assinatura dos certificados - "podendo ser  utilizada tanto em produção como desenvolvimento".



