# Documentação

O objetivo dessa documentação é mostrar o passo a passo para subir uma aplicação Wordpress + DB Mysql utilizando docker. Os sistemas operacionais Windows e Ubuntu serão abordados nessa documentação.


> ## Windows  

**Pré requisitos:**
* Instalar [Docker Desktop](https://docs.docker.com/desktop/install/windows-install/). 
* Verificar se o Hyper-V esta habilitado. Para isso, abra o prompt de comando como administrador e execute o seguinte comando: `bcdedit`.
Caso esteja desabilitado, ainda com o prompt de comando como administrador, execute `bcdedit /set hypervisorlaunchtype auto` e reinicie a máquina.

Utilize o arquivo *[docker-compose.yml](https://github.com/samucosta13/compass-docker/blob/main/docker-compose.yml)* deste repositório para estruturar os serviços e definir as cofigurações da aplicação. Esse arquivo pode ser modificado por qualquer editor de texto de sua preferência. Neste caso, foi utilizado o editor de código fonte [Visual Studio Code](https://code.visualstudio.com/download).

Antes de subir a aplicação, é necessário criar dois volumes: banco e site. Para isso, no Power Shell do Windows, ou até mesmo no terminal do VS Code, execute: `docker volume create banco` e `docker volume create site`. Certifique-se de que o Docker Desktop esteja ativo para rodar estes comandos.

>**Observação:** os volumes criados no Windows, são encontrados no caminho \\\wsl$\docker-desktop-data\data\docker\volumes. Eles podem ser acessados da seguinte maneira: 
>>![image](https://user-images.githubusercontent.com/62852333/196316460-3e359a90-7c2d-437f-bebd-067926f1d421.png)  
  
* No diretório onde está o arquivo *docker-compose.yml*, suba a aplicação com o seguinte comando `docker compose up`;
* No navegador, acesse a página *localhost*;
* Selecione o idioma do wordpress;
* Insira usuário, senha e email do usuário administrador da página;


> ## Ubuntu



Antes de subir os containers, é necessário criar um Docker Volume chamado 'banco', para o MySQL, e outro chamado 'site', para o WordPress.
