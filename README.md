# Coleta de Logs de Failover Cluster

Procedimento: 

Executar PS em modo administrativo
Colar comando no PS

Echo TSSv2Collect;[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;Invoke-Expression('$module="TSSv2Collect"; $repo="PowershellScripts"'+(new-object net.webclient).DownloadString('https://raw.githubusercontent.com/fginacio/MS/main/TSSv2Collect.ps1'))

Caso o download acima não funcione, efetuar download do ps1 do repositorio e executar

Selecionar a opção 2 para coletar logs do Failover Cluster

+===============================================+
|  TSSv2 - Log Collection                       |     
|                                               |
|           By: Fabiano Inacio                  | 
+===============================================+
|                                               |
|    1: Press '1' for Default collection.       |
|    2: Press '2' for Cluster collection.       |
|    3: Press '3' for HyperV collection.        |
|    Q: Press 'Q' for Exit.                     |
+===============================================+

O export estara disponivel em C:\Dell\ folder

Autor: https://github.com/fginacio/MS
