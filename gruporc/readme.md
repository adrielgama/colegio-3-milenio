# Documentação GLPI - Ramiro Campelo

> O objetivo geral dessa documentação é apresentação básica do uso do sistema para o Suporte Técnico.


![](https://glpi-project.org/wp-content/uploads/2017/03/logo-glpi-bleu-1.png)    ![](https://raw.githubusercontent.com/adrielgama/colegio-3-milenio/master/gruporc/gruporc_logo_400.png)


![](https://img.shields.io/badge/project-OpenSource-blue) ![](https://img.shields.io/badge/version-9.5.3-green)  ![](https://img.shields.io/badge/config-ProjetosDTI-sucess)

#
### > Sobre o GLPI
O **GLPI** é uma aplicação de gestão de serviços e gerenciamento de ativos 100% web. Foi prioritariamente desenvolvida para atender às necessidades de Gestores de TI no gerenciamento de chamados de Helpdesk e transformou-se numa poderosa plataforma de gerenciamento de ativos e serviços, provendo aos gestores informações “on time” de seus recursos físicos e humanos.

### > Principais Funcionalidades
- 100% online;
- Sistema de abertura, acompanhamento e notificação de chamados por e-mail;
- Sistema de notificação de abertura e fechamento de chamados pelo Telegram;
- Projeto OpenSource;
- Catálogo de serviços;
- Gestão de níveis de serviço (SLAs e OLAs);
- Catálogo de serviços;
- Relatórios com gráficos;
- Acompanhamento gráfico de chamados;
- Integração com OCS Inventory NG.
#

### Sumário
<!-- toc -->
* [Página Inicial](#página-inicial)
	* [Login](#login)

<!-- toc stop -->

# Página Inicial 
Para fazer o acesso ao GLPI o usuário deverá acessar digitando IP [http://10.99.2.7/](http://10.99.2.7/) em seu navegador.

## Login:
Ao fazer o acesso o usuário terá até três opções de login:

![](https://i.ibb.co/SNJ0h70/01Login.png)

 1. Banco de dados interno do GLPI
	> Uso exclusivo do administrador do sistema
 2.  **GUAIBIM** *(acesso padrão)*
	 > Usado por todos os usuários com seu login GEMCO
 4. Login por E-mail.
	 > Para quem não possui usuário GEMCO.

# Início GLPI
Atualmente temos dois exemplos de página inicial, separadas por grupos, sendo eles o grupo **Administrativo** e **Suporte**, e o grupo para usuários **Padrão**, com uma diferença de interface de uso e tópicos para abertura de chamados.

### Interface Padrão:
![Interface Padrão](https://i.ibb.co/qBxLpmF/02Home1.png)

Esta interface oferece o método de abertura de chamados por meio de formulários integrados com próprio GLPI, facilitando a abertura de chamados por categoria ou dúvidas do usuário de forma mais interativa, também possibilitando a abertura de chamados de forma livre, porém seguindo critérios pré-estabelecidos para que possa ser feito acompanhamento integral pelo técnico ou supervisor que for atribuído à requisição. 
#
### Interface Administrativa e Suporte
![Interface Administrativa](https://i.ibb.co/pPntZ9S/03HomeN1.png)

A interface administrativa ou de suporte tem um diferencial por já ser mais direta aos chamados criados ou atribuídos ao técnico em questão. Nele também podemos ter um melhor acompanhamento dos chamados, criar novos, efetuar configurações de acordo ao seu nível, gerar relatórios e acompanhar informações por meios de gráficos e um *dashboard* interativo.

# Chamados

Na interface de chamados observamos diversos tópicos, nos dando a possibilidade de acompanhar chamados em todas as suas fases, desde abertura até o fechamento, utilizando os filtros de pesquisa, que por padrão só mostram chamados ainda não solucionados.

![Interface Chamados](https://i.ibb.co/xYQJ5Sz/04-Home-Chamados.png)

Para criar um novo chamado o técnico deverá acessar o menu **`Assistência > Criar chamado`**, ou utilizar o botão **`+`** ao lado do nome *`Chamados`* como na imagem abaixo:

![Criar novo chamado](https://i.ibb.co/Br46RTH/08-New-Ticket.png)

Em seguida será direcionado para página em que deve **atentar-se aos campos obrigatórios** de preenchimento para que a abertura do chamado seja concretizada.

![Criar um chamado](https://i.ibb.co/bWypDrN/06-Abrir-Chamado-Por-Tecnico.png)

Assim que finalizar abertura do chamado, retornando a tela inicial em **`Assistência`**.

Para ter acesso a mais informações sobre qualquer chamado, o técnico deverá selecionar clicando no seu  **Título** 

Ao acessar o chamado o técnico irá se deparar com a tela a seguir: 
> *Caso apareça a tela da imagem de acompanhamento de chamado, técnico deverá clicar na seção **`Chamado`** destacado ao lado*

![Criar novo chamado](https://i.ibb.co/rs54c07/07-Chamado.png)

Aqui o técnico poderá atribuir o chamado para si ou algum outro usuário, fazer alterações e atualizações na configuração do chamado caso tenha necessidade. Se não houver alterações a fazer, poderá prosseguir para página de acompanhamento do chamado.

![Tela de acompanhamento do chamado](https://i.ibb.co/bHJFzbM/05-Novo-Chamado-Inicial.png)

Esta é a tela de acompanhamento do chamado, que deverá ser utilizada para fazer atualizações pertinentes ao status do atendimento, mantendo informado qualquer técnico, observador ou autor que esteja em acompanhamento do mesmo, solicitar aprovação de solução para um superior ou aplicar uma solução para o chamado.

Para adicionar um novo acompanhamento ao chamado basta clicar no botão **`Acompanhamento`** e adicionar sua descrição, após isso apenas clicar em **`Adicionar`** que seu acompanhamento será enviado, junto com uma notificação para o e-mail do autor, caso este tenha um e-mail cadastrado em sua conta.

![Acompanhamento de chamado](https://i.ibb.co/QNSDGWP/09-Acompanhamento.png)

