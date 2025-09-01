# IBM_MQ_Multi-Inst-ncia_com_App_Connect_Enterprise_Red-Hat-Enterprise-Linux_v9.6

## Introdução

#### A continuidade de negócios tem sido um requisito central para as empresas que dependem de integrações em tempo real e troca confiável de mensagens Neste documento apresentamos um passo a passo completo para a instalação de um ambiente ``IBM MQ Multi-Instância`` combinado com ``IBM App Connect Enterprise (ACE)`` utilizando três servidores ``Red Hat Enterprise Linux (RHEL)``

| Função | Hostname | Papel |
| ------ | -------- | ----- |
| Servidor de armazenamento compartilhado (NFS) | http://IBMQ11.com | Exporta o diretório /MQHA para logs e dados de fila compartilhados. |
| Instância prioritária do queue manage | http://IBMQ12.com | Ativa por padrão (primary). |
| Instância de standby do queue manager | http://IBMQ13.com | Assume automaticamente em caso de falha do primary. |