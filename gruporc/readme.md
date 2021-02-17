# Documentação GLPI - Ramiro Campelo

> O objetivo geral dessa documentação é apresentação básica do uso do sistema para o Suporte Técnico.


![](https://glpi-project.org/wp-content/uploads/2017/03/logo-glpi-bleu-1.png)    ![](https://raw.githubusercontent.com/adrielgama/colegio-3-milenio/master/gruporc/gruporc_logo_400.png)


![](https://img.shields.io/badge/project-OpenSource-blue) ![](https://img.shields.io/badge/glpi_version-9.5.3-ffea00)  ![](https://img.shields.io/badge/custom-Projetos_DTI-sucess) ![](https://img.shields.io/badge/doc_version-1.0-orange)

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
* [Início GLPI](#início-gpli)
 	* [Interface Padrão](#interface-padrão)
	* [Interface Administrativa e Suporte](#interface-administrativa-e-suporte)
* [Chamados](#chamados)
	* [Abertura de chamado](#abertura-de-chamado)
	* [Acompanhamento de chamado](#acompanhamento-de-chamado)
	* [Solução do chamado](#solução-do-chamado)
	* [Aprovação do chamado](#aprovação-do-chamado)
	* [Reabrindo chamado](#reabrindo-chamado)
	* [Clonando chamados](#clonando-chamados)
	* [Abertura de chamado por e-mail](#abertura-de-chamado-por-e-mail)
* [Dashboard](#dashboard)

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

## Abertura de chamado
Para criar um novo chamado o técnico deverá acessar o menu **`Assistência > Criar chamado`**, ou utilizar o botão **`+`** ao lado do nome *`Chamados`* como na imagem abaixo:

![Criar novo chamado](https://i.ibb.co/Br46RTH/08-New-Ticket.png)

Em seguida será direcionado para página em que deve **atentar-se aos campos obrigatórios** de preenchimento para que a abertura do chamado seja concretizada.

![Criar um chamado](https://i.ibb.co/bWypDrN/06-Abrir-Chamado-Por-Tecnico.png)

Assim que finalizar abertura do chamado, retornando a tela inicial em **`Assistência`**.

Para ter acesso a mais informações sobre qualquer chamado, o técnico deverá selecionar clicando no seu  **Título** 

Ao acessar o chamado o técnico irá se deparar com a tela a seguir: 
> *Caso apareça a tela da imagem de acompanhamento de chamado, técnico deverá clicar na seção **`Chamado`** destacado ao lado*

Aqui o técnico poderá atribuir o chamado para si ou algum outro usuário, fazer alterações e atualizações na configuração do chamado caso tenha necessidade. Se não houver alterações a fazer, poderá prosseguir para página de acompanhamento do chamado.

![Criar novo chamado](https://i.ibb.co/rs54c07/07-Chamado.png)

## Acompanhamento de chamado
Abaixo a tela de acompanhamento do chamado, que deverá ser utilizada para fazer atualizações pertinentes ao status do atendimento, mantendo informado qualquer técnico, observador ou autor que esteja em acompanhamento, solicitar aprovação de solução para um superior quando necessário, ou aplicar uma solução para o chamado.

![Tela de acompanhamento do chamado](https://i.ibb.co/bHJFzbM/05-Novo-Chamado-Inicial.png)


Para adicionar um novo acompanhamento ao chamado basta clicar no botão **`Acompanhamento`** e adicionar sua descrição, após isso apenas clicar em **`Adicionar`** que seu acompanhamento será enviado, junto com uma notificação para o e-mail do autor, caso este tenha um e-mail cadastrado em sua conta.

![Acompanhamento de chamado](https://i.ibb.co/QNSDGWP/09-Acompanhamento.png)

## Solução do chamado

Ao executar a tarefa de **`Solução`** temos acesso à alguns modelos já pré-definidos de solução, juntamente com o tipo da solução, facilitando a resposta dos chamados.

![Solução Chamado](https://i.ibb.co/PFX3GCk/10-Modelo-Solucao.png)

![Solução Chamado 2](https://i.ibb.co/L6WCLBy/11-Solucao-Chamado.png)

## Aprovação do chamado

Ao enviar o formulário o chamado constará como modo `Solucionado`, aguardando que o autor do chamado aprove a solução enviada pelo técnico.
> Caso quem tenha feito a abertura do chamado e aplicado modelo de solução tenha sido o próprio técnico, ele mesmo poderá fazer a aprovação da solução.

![Aguardando Aprovação AUTOR](https://i.ibb.co/LvCLhGT/12-Tela-Aprovacao-Autor.png)

 Após aprovação, o status é alterado para **`Fechado`** e o chamado dá como encerrado. Caso a aprovação seja recusada, o chamado terá o do botão de solução disponível aguardando uma nova atualização para que seja feito os passos até o fechamento total do chamado.
 
## Reabrindo chamado
O GLPI também dispõe de reabertura de chamado, que pode ocorrer por uma solução aprovada apresentar falha futura, evitando a abertura de uma nova assistência, o chamado pode ser reaberto e feito novo acompanhamento até sua [solução](#solução-do-chamado).

Basta o usuário acessar o chamado fechado, ir na aba `Chamado` e clicar em **`Reabrir`**.
![Reabrir chamado fechado](https://i.ibb.co/t33hNpV/13-Reabrir-Chamado.png)


## Clonando chamados
Para clonar/duplicar o chamado, basta que o técnico selecione o chamado desejado, e acessar botão  `Ações > Clonar` escolha a quantidade de cópias necessárias para o chamado. 

![Clonar Chamado GIF](https://i.ibb.co/KVKXHR8/Clonar-Chamado-GIF.gif)

## Abertura de chamado por e-mail

Uma das novas funcionalidades é abertura de chamado utilizando o e-mail. Para isso o usuário precisa ter um endereço de e-mail válido cadastrado em nosso sistema, seja ele vinculado ao perfil [GUAIBIM](#login) ou [Login por e-mail](#login). 

Basta que o usuário envie um e-mail para ti.chamados@lojasguaibim.com.br com 
`Assunto` *(que será o título do chamado)*, e `Corpo` *(que será a descrição)*. 
> Preferencialmente todo chamado, seja aberto ou respondido pelo e-mail em forma de acompanhamento, **deve ser removido todo o corpo de assinatura**, para facilitar o uso da aplicação e também o acompanhamento das notificações que chegarão por e-mail, para não deixar uma aparência poluída.

![Abrindo chamado por email](https://i.ibb.co/NmpJRbD/New-Ticket-Mail-GIF.gif)

# Dashboard

O painel de controle é acessado na aba **`Plug-ins > Painel`**. 

![Dashboard](https://i.ibb.co/tCy3Qjj/14-Dashboard-Tec.png)

Nele o técnico tem acesso ao seu histórico de chamados em um determinado período. O histórico é apresentado em formato de gráficos com informações como quantidade de chamados atendidos, chamados atribuídos, tempo de solução dos chamados e até mesmo sua pontuação na pesquisa de satisfação, um painel completo sobre um resumo do técnico.

![Dashboard Tec](https://i.ibb.co/JCKL59S/15-Dash-Painel.png)

