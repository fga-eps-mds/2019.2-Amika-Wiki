# Especificação dos Casos de Uso

## 1. Introdução

## 2. Metodologia

## 3. Relação de Casos de Uso Abordados

ID <a name="table"></a>| Título
-- | --
[UC01](#UC01) | Gerenciar Alunos
[UC02](#UC02) | Manter Turma
[UC03](#UC03) | Auto Gerenciar Matrícula 
[UC04](#UC04) | Manter Grupo
[UC05](#UC05) | Visualizar Perfil
[UC06](#UC06) | Adicionar Humor do Dia
[UC07](#UC07) | Visualizar Dashboard dos Grupos
[UC08](#UC08) | Visualizar Gráfico de Humor da Turma
[UC09](#UC09) | Mandar Notificação Push
[UC10](#UC10) | Manter Agendas da Felicidade
[UC11](#UC11) | Realizar Agendas da Falicidade
[UC12](#UC12) | Compartilhar Agenda
[UC13](#UC13) | Avaliar Agenda
[UC14](#UC14) | Adicionar Recepção da Semana
[UC15](#UC15) | Realizar Atividades do Produto Final de Felicidade
[UC16](#UC16) | Manter Enquete
[UC17](#UC17) | Manter Thread
[UC18](#UC18) | Manter Mural
[UC19](#UC19) | Visualizar Informações de Atendimento Psicológico 
[UC20](#UC20) | Manter Materiais
[UC21](#UC21) | Manter Músico
[UC22](#UC22) | Manter Banda
[UC23](#UC23) | Adicionar Cronograma Happy And Roll

## 4. Especificação

## [UC01](#table) - Gerenciar Aluno <a name="UC01"></a>

### Breve Descrição
- O professor que administra o sistema deve ter a opção de cadastrar o aluno.

### Ator Principal
- Administrador.

### Condições Prévias
- Existir no sistema as entidades professor e aluno.

### Fluxo de Eventos
#### Fluxo Básico
- O professor clica no icone de registrar aluno, na página de admin.
- O professor preenche os dados do aluno a se registrar.

### Condições Posteriores
- Ficara registrado no sistema um novo aluno.


## [UC02](#table) - Manter turma <a name="UC02"></a> 

### Breve Descrição
- O professor que administra o sistema deve ter a opção de cadastrar uma turma e fazer as devidas alterações em turmas já existentes, assim como excluir uma turma do sistema.

### Ator Principal
- Administrador.

### Condições Prévias
- Existir no sistema as entidades professor e turmas.

### Fluxo de Eventos
#### Fluxo Básico
- O professor clica no icone de manter turma, na página de admin.
- O professor preenche os dados da turma a se registrar.
- O professor clica no ícone de excluir turma.
- O professor clica no ícone de alterar dados de uma determinada turma.

### Condições Posteriores
- Ficará registrado no sistema uma nova turma.
- Ficará excluida do sistema uma turma antes existente. 
- Ficarão alterados os dados de uma turma já existente.


## [UC03](#table) - Auto Gerenciar Matrícula <a name="UC03"></a> 

### Breve Descrição
- O aluno deve ter a opção de fazer o próprio cadastro no sistema.

### Ator Principal
- Aluno usuário.

### Condições Prévias
- Deve estar no sistema a entidade aluno.

### Fluxo de Eventos
#### Fluxo Básico
- O aluno clica em cadastrar na página inicial da aplicação.
- O aluno preenche os dados requeridos.
- O aluno clica em matricular.

### 3.4 Condições Posteriores
- Vai estar cadastrado no sistema um novo usuário aluno.


## [UC04](#table) - Manter Grupo <a name="UC04"></a> 

### Breve Descrição
- O usuário aluno terá como fazer o registro e alterar os dados do grupo em que participa.

### Ator Principal
- Aluno usuário.

### Condições Prévias
- Deve estar no sistema a entidade aluno.
- Deve estar no sistema a entidade grupo.

### Fluxo de Eventos
#### Fluxo Básico
- O usuário aluno clica no ícone de seu grupo.
- O aluno preenche os dados requeridos.
- O aluno clica em salvar as alterações feitas.

### Condições Posteriores
- Ficará registrado no sistema um novo aluno em um grupo.
- Ficará excluido do sistema um aluno de grupo existente. 
- ficarão alterados os dados de um grupo já existente.


## [UC05](#table) - Visualizar Perfil <a name="UC05"></a> 

### Breve Descrição
- Usuário deseja visualizar informações sobre o seu perfil, como: pontuação no índice de felicidade autêntica, total de pontos, informações básicas do usuário, etc.

### Ator Principal
- Usuário aluno.

### Condições Prévias
- O usuário deve ter vínculo com a instituição.
- O usuário deve estar logado.

### Fluxo de Eventos
- O usuário irá visualizar o status atual de seus dados de perfil
#### Fluxo Básico
O fluxo básico é composto de passos que o usuário seguirá para poder visualizar seus dados.
- O usuário faz login no sistema
- O usuário clica em perfil
- O caso de uso encerra

### Condições Posteriores
- Visualização dos dados com sucesso.


## [UC06](#table) - Adicionar Humor do Dia <a name="UC06"></a> 

### Breve Descrição
- Essa funcionalidade oferece uma lista de emojis para que o usuário selecione apenas um  e dessa maneira o sistema classifica o humor que o ele está vivenciando no dia. 

### Ator Principal
- Usuário aluno.

### Condições Prévias
- O usuário deve estar logado no sistema
- O usuário deve ter vínculo com a instituição.
- O usuário ainda não pode ter selecionado um humor para aquele dia

### Fluxo de Eventos
- O usuário irá selecionar o emoji que mais se aproxima do humor que ele está passando naquele dia.
#### Fluxo Básico
Esse fluxo se inicia quando o usuário deseja registrar o seu humor referente ao dia atual.
- O usuário acessa o perfil.
- O usuário então acessa o humor do dia.
- O usuário escolhe um dos emojis.
#### Fluxo Alternativo
Esse fluxo se inicia quando o usuário ao invés de selecionar um dos emojis clica em "Cancelar".
- O usuário clica em "Cancelar".
- O caso de uso se encerra.

### Condições Posteriores
- Visualizar o gráfico baseado em todos os humores do usuário até o atual dia.
- O caso de uso encerra.

## [UC07](#table) - Visualizar Dashboard dos Grupos <a name="UC07"></a> 

### Breve Descrição
- Essa funcionalidade permite ao administrador visualizar informações de todos os grupos da turma por meio de cards. Cada card contém informações básicas de cada grupo e um link para a página do grupo.

### Ator Principal
- Administrador.

### Condições Prévias
- O administrador deve estar logado no sistema.
- Devem existir grupos cadastrados no sistema.

### Fluxo de Eventos
- O administrador irá ter acesso as informações básicas de cada grupo cadastrado por meio dos cards.
- O administrador pode saber mais sobre cada grupo acessando a página do grupo por meio do link no card.
#### Fluxo Básico
Esse fluxo se inicia quando o administrador deseja ver os dados de todos os grupos ou de apenas um grupo cadastrado.
- O administrador acessa "Grupos"
- O adminstrador acessa "Listar grupos".
- O caso de uso se encerra.
#### Fluxo Alternativo
Esse fluxo se inicia quando o administrador deseja acessar mais informações além das básicas que o card oferece.
- O administrador acessa o link no card.
- O caso de uso se encerra.

### Condições Posteriores
- Visualizar informações básicas de todos os grupos com sucesso.
- Acessar por meio do link do card mais informações sobre o grupo selecionado.


## [UC08](#table) - Visualizar Gráfico de Humor da Turma <a name="UC08"></a> 

### Breve Descrição
- Essa funcionalidade permite ao administrador checar o humor da turma ao longo do tempo por meio de um gráfico que leva em conta cada aluno.

### Ator Principal
- Administrador.

### Condições Prévias
- O administrador deve estar logado.
- Ao menos uma turma deve estar cadastrada no sistema.

### Fluxo de Eventos
- O administrador acessará todas as turmas.
- O administrador terá acesso ao gráfico de humor de cada turma.
#### Fluxo Básico
Esse fluxo se inicia quando o administrador lista turmas e deseja ver humor de determinada turma.
- O administrador acessa "Turmas".
- O administrador então seleciona a turma que deseja ver o gráfico de humor.
- O administrador acessa o gráfico de humor da turma desejada.
- O caso de uso se encerra.

### Condições Posteriores
- Visualização do gráfico de humor da turma.


## [UC09](#table) - Mandar Notificação Push <a name="UC09"></a>

### Breve Descrição
- Essa funcionalidade permite ao administrador mandar notificações aos alunos de uma turma.

### Ator Principal
- Administrador.

### Condições Prévias
- O administrador deve estar logado no sistema.
- Deve existir ao menos uma turma cadastrada no sistema.

### Fluxo de Eventos
- O administrador irá ter acesso às turmas e poderá enviar notificações para os alunos de uma determinada turma.
#### Fluxo Básico
Esse fluxo se inicia quando o administrador deseja enviar uma notificação aos alunos de uma turma.
- O administrador acessa "Turmas".
- O administrador escolhe uma das turmas.
- O administrador digita a mensagem que ele deseja enviar.
- O administrador envia a notificação.
- O caso de uso se encerra.

### Condições Posteriores

## [UC10](#table) - Manter Agendas da Felicidade <a name="UC10"></a>

### Breve descrição
- Essa funcionalidade permite ao administrador criar, editar ou deletar agendas.

### Ator Principal
- Administrador.

### Condições Prévias
- O administrador deve estar logado.

### Fluxo de Eventos
- O administrador criará uma agenda (atividade).
- Os usuários poderão visualizar a agenda.
#### Fluxo Básico
- O administrador acessa "Agendas".
- O administrador cria uma agenda.   
#### Fluxo Alternativo
**[FA01] - Deletar agenda** 
- O administrador acessa "Agendas".
- O administrador visualiza as agendas existentes.
- O administrador escolhe uma agenda.
- O administrador deleta a agenda escolhida.  
**[FA02] - Editar agenda**
- O administrador acessa "Agendas".
- O administrador visualiza as agendas existentes.
- O administrador escolhe uma agenda.
- O administrador edita a agenda escolhida.  

### Condições posteriores
- Visualização da(s) agenda(s) pelos usuários.


## [UC11](#table) - Realizar Agendas da Felicidade <a name="UC11"></a>

### Breve Descrição
- Essa funcionalidade permite ao usuário realizar agendas.

### Ator Principal
- Usuário.

### Condições Prévias
- O usuário deve estar logado.
- Deve existir ao menos uma agenda.

### Fluxo de Eventos
#### Fluxo Básico
- O usuário acessa "Agendas".
- O usuário escolhe uma agenda.   
- O usuário envia a resposta da agenda.

### Condições Posteriores
- Visualização da resposta pelo administrador.


## [UC12](#table) - Compartilhar Agenda <a name="UC12"></a>

### Breve Descrição
- Essa funcionalidade permite ao usuário compartilhar sua agenda pessoal semanal com seus colegas de turma.

### Ator Principal
- Usuário.

### Condições Prévias
- O usuário deve estar logado.

### Fluxo de Eventos
- O usuário compartilha sua agenda semanal de atividades com seus colegas.
- A agenda do aluno estará disponível para que a visualização seja possível por outros alunos. 
#### Fluxo Básico
- O usuário acessa "Agenda pessoal".
- O usuário compartilha suas atividades semanais.
- O a agenda semanal do usuário se torna disponível para a visualização por outros usuários.
- O caso de uso se encerra.

### 12.4 Condições Posteriores
- A agenda semanal do usuário é compartilhada com seus colegas de turma.


## [UC13](#table) - Avaliar Agenda <a name="UC13"></a>

### Breve Descrição
- Esta funcionalidade permite ao usuário avaliar as atividades que foram passadas, com objetivo de avaliar quais foram as mais interessantes de se realizar.

### Ator Principal
- Usuário.

### Condições Prévias
- O usuário deve estar logado.
- Atividades devem ter sido realizadas para que o usuário possa avaliá-las.

### Fluxo de Eventos
- O usuário, logado, avalia (1 a 5 estrelas) atividades já realizadas de acordo com seu nível de satisfação com aquela atividade.
- O administrador tem acesso às avaliações feitas pelos alunos, e assim tem controle sobre os tipos de atividades que mais satisfazem os alunos.
#### Fluxo Básico
- O usuário acessa "Atividades" e seleciona uma atividade já realizada.
- O usuário avalia essa atividade de 1 a 5 estrelas, de acordo com seu nível de satisfação com esta atividade.
- O administrador tem acesso a todas as avaliações feitas, tendo, assim, controle sobre os tipos de atividade que mais satisfazem os alunos.
- O caso de uso se encerra.

### Condições Posteriores
- O administrador poderá visualizar as atividades mais interessantes de se realizar, comparando a avaliação de cada tipo de atividade.


## [UC14](#table) - Adicionar Recepção da Semana <a name="UC14"></a>

### Breve Descrição
- Essa funcionalidade permite aos alunos adicionar um evento chamado "recepção" com o objetivo de informar ao professor sobre atividades realizadas nessa recepção. As recepções são eventos que ocorrem

### Ator Principal
- Usuário.

### Condições Prévias
- O usuário deve estar logado.

### Fluxo de Eventos
- O usuário cria uma recepção com atividades a serem realizadas.
- A partir disso, o administrador pode ver e controlar as atividades realizadas nas recepções.
#### Fluxo Básico
- O usuário cria uma recepção e adiciona as atividades a serem realizadas na recepção.
- O administrador poderá, então, visualizar e controlar a recepção.
- O caso de uso se encerra.

### Condições Posteriores
- O administrador terá visualização completa e controle sobre as atividades realizadas nas recepções.


## [UC15](#table) - Realizar Atividades do Produto Final de Felicidade <a name="UC15"></a>

### Breve Descrição
- Essa funcionalidade permite ao usuário realizar atividades do produto final da disciplina e ao professor acompanhar o adamento do mesmo.

### Ator Principal
- Usuário.

### Condições Prévias
- O usuário deve estar logado.

### Fluxo de Eventos
- O usuário envia suas atividades ao decorrer do semestre.
- O administrador terá acesso ao informativo em formato de linha do tempo quanto ao andamento do projeto.
#### Fluxo Básico
- O usuário acessa "Atividades".
- O usuário seleciona o arquivo que deseja enviar e cria uma descrição.
- O usuário então envia a atividade desejada.
- O professor acessa a linha do tempo de atividades daquele usuário.
- O caso de uso se encerra.

### Condições Posteriores
- Visualização do andamento do produto final da disciplina.


## [UC16](#table) - Manter Enquete <a name="UC16"></a>

### Breve Descrição
- Essa funcionalidade permite ao administrador criar enquetes para votação rápida através do aplicativo e deixá-las prontas para edição, visualização e votação

### Atores Principais
- Administrador e Usuário.

### Condições Prévias
- O administrador deve estar logado.
- Turma deve estar criada.

### Fluxo de Eventos
- O administrador criará uma enquete para a turma selecionada.
- Os usuários irão votar na enquete.
- O administrador terá acesso ao resultado da enquete criada.

#### Fluxo Básico
#### [FB01] - Criação e votação de enquete <a name="FB01enquete"></a>
- O administrador acessa "Mural".
- O administrador então seleciona a opção "Criar enquete".
- O administrador informa os dados da enquete a ser criada.
- O administrador clica na opção de criar a enquete.
- Os usuários acessam "Mural".
- Os usuários escolhem o seu voto.
- O administrador visualiza os resultados da enquete.
- O caso de uso se encerra.

#### Fluxo Alternativo
#### [FA01] - Deletar enquete <a name="FA01enquete"></a>
O caso de uso começa quando o administrador deseja editar uma enquete criada previamente
- O administrador acessa "Mural".
- O administrador visualiza as enquetes existentes.
- O administrador seleciona a opção de deletar a enquete de sua escolha.
- A enquete é deletada
#### [FA02] - Editar enquete <a name="FA02enquete"></a>
O caso de uso começa quando o administrador deseja editar uma enquete criada previamente
- O administrador acessa "Mural".
- O administrador visualiza as enquetes existentes.
- O administrador seleciona a opção de editar a enquete de sua escolha.
- O administrador edita a enquete.

### Condições Posteriores
- Em [FB01](#FB01enquete) O sistema deve disponibilizar a visualização dos resultados da enquete.
- Em [FA01](#FA01enquete) O sistema deverá deletar a enquete selecionada e exibir uma mensagem informando que a enquete foi deletada
- Em [FA02](#FA02enquete) O sistema deverá alterar os dados da enquete e exibir uma mensagem informando que a enquete foi editada

## [UC17](#table) - Manter Thread <a name="UC17"></a>

### Breve Descrição
- Essa funcionalidade permite aos usuários comentar os tópicos criados por outros usuários ou administradores no Mural.

### Ator Principal
- Usuário.

### Condições Prévias
- O usuário deve estar logado.
- Tópico deve estar criado no mural.

### Fluxo de Eventos
- Um usuário criará um tópico para discussão.
- Outros usuários criarão comentários naquele tópico
#### Fluxo Básico
#### [FB01] - Criar Thread em um tópico<a name="FB01thread"></a>
O caso de uso começa quando um usuário resolve criar uma thread em um tópico criado previamente
- O usuário acessa "Mural".
- O usuário cria um tópico a ser discutido.
- Outro usuário acessa "Mural".
- O outro usuário vê o tópico criado e seleciona a opção "Comentar".
- O outro usuário cria seu comentário e salva.
- Os usuários poderão visualizar os comentários criados nos tópicos do mural.
- O caso de uso se encerra.

#### Fluxo Alternativo
#### [FA01] - Deletar Thread <a name="FA01thread"></a>
O caso de uso começa quando o usuário deseja deletar uma thread de sua autoria criada previamente 
- O usuário acessa "Mural".
- O usuário visualiza os tópicos existentes.
- O usuário acessa um dos tópicos.
- O usuário acessa a thread de sua criação.
- O usuário seleciona a opção de deletar a thread.  
#### [FA02] - Editar Informações da Banda <a name="FA02thread"></a>
O caso de uso começa quando o usuário editar uma thread de sua autoria criada previamente 
- O usuário acessa "Mural".
- O usuário visualiza os tópicos existentes.
- O usuário acessa um dos tópicos.
- O usuário acessa a thread de sua criação.
- O usuário seleciona a opção de edit a thread.
- O usuário edita a thread.

### Condições Posteriores
- Em [FB01](#FB01thread) o sistema deverá disponibilizar a visualização da thread para todos os usuários.
- Em [FA01](#FA01thread) o sistema deverá deletar a thread selecionada e mostrar uma mensagem informando que a thread foi deletada.
- Em [FA02](#FA02thread) o sistema deverá editar a thread selecionada e mostrar uma mensagem informando que a thread foi editada.

## [UC18](#table) - Manter Mural <a name="UC18"></a>

### Breve Descrição
- Consiste em criar um canal de comunicação dinâmico entre os alunos e o professor, criando algo similar a um mural, a onde o aluno entrará e poderá ver as atividades propostas pelo o professor.

### Ator Principal
- Administrador.

### Condições Prévias
- O aluno deve estar cadastrado e logado.

### Fluxo de Eventos
#### Fluxo Básico
O fluxo básico se inicia no momento que o professor adicionar alguma atividade no mural.
- O professor acessar a página do mural.
- O professor seleciona a opção de criar uma atividade.
- O professor especifica como será a atividade é posta ela.
#### Fluxo Alternativo
O fluxo alternativo irá se iniciar quando o aluno acessar a página do mural.
- O aluno acessar a página do mural.
- O aluno seleciona a atividade desejada.
- O aluno tem acesso como será feita tal atividade e seus requisitos

### Condições Posteriores
- O aluno e o professor terá acesso a todas atividades propostas, e o professor terá a possibilidades de criar outras.

## [UC19](#table) - Visualizar Informações de Atendimento Psicológico <a name="UC19"></a>

### Breve Descrição
- Criar uma área informativa, a onde o aluno poderá ver procurar ajuda psicologia e outros canais que possa ser de ajuda, contendo números de contato, e-mails e afins, para facilitar o aluno encontrar a ajuda que ele precisa.

### Ator Principal
- Usuário.

#### Condições Prévias
- O aluno deve estar cadastrado e logado.

### Fluxo de Eventos
#### Fluxo Básico
O aluno acessa uma página onde ele pode conseguir a ajuda que precisa.
- O aluno acessa a página de área informativa.
- O aluno escolhe o tipo de ajuda que precisa.
- O aluno tem acesso aos meios de ajuda necessário

### Condições Posteriores
- O aluno terá acesso a todos os meios de ajuda disponível na página.
    
## [UC20](#table) - Manter Materiais <a name="UC20"></a>

### Breve Descrição
- Criar uma área de compartilhamento de material da disciplina, um local onde terá o conteúdo proposto pela a disciplina, o conteúdo que está sendo utilizado na aula, assim facilitando o uso do material para a disciplina.

### Ator Principal
- Administrador.

### 20.4 Condições Prévias
- O aluno deve estar cadastrado e logado.

### Fluxo de Eventos
### Fluxo Básico
O fluxo básico se inicia no momento que o professor adicionar algum conteúdo na área de compartilhamento.
- O professor acessar a página de compartilhamento.
- O professor seleciona a opção de enviar conteúdo.
- O professor escolhe o conteúdo e o envia.
### Fluxo Alternativo
O fluxo alternativo irá se iniciar quando o aluno acessar a página de compartilhamento.
- O aluno acessar a página de compartilhamento.
- O aluno seleciona o conteúdo desejado.
- O aluno tem acesso ao conteúdo desejado.

### Condições Posteriores
- O aluno e o professor terá acesso a todo conteúdo disponível na página, e o professor terá a possibilidades de enviar mais conteúdo.

## [UC21](#table) - Manter Músico <a name="UC21"></a>

### Breve Descrição
- Os usuários que forem participar do evento Happy and Roll devem poder se cadastrar no sistema como músicos.

### Ator Principal
- Usuário.

### Condições Prévias
- Qualquer usuário poderá se cadastrar no evento e visualizar as informações dos músicos já cadastrados, estando este cadastrado ou não na plataforma Amika.
- Para editar seus dados e deletar seu cadastro o músico deve estar previamente cadastrado no sistema.

### Fluxo de Eventos
#### Fluxo Básico
#### [FB01] - Cadastrar Músico no Sistema <a name="FB01musico"></a>
O caso de uso começa quando o usuário resolve se cadastrar como músico para o evento Happy and Roll.
- O usuário acessa o sistema.
- O usuário clica em Happy and Holl.
- O usuário clica em Me Cadastrar Como Músico.
- O usuário insere suas informações.
- O usuário salva as suas informações.
- O caso de uso se encerra.
#### [FB02] - Visualizar Informações dos Músicos <a name="FB02musico"></a>
O caso de uso começa quando o usuário deseja saber as informações a respeito dos músicos já cadastrados para o Happy and Holl.
- O usuário acessa o sistema.
- O usuário clica em Happy and Holl.
- O usuário clica em Músicos Cadastrados.
- O usuário visualiza uma lista com as informações dos músicos cadastrados.
- O caso de uso se encerra.
#### [FB03] - Visualizar Perfil de Músico <a name="FB03musico"></a>
O caso de uso começa quando o usuário deseja visualizar seu perfil como músico.
- O usuário acessa o sistema.
- O usuário clica em Happy and Holl.
- O usuário clica em Acessar como Músico.
- O usuário faz login.
- O usuário visualiza as suas informações de músico.
- O caso de uso se encerra. [[FA01]](#FA01musico) [[FA02]](#FA02musico)

#### Fluxo Alternativo
#### [FA01] - Editar Informações do Músico <a name="FA01musico"></a>
O caso de uso começa quando um músico já cadastrado resolve fazer alguma alteração nos seus dados.
- O usuário clica em Editar Meu Perfil de Músico.
- O usuário altera os dados desejados.
- O usuário salva as alterações.
- O caso de uso se encerra.
#### [FA02] - Deletar Cadastro do Músico <a name="FA02musico"></a>
O caso de uso começa quando um músico já cadastrado resolve excluir seu cadastro.
- O usuário clica em Excluir Meu Perfil de Músico.
- O usuário exclui seus dados do sistema.
- O caso de uso se encerra.

### Condições Posteriores
- Em [FB01](#FB01musico) o sistema deverá mostrar uma mensagem informando que o músico foi cadastrado com sucesso.  
- Em [FB02](#FB02musico) o sistema deverá exibir uma lista com as informações dos músicos que estão cadastrados para o evento.
- Em [FB03](#FB03musico) o sistema deverá exibir as informações do próprio músico. 
- Em [FA01](#FA01musico) o sistema deverá mostrar uma mensagem informando que os dados foram alterados com sucesso. 
- Em [FA02](#FA02musico) o sistema deverá mostrar uma mensagem informando que o músico foi deletado com sucesso e retornar a página inicial do Happy and Holl. 


## [UC22](#table) - Manter Banda <a name="UC22"></a>

### Breve Descrição
- Os usuários que forem participar do evento Happy and Roll devem poder se cadastrar no sistema como uma banda, com o intuito de procurar outros membros para a banda, deixando seu contato para os interessados.

### Ator Principal
- Usuário.

### Condições Prévias
- Qualquer usuário poderá cadastrar uma banda no sistema e visualizar as informações das bandas cadastradas, estando este cadastrado ou não na plataforma Amika.
- Para editar seus dados e deletar seu cadastro a banda do usuário deve estar previamente cadastrada no sistema.

### Fluxo de Eventos
#### Fluxo Básico
#### [FB01] - Cadastrar Bandas no Sistema <a name="FB01banda"></a>
O caso de uso começa quando um usuário resolve cadastrar sua banda para o evento Happy and Holl.
- O usuário acessa o sistema.
- O usuário clica em Happy and Holl.
- O usuário clica em Cadastrar Banda.
- O usuário insere as informações sobre a banda.
- O usuário salva as informações.
- O caso de uso se encerra.
#### [FB02] - Visualizar Informações das Bandas <a name="FB02banda"></a>
O caso de uso começa quando o usuário deseja saber as informações a respeito das bandas já cadastrados para o Happy and Holl.
- O usuário acessa o sistema.
- O usuário clica em Happy and Holl.
- O usuário clica em Bandas Cadastradas.
- O usuário visualiza uma lista com as informações das bandas cadastradas.
- O caso de uso se encerra.
#### [FB03] - Visualizar Perfil de Banda <a name="FB03banda"></a>
O caso de uso começa quando o usuário deseja visualizar seu perfil como banda.
- O usuário acessa o sistema.
- O usuário clica em Happy and Holl.
- O usuário clica em Acessar como Banda.
- O usuário faz login.
- O usuário visualiza as informações de sua banda.
- O caso de uso se encerra. [[FA01]](#FA01banda) [[FA02]](#FA02banda)

#### Fluxo Alternativo
#### [FA01] - Editar Informações da Banda <a name="FA01banda"></a>
O caso de uso começa quando o membro de uma banda já cadastrado resolve fazer alguma alteração nos dados da mesma.
- O usuário clica em Editar Perfil da Banda.
- O usuário altera os dados desejados.
- O usuário salva as alterações.
- O caso de uso se encerra.
#### [FA02] - Deletar Cadastro da Banda  <a name="FA02banda"></a>
O caso de uso começa quando uma banda já cadastrado resolve excluir seu cadastro.
- O usuário clica em Excluir Meu Perfil de Banda.
- O usuário exclui os dados da sua banda do sistema.
- O caso de uso se encerra.

### Condições Posteriores
- Em [FB01](#FB01banda) o sistema deverá mostrar uma mensagem informando que a banda foi cadastrada com sucesso. 
- Em [FB02](#FB02banda) o sistema deverá exibir uma lista com as informações das bandas que estão cadastrados para o evento.
- Em [FB03](#FB03banda) o sistema deverá exibir as informações da própria banda. 
- Em [FA01](#FA01banda) o sistema deverá mostrar uma mensagem informando que os dados da banda foram alterados com sucesso. 
- Em [FA02](#FA02banda) o sistema deverá mostrar uma mensagem informando que a banda foi deletada com sucesso e retornar a página inicial do Happy and Holl. 


## [UC23](#table) - Adiciona Cronograma Happy and Roll <a name="UC23"></a>
 
### Breve Descrição
- O professor que administra o sistema poderá adicionar e editar as informações de um cronograma do evento Happy And Roll.

### Ator Principal
- Administrador.

### Condições Prévias
- O administrador deverá estar logado no sistema.
- Para ser possível a edição, o cronograma deve estar previamente criado.

### Fluxo de Eventos
#### Fluxo Básico
#### [FB01] Adicionar Cronograma Happy and Roll
O caso de uso se inicia quando o professor que administra o sistema decide adicionar as informações do cronograma Happy and Roll.
- O professor loga no sistema.
- O professor clica em Adicionar Cronograma Happy And Roll.
- O professor adiciona as datas e horários em que cada banda ou músico irá se apresentar.
- O professor salva as alterações.
- O caso de uso se encerra.
#### [FB02] Editar Cronograma Happy and Roll
O caso de uso se inicia quando o professor que administra o sistema decide alterar as informações do cronograma Happy and Roll.
- O professor loga no sistema.
- O professor clica em Editar Cronograma Happy And Roll.
- O professor altera os dados desejados.
- O professor salva as alterações.
- O caso de uso se encerra.

### Condições Posteriores
- O cronograma do evento estará disponível para vizualização de todos.
