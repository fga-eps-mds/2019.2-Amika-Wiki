# Especificação dos Casos de Uso

## 1. Introdução
O presente documento traz os casos de uso em detalhes, apresentando os fluxos básicos e os fluxos alternativos de cada caso. Expondo descrição, atores envolvidos, condições prévias, fluxos e condições posteriores. Sendo, desse modo, uma forma completa e minunciosa de um modelo tradicional que representa como o sistema Amika funciona. 

#### 1.1. Definições, Acrônimos e Abreviações

**Acrônimo/Abreviação** | **Definição**
------------------------|-------------------
FB | Fluxo Básico
FA | Fluxo Alternativo
UC | Caso de Uso

## 2. Metodologia
Para realizar a elaboração desse documento, a equipe utilizou as histórias de usuário apontadas no [backlog do projeto](https://fga-eps-mds.github.io/2019.2-Amika-Wiki/#/docs/projeto/backlog). Os tópicos foram separados entre os membros, para que todos colaborassem com uma parcela do documento. Os casos de uso que são descritos nesse documento estão listados no tópico abaixo.

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
[UC11](#UC11) | Realizar Agendas da Felicidade
[UC12](#UC12) | Compartilhar Agenda da Felicidade
[UC13](#UC13) | Avaliar Agenda da Felicidade
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

## [UC01](#table) - Gerenciar Alunos <a name="UC01"></a>

### Breve Descrição
- O professor que administra o sistema deve ter a opção de cadastrar um aluno específico, cadastrar lista de alunos por meio de um arquivo CSV e remover aluno.

### Ator Principal
- Administrador.

### Condições Prévias
- O professor deve estar logado no sistema.


### Fluxo de Eventos
#### Fluxo Básico
#### [FB01] Cadastrar Aluno Específico <a name = "fb01gerenciaralunos"></a>
O caso de uso se inicia quando o professor decide cadastrar um novo aluno.
- O professor clica no ícone de Registrar Aluno, na página de admin.
- O professor preenche os dados do aluno a se registrar.
- O professor salva os dados.
- O caso de uso se encerra.

#### [FB02] Cadastrar lista de alunos via CSV <a name = "fb02gerenciaralunos"></a>
O caso de uso se inicia quando o professor decide cadastrar uma lista de alunos retirando seus dados de um arquivo CSV.
- O professor clica no ícone de Registrar Alunos Via CSV.
- O professor envia o arquivo CSV para o sistema.
- O professor salva as alterações.
- O caso de uso se encerra.

#### [FB03] Remover aluno <a name = "fb03gerenciaralunos"></a>
O caso de uso se inicia quando o professor decide deletar um aluno do sistema.
- O professor clica no ícone de Remover Aluno, na página de admin.
- O professor salva a alteração.
- O caso de uso se encerra.

### Condições Posteriores
- Em [FB01](#fb01gerenciaralunos) ficará registrado no sistema um novo aluno.
- Em [FB02](#fb02gerenciaralunos) ficará registrado uma lista de novos alunos no sistema.
- Em [FB03](#fb03gerenciaralunos) um cadastro de aluno estará removido do sistema.


## [UC02](#table) - Manter turma <a name="UC02"></a> 

### Breve Descrição
- O professor que administra o sistema deve ter a opção de cadastrar uma turma e fazer as devidas alterações em turmas já existentes, assim como excluir uma turma do sistema.

### Ator Principal
- Administrador.

### Condições Prévias
- O professor administrador deverá estar logado no sistema.


### Fluxo de Eventos
#### Fluxo Básico

#### [FB01] - Cadastrar Turma no Sistema <a name = "fb01manterturma"></a>
O caso de uso começa quando o professor resolve cadastrar uma turma.
- O professor clica em Turmas.
- O professor insere as informações sobre a nova turma.
- O professor salva as informações.
- O caso de uso se encerra.

#### [FB02] - Visualizar Informações da Turma <a name = "fb02manterturma"></a>
O caso de uso começa quando o professor deseja saber as informações a respeito de uma turma.
- O professor clica em Turmas.
- O professor visualiza uma página com as informações das turmas cadastradas.
- O caso de uso se encerra. [[FA01]](#fa01manterturma) [[FA02]](#fa02manterturma)

#### Fluxo Alternativo
#### [FA01] - Editar Informações das Turmas <a name = "fa01manterturma"></a>
O caso de uso começa quando o professor administrador resolve fazer alguma alteração nos dados das turmas.
- O professor clica em Editar Turmas.
- O professor altera os dados desejados.
- O professor salva as alterações.
- O caso de uso se encerra.

#### [FA02] - Deletar Cadastro de Turma <a name = "fa02manterturma"></a>
O caso de uso começa quando o professor administrador resolve excluir determinada turma.
- O professor clica em Excluir Turma.
- O professor confirma as alterações.
- O caso de uso se encerra.

### Condições Posteriores
- Em [FB01](#fb01manterturma) O sistema deverá registrar uma nova turma.
- Em [FB02](#fb02manterturma) O sistema deverá- mostrar as informações de uma turma determinada. 
- Em [FA01](#fa01manterturma) O sistema deverá registar as alterações feitas em uma turma determinada.
- Em [FA01](#fa02manterturma) O sistema deverá apagar as informações de uma turma determinada.


## [UC03](#table) - Auto Gerenciar Matrícula <a name="UC03"></a> 

### Breve Descrição
- O aluno deve ter a opção de fazer o próprio cadastro no sistema.

### Ator Principal
- Usuário.

### Condições Prévias
- O usuário deve acessar a página do sistema Amika.
- O usuário deve estar previamente matriculado na disciplina Felicidade da Universidade de Brasília.
- A matrícula do usuário deve estar previamente cadastrada no sistema Amika.


### Fluxo de Eventos
#### Fluxo Básico
#### [FB01] Realizar cadastro
O caso de uso se inicia quando o aluno resolve fazer seu cadastro no sistema Amika.
- O aluno clica em Cadastrar na página inicial da aplicação.
- O aluno preenche os dados requeridos.
- O aluno clica em Matricular.
- O caso de uso se encerra.

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

#### [FB01] - Cadastrar Grupo no Sistema
O caso de uso começa quando um usuário resolve cadastrar seu grupo.
- O usuário acessa o sistema.
- O usuário clica em Meu Grupo.
- O usuário clica em Cadastrar Grupo.
- O usuário insere as informações sobre o grupo.
- O usuário salva as informações.
- O caso de uso se encerra.

#### [FB02] - Visualizar Informações do Grupo
O caso de uso começa quando o usuário deseja saber as informações a respeito de seu grupo.
- O usuário acessa o sistema.
- O usuário clica em Meu Grupo.
- O usuário clica em Grupos Cadastradas.
- O usuário visualiza uma página com as informações do grupo em que está cadastrado.
- O caso de uso se encerra.

#### Fluxo Alternativo
#### [FA01] - Editar Informações do Grupo
O caso de uso começa quando um usuário já cadastrado resolve fazer alguma alteração nos dados de seu grupo.
- O usuário acessa o sistema.
- O usuário clica em Meu Grupo.
- O usuário clica em Editar Grupo.
- O usuário altera os dados desejados.
- O usuário salva as alterações.
- O caso de uso se encerra.

#### [FA02] - Deletar Cadastro do Grupo 
O caso de uso começa quando um aluno já cadastrado resolve excluir seu grupo.
- O usuário acessa o sistema.
- O usuário clica em Meu Grupo.
- O usuário clica em Editar Grupo.
- O usuário clica em Excluir Grupo.
- O usuário exclui os dados de seu grupo do sistema.
- O caso de uso se encerra.

### Condições Posteriores
- Em [FB01] O sistema deverá registrar um novo grupo.
- Em [FB02] O sistema deverá- mostrar as informações do grupo determinado. 
- Em [FA01] O sistema deverá registar as alterações feitas no grupo determinado.
- Em [FA01] O sistema deverá apagar as informações do grupo determinado.

## [UC05](#table) - Visualizar Perfil <a name="UC05"></a> 

### Breve Descrição
- Usuário deseja visualizar informações sobre o seu perfil, como: pontuação no índice de felicidade autêntica, total de pontos, informações básicas do usuário, etc.

### Ator Principal
- Usuário.

### Condições Prévias
- O usuário deve estar logado.


### Fluxo de Eventos
#### Fluxo Básico
#### [FB01] Visualizar dados do próprio perfil
O caso de uso se inicia quando o usuário deseja visualizar as informações de seu perfil.
- O usuário faz login no sistema
- O usuário clica em Perfil
- O caso de uso encerra

### Condições Posteriores
- Visualização dos dados com sucesso.


## [UC06](#table) - Adicionar Humor do Dia <a name="UC06"></a> 

### Breve Descrição
- Essa funcionalidade oferece uma lista de emojis para que o usuário selecione apenas um  e dessa maneira o sistema classifica o humor que o ele está vivenciando no dia. 

### Ator Principal
- Usuário.

### Condições Prévias
- O usuário deve estar logado no sistema.
- O usuário ainda não pode ter selecionado um humor para aquele dia.


### Fluxo de Eventos
#### Fluxo Básico
#### [FB01] Registrar Humor do Dia
O caso de uso se inicia quando o usuário deseja registrar o seu humor referente ao dia atual.
- O usuário acessa o Perfil.
- O usuário então acessa o Humor do Dia.
- O usuário escolhe um dos emojis. [FA01](#fa01humordodia)
- O caso de uso se encerra.
#### Fluxo Alternativo 
#### [FA01] Cancelar Ação <a name="fa01humordodia"></a>
O caso de uso se inicia quando o usuário ao invés de selecionar um dos emojis clica em Cancelar.
- O usuário clica em Cancelar.
- O caso de uso se encerra.

### Condições Posteriores
- Possibilidade de visualizar o gráfico baseado em todos os humores do usuário até o atual dia.

## [UC07](#table) - Visualizar Dashboard dos Grupos <a name="UC07"></a> 

### Breve Descrição
- Essa funcionalidade permite ao administrador visualizar informações de todos os grupos da turma por meio de cards. Cada card contém informações básicas de cada grupo e um link para a página do grupo.

### Ator Principal
- Administrador.

### Condições Prévias
- O administrador deve estar logado no sistema.
- Devem existir grupos cadastrados no sistema.


### Fluxo de Eventos
#### Fluxo Básico
#### [FB01] Visualizar Lista de Grupos Cadastrados
O caso de uso se inicia quando o administrador deseja ver os dados de todos os grupos ou de apenas um grupo cadastrado.
- O administrador acessa Grupos.
- O adminstrador acessa Listar grupos.
- O caso de uso se encerra. [FA01](#fa01dashboardgrupos)
#### Fluxo Alternativo
#### [FA01] Visualizar Dados de Um Grupo Específico <a name="fa01dashboardgrupos"></a>
O caso de uso se inicia quando o administrador deseja acessar mais informações além das básicas que o card oferece.
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
#### Fluxo Básico
#### [FB01] Visualizar Gráfico de Humor
O caso de uso se inicia quando o administrador deseja ver humor de determinada turma.
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
#### Fluxo Básico
#### [FB01] Enviar Notificação
O caso de uso se inicia quando o administrador deseja enviar uma notificação aos alunos de uma turma.
- O administrador acessa Turmas.
- O administrador escolhe uma das turmas.
- O administrador digita a mensagem que ele deseja enviar.
- O administrador envia a notificação.
- O caso de uso se encerra.

### Condições Posteriores
- Os usuários cadastrados na turma recebem a notificação.


## [UC10](#table) - Manter Agendas da Felicidade <a name="UC10"></a>

### Breve descrição
- Essa funcionalidade permite ao administrador criar, visualizar, editar ou deletar Agendas da Felicidade, que são atividades que devem ser realizadas pelos alunos ao longo do semestre.

### Ator Principal
- Administrador.

### Condições Prévias
- O administrador deve estar logado.


### Fluxo de Eventos
#### Fluxo Básico
#### [FB01] Adicionar Agendas da Felicidade
O caso de uso se inicia quando o professor que administra o sistema resolve adicionar uma Agenda da Felicidade.
- O administrador acessa Agendas.
- O administrador adiciona as informações da Agenda.
- O caso de uso se encerra.

#### [FB02] Visualizar Agendas da Felicidade
O caso de uso se inicia quando o professor que administra o sistema decide visualizar as informações de uma Agenda da Felicidade já criada.
- O administrador acessa Agendas.
- O administrador visualiza as agendas existentes.
- O administrador clica na Agenda desejada.
- O administrador visualiza o conteúdo desejado.
- O caso de uso se encerra. [[FA01]](#fa01agendadafelicidade) [[FA02]](#fa02agendadafelicidade)

#### Fluxo Alternativo
#### [FA01] - Deletar Agenda da Felicidade <a name="fa01agendadafelicidade"></a>
O caso de uso se inicia quando o professor resolve deletar alguma Agenda.
- O administrador deleta a agenda escolhida.  
- As alterações são salvas.
- O caso de uso se encerra.

#### [FA02] - Editar Agenda da Felicidade <a name="fa02agendadafelicidade"></a>
O caso de uso se inicia quando o professor resolve editar alguma Agenda.
- O administrador edita a agenda escolhida.  
- As alterações são salvas.
- O caso de uso se encerra.

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
#### [FB01] Realizar Agenda
O caso de uso se inicia quando o usuário deseja realizar uma Agenda da Felicidade. 
- O usuário acessa Agendas.
- O usuário escolhe uma Agenda.   
- O usuário envia a resposta da agenda.
- O caso de uso se encerra.

### Condições Posteriores
- Visualização da resposta pelo administrador.


## [UC12](#table) - Compartilhar Agenda da Felicidade<a name="UC12"></a>

### Breve Descrição
- Essa funcionalidade permite ao usuário compartilhar sua agenda pessoal semanal com seus colegas de turma.

### Ator Principal
- Usuário.

### Condições Prévias
- O usuário deve estar logado.


### Fluxo de Eventos
#### Fluxo Básico
#### [FB01] Compartilhar Agenda
O caso de uso se inicia quando o usuário resolve compartilhar sua agenda semanal de atividades com seus colegas.
- O usuário acessa Agenda Pessoal.
- O usuário compartilha suas atividades semanais.
- A agenda semanal do usuário é compartilhada com seus colegas de turma.
- O caso de uso se encerra.

### 12.4 Condições Posteriores
- A agenda do aluno estará disponível para que a visualização seja possível por outros alunos. 


## [UC13](#table) - Avaliar Agenda da Felicidade <a name="UC13"></a>

### Breve Descrição
- Esta funcionalidade permite ao usuário avaliar as Agendas que foram passadas, com objetivo de avaliar quais foram as mais interessantes de se realizar.

### Ator Principal
- Usuário.

### Condições Prévias
- O usuário deve estar logado.
- As agendas devem ter sido realizadas para que o usuário possa avaliá-las.


### Fluxo de Eventos
#### Fluxo Básico
#### [FB01] Realizar avaliação de Agenda da Felicidade
O caso de uso se inicia quando o usuário resolve avaliar uma Agenda já realizada.
- O usuário acessa Agenda e seleciona uma atividade já realizada.
- O usuário avalia essa Agenda de 1 a 5 estrelas, de acordo com seu nível de satisfação com esta atividade.
- O caso de uso se encerra.

### Condições Posteriores
- O administrador poderá visualizar as atividades mais interessantes de se realizar, comparando a avaliação de cada tipo de atividade.
- O administrador tem acesso às avaliações feitas pelos alunos, e assim tem controle sobre os tipos de atividades que mais satisfazem os alunos.


## [UC14](#table) - Adicionar Recepção da Semana <a name="UC14"></a>

### Breve Descrição
- Essa funcionalidade permite aos alunos adicionar um evento chamado Recepção com o objetivo de informar ao professor sobre atividades realizadas nessa recepção.

### Ator Principal
- Usuário.

### Condições Prévias
- O usuário deve estar logado.


### Fluxo de Eventos
#### Fluxo Básico
#### [FB01] Adicionar Recepção
O caso de uso se inicia quando o usuário precisa adicionar sua Recepção da Semama.
- O usuário clica em Recepção.
- O usuário cria uma recepção e adiciona as atividades a serem realizadas na recepção.
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
#### Fluxo Básico
#### [FB01] Realizar Atividade
- O usuário acessa "Atividades".
- O usuário seleciona o arquivo que deseja enviar e cria uma descrição.
- O usuário então envia a atividade desejada.
- O caso de uso se encerra.

### Condições Posteriores
- Visualização do andamento do produto final da disciplina pelo professor.


## [UC16](#table) - Manter Enquete <a name="UC16"></a>

### Breve Descrição
- Essa funcionalidade permite ao administrador criar enquetes para votação rápida através do aplicativo e deixá-las prontas para edição, visualização e votação

### Atores Principais
- Administrador e Usuário.

### Condições Prévias
- O administrador deve estar logado.
- Turma deve estar criada.


- O administrador criará uma enquete para a turma selecionada.
- Os usuários irão votar na enquete.
- O administrador terá acesso ao resultado da enquete criada.

### Fluxo de Eventos
#### Fluxo Básico
#### [FB01] - Criação e votação de enquete <a name="FB01enquete"></a>
- O administrador acessa "Mural".
- O administrador então seleciona a opção "Criar enquete".
- O administrador informa os dados da enquete a ser criada.
- O administrador clica na opção de criar a enquete.

#### [FB02] - Criação e votação de enquete <a name="FB02enquete"></a>
- Os usuários acessam "Mural".
- Os usuários escolhem a enquete a ser votada.
- Os usuários fazem sua votação.

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
- Em [FB01](#FB01enquete) O sistema deve disponibilizar a visualização da enquete para que os usuários votem.
- Em [FB02](#FB01enquete) O sistema deve disponibilizar a visualização dos resultados da enquete.
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
#### Fluxo Básico
#### [FB01] - Criar Thread em um tópico<a name="FB01thread"></a>
O caso de uso começa quando um usuário resolve criar uma thread em um tópico criado previamente
- O usuário acessa "Mural".
- O usuário acessa tópico a ser discutido.
- O usuário vê o tópico criado previamente e seleciona a opção "Comentar".
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

#### [FA02] - Editar Thread <a name="FA02thread"></a>
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
- Consiste em criar um canal de comunicação dinâmico entre os alunos e o professor, criando algo similar a um fórum, onde poderão ser criados tópicos. Além de ser possível a visualização, edição, e exclusão desses tópicos.

### Ator Principal
- Usuário.

### Condições Prévias
- O usuário deve estar cadastrado e logado.


### Fluxo de Eventos
#### Fluxo Básico
#### [FB01] Criar Tópico
O caso de uso se inicia no momento que um usuário resolver adicionar algum tópico no Mural.
- O usuário acessa o Mural.
- O usuário cria um tópico.
- O usuário adiciona as informações desejadas no tópico.
- O usuário publica o tópico.
- O caso de uso se encerra.

#### [FB02] Visualizar Tópico
O caso de uso se inicia quando um usuário deseja visualizar algum tópico publicado por ele.
- O usuário acessa o Mural.
- O usuário clica em Meus Tópicos.
- O usuário visualiza uma lista com os tópicos que ele publicou.
- O usuário clica no tópico desejado e visualiza as informações sobre ele.
- O caso de uso se encerra. [[FA01]](#fa01mantermural) [[FA02]](#fa02mantermural)

#### Fluxo Alternativo
#### [FA01] Editar Tópico <a name="#fa01mantermural"></a>
O caso de uso se inicia quando o usuário resolve editar um tópico criado por ele.
- O aluno clica em Editar Tópico.
- O aluno realiza as alterações desejadas.
- O aluno salva as alterações.
- O caso de uso se encerra.

#### [FA02] Deletar Tópico <a name="#fa02mantermural"></a>
O caso de uso se inicia quando o usuário resolve deletar um tópico criado por ele.
- O aluno clica em Deletar Tópico.
- O aluno confirma a ação.
- O tópico é deletado.
- O caso de uso se encerra.

### Condições Posteriores
- Alunos usuários do sistema e professor administrador terão acesso ao tópicos adicionados e suas alterações.

## [UC19](#table) - Visualizar Informações de Atendimento Psicológico <a name="UC19"></a>

### Breve Descrição
- Criar uma área informativa, a onde o aluno poderá ver procurar ajuda psicológica e outros canais que possam ser de ajuda, contendo números de contato, e-mails e afins, para facilitar o aluno encontrar atendimento especializado.

### Ator Principal
- Usuário.

#### Condições Prévias
- O aluno deve estar cadastrado e logado.


### Fluxo de Eventos
#### Fluxo Básico
#### [FB01] Acessar a Página com as Informações
O caso de uso se inicia quando um usuário deseja saber informações sobre atendimento psicológico especializado.
- O aluno acessa a página de área informativa.
- O aluno visualiza as informações desejadas.
- O caso de uso se encerra.

### Condições Posteriores
- O aluno terá acesso a todos os meios de ajuda disponível na página.
    
## [UC20](#table) - Manter Materiais <a name="UC20"></a>

### Breve Descrição
- Criar uma área de compartilhamento de material da disciplina, um local onde terá o conteúdo proposto pela a disciplina, o conteúdo que está sendo utilizado na aula, assim facilitando o uso do material para a disciplina.

### Ator Principal
- Administrador.

### 20.4 Condições Prévias
- O administrador deve estar logado.


### Fluxo de Eventos
#### Fluxo Básico
#### [FB01] Adicionar Material
O caso de uso se inicia no momento que o professor deseja adicionar algum conteúdo na área de compartilhamento.
- O professor acessa a página de compartilhamento.
- O professor seleciona a opção de Enviar Material.
- O professor escolhe o conteúdo e o envia.
- O caso de uso se encerra

#### [FB02] Visualizar Material
O caso de uso se inicia quando o professor deseja visualizar algum conteúdo de um Material compartilhado.
- O professor acessa a página de compartilhamento.
- O professor seleciona a opção de Visualizar Material.
- O professor visualiza o Material desejado.
- O caso de uso se encerra. [[FA01]](#fa01mantermaterial) [[FA02]](#fa02mantermaterial)

#### Fluxo Alternativo
#### [FA01] Editar Material <a name="fa01mantermaterial"></a>
O caso de uso se inicia quando o professor deseja editar algum Material já compartilhado.
- O professor clica em Editar Material.
- O professor realiza as alterações desejadas.
- O professor confirma as alterações.
- O caso de uso se encerra.

#### [FA02] Deletar Material <a name="fa02mantermaterial"></a>
O caso de uso se inicia quando o professor deseja deletar algum Material já compartilhado.
- O professor clica em Deletar Material.
- O professor confirma a ação.
- O material é deletado.
- O caso de uso se encerra.

### Condições Posteriores
- O aluno e o professor terão acesso a todo conteúdo disponível na página de compartilhamento de Material.

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
