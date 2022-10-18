# Documentação

O objetivo dessa documentação é mostrar o passo a passo para subir uma aplicação Wordpress + DB Mysql utilizando docker. Os sistemas operacionais Windows e Ubuntu serão abordados nessa documentação.

> ## Sumário


> ## Windows
* Primeiramente, é necessário fazer a instalação do [Docker Desktop](https://docs.docker.com/desktop/install/windows-install/). 
* Após isso, verifique se o Hyper-V essa habilitado. Para isso, abra o prompt de comando como administrador e execute o seguinte comando: `bcdedit`.
Caso esteja desabilitado, ainda com o prompt de comando como administrador, execute: `bcdedit /set hypervisorlaunchtype auto`


> ## Ubuntu



Antes de subir os containers, é necessário criar um Docker Volume chamado 'banco', para o MySQL, e outro chamado 'site', para o WordPress.
