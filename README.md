Seja Bem-vindo ao repositório FAQ SISCOSERV!
  
* [Tutorial de Manutenção do Conteúdo FAQ](https://github.com/mdicgovbr/pagina-FAQ/blob/master/tutorial-manutencao-FAQ.md)
* [Tutorial de Deploy contínuo no GitHub Pages](https://github.com/mdicgovbr/pagina-FAQ/blob/master/tutorial-publicacao-githubpages.md)

## Rodando localmente

Nesta seção está descrito cada passo necessário para a configuração e utilização da aplicação localmente.

#### Pré-requisitos
  * [Git](https://git-scm.com/)
  * [Docker](https://www.docker.com/get-docker)
  * [Docker-composer](https://docs.docker.com/compose/install/#install-compose)

#### Configuração

Clone o repositório no diretório desejado

	git clone https://github.com/mdicgovbr/pagina-FAQ.git

Utilize o seguinte comando para subir a aplicação

	docker-compose up

A aplicação pode ser acessada através do localhost:

	localhost:4000
