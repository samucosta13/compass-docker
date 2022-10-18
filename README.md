# Documentação

O objetivo dessa documentação é mostrar o passo a passo para subir uma aplicação Wordpress + DB Mysql utilizando docker. Os sistemas operacionais Windows e Ubuntu serão abordados nessa documentação.

> ## Sumário


> ## Windows
**Pré requisitos:**
* Primeiramente, é necessário fazer a instalação do [Docker Desktop](https://docs.docker.com/desktop/install/windows-install/). 
* Após isso, verifique se o Hyper-V esta habilitado. Para isso, abra o prompt de comando como administrador e execute o seguinte comando: `bcdedit`.
Caso esteja desabilitado, ainda com o prompt de comando como administrador, execute: `bcdedit /set hypervisorlaunchtype auto`

Feito os passos anteriores, o Docker Desktop estará pronto para uso. Utilize o arquivo [docker-compose.yml](https://github.com/samucosta13/compass-docker/blob/main/docker-compose.yml) deste repositório para estruturar os serviços e definir as cofigurações da aplicação. Esse arquivo pode ser modificado por qualquer editor de texto de sua preferência. Neste caso, foi utilizado o editor de código fonte [Visual Studio Code](https://code.visualstudio.com/download)

Antes de subir a aplicação, é necessário criar dois volumes: banco e wordpress. Para isso:
`d`

> ## Ubuntu



Antes de subir os containers, é necessário criar um Docker Volume chamado 'banco', para o MySQL, e outro chamado 'site', para o WordPress.
