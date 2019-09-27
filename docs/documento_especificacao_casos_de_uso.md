
## 1. UC01 - Administrador cadastrar Aluno

#### 1.1 Descrição
- O professor que administra o sistema deve ter a opção de cadastrar o aluno

#### 1.2 Atores
- Administrador

#### 1.3 Pré Condições
- Existir no sistema as entidades professor e aluno

#### 1.4 Fluxo Principal
- não se aplica

#### 1.5 Fluxos Alternativos
- não se aplica

#### 1.6. Fluxo de Exceção
- não se aplica

#### 1.7. Pós Condições
- Estará cadastrado um aluno

## 2. UC02 - Administrador manter turma

#### 2.1. Descrição
- O professor que administra o sistema deve ter a opção de cadastrar uma turma e fazer as devidas alterações

#### 2.2. Atores
Administrador

#### 2.3. Pré Condições

#### 2.4. Fluxo Principal

#### 2.5. Fluxos Alternativos

#### 2.6. Fluxo de Exceção

#### 2.7. Pós Condições

## 3. UC03 - Aluno realizar o próprio cadastro

#### 3.1 Descrição
- O aluno usuário do sistema deve ter a opção de fazer o seu próprio cadastro

#### 3.2. Atores
Aluno

#### 3.3. Pré Condições

#### 3.4. Fluxo Principal

#### 3.5. Fluxos Alternativos

#### 3.6. Fluxo de Exceção

#### 3.7. Pós Condições

## 4. UC04 - Aluno gerenciar o próprio grupo

#### 4.1 Descrição
- O aluno usuário do sistema deve ter a opção de fazer o próprio gerenciamento de seu grupo

#### 4.2 Atores
- Aluno

#### 4.3. Pré Condições
- O aluno deve existir no sistema
- Os grupos devem existir no sistema

#### 4.4 Fluxo Principal

#### 4.5. Fluxos Alternativos

#### 4.6. Fluxo de Exceção

#### 4.7. Pós Condições

## 5. UC05 - Visualizar perfil
#### 5.1 Breve descrição
<p>Usuário deseja visualizar informações sobre o seu perfil, como: Pontuação no índice de felicidade autêntica, total de pontos, informações básicas do usuário, etc.</p>

#### 5.2 Ator Principal
Usuário

#### 5.3 Condições prévias
- O usuário deve ter vínculo com a instituição.
- O usuário deve estar logado.

#### 5.4 Condições posteriores
Visualização dos dados com sucesso.

#### 5.5 Fluxo de eventos
- O usuário irá visualizar o status atual de seus dados de perfil

#### 5.5.1 Fluxo Básico
O fluxo básico é composto de passos que o usuário seguirá para poder visualizar seus dados.
<ol>
    <li>O usuário faz login no sistema</li>
    <li>O usuário clica em perfil</li>
    <li>O caso de uso encerra</li>
</ol>

#### 5.5.2 Fluxo Alternativo
Não se aplica
#### 5.5.3 Fluxo de Exceção
Não se aplica

#### 5.6 Regras de Negócio
Não se aplica

## 6. UC06 - Adicionar humor do dia
#### 6.1 Breve descrição
Essa funcionalidade oferece uma lista de emojis para que o usuário selecione apenas um  e dessa maneira o sistema classifica o humor que o ele está vivenciando no dia. 

#### 6.2 Ator Principal
Usuário.

#### 6.3 Condições prévias
- O usuário deve estar logado no sistema
- O usuário deve ter vínculo com a instituição.
- O usuário ainda não pode ter selecionado um humor para aquele dia

#### 6.4 Condições posteriores
Visualizar o gráfico baseado em todos os humores do usuário até o atual dia.

#### 6.5 Fluxo de eventos
- O usuário irá selecionar o emoji que mais se aproxima do humor que ele está passando naquele dia.

#### 6.5.1 Fluxo Básico
Esse fluxo se inicia quando o usuário deseja registrar o seu humor referente ao dia atual.
<ol>
    <li>O usuário acessa o perfil.</li>
    <li>O usuário então acessa o humor do dia.</li>
    <li>O usuário escolhe um dos emojis.</li>
    <li>O caso de uso encerra.</li>
</ol>

#### 6.5.2 Fluxo Alternativo
Esse fluxo se inicia quando o usuário ao invés de selecionar um dos emojis clica em "Cancelar".

<ol>
    <li>O usuário clica em "Cancelar".</li>
    <li>O caso de uso se encerra.</li>
</ol>

#### 6.5.3 Fluxo de Exceção
Não se aplica

#### 6.6 Regras de Negócio
Não se aplica

## 7. UC07 - Visualizar dashboard dos grupos
#### 7.1 Breve descrição
Essa funcionalidade permite ao administrador visualizar informações de todos os grupos da turma por meio de cards. Cada card contém informações básicas de cada grupo e um link para a página do grupo.

#### 7.2 Ator Principal
Administrador.

#### 7.3 Condições prévias
- O administrador deve estar logado no sistema.
- Devem existir grupos cadastrados no sistema.

#### 7.4 Condições posteriores
- Visualizar informações básicas de todos os grupos com sucesso.
- Acessar por meio do link do card mais informações sobre o grupo selecionado.

#### 7.5 Fluxo de eventos
- O administrador irá ter acesso as informações básicas de cada grupo cadastrado por meio dos cards.
- O administrador pode saber mais sobre cada grupo acessando a página do grupo por meio do link no card.

#### 7.5.1 Fluxo Básico
Esse fluxo se inicia quando o administrador deseja ver os dados de todos os grupos ou de apenas um grupo cadastrado.
<ol>
    <li>O administrador acessa "Grupos".</li>
    <li>O adminstrador acessa "Listar grupos".</li>
    <li>O caso de uso se encerra.</li>
</ol>

#### 7.5.2 Fluxo Alternativo
Esse fluxo se inicia quando o administrador deseja acessar mais informações além das básicas que o card oferece.
<ol>
    <li>O administrador acessa o link no card.</li>
    <li>O caso de uso se encerra.</li>
</ol>

#### 7.5.3 Fluxo de Exceção
Não se aplica.

#### 7.6 Regras de Negócio
Não se aplica.

## 8. UC08 - Visualizar gráfico de humor da turma
#### 8.1 Breve descrição
Essa funcionalidade permite ao administrador checar o humor da turma ao longo do tempo por meio de um gráfico que leva em conta cada aluno.

#### 8.2 Ator Principal
Administrador.

#### 8.3 Condições prévias
- O administrador deve estar logado.
- Ao menos uma turma deve estar cadastrada no sistema.

#### 8.4 Condições posteriores
- Visualização do gráfico de humor da turma.

#### 8.5 Fluxo de eventos
- O administrador acessará todas as turmas.
- O administrador terá acesso ao gráfico de humor de cada turma.

#### 8.5.1 Fluxo Básico
Esse fluxo se inicia quando o administrador lista turmas e deseja ver humor de determinada turma.
<ol>
    <li>O administrador acessa "Turmas".</li>
    <li>O administrador então seleciona a turma que deseja ver o gráfico de humor.</li>
    <li>O administrador acessa o gráfico de humor da turma desejada.</li>
    <li>O caso de uso se encerra.</li>
</ol>

#### 8.5.2 Fluxo Alternativo
Não se aplica.

#### 8.5.3 Fluxo de Exceção
Não se aplica.

#### 8.6 Regras de Negócio
Não se aplica.

## 9. UC09 - Mandar notificação push
#### 9.1 Breve descrição
Essa funcionalidade permite ao administrador mandar notificações aos alunos de uma turma.

#### 9.2 Ator Principal
Administrador.

#### 9.3 Condições prévias
- O administrador deve estar logado no sistema.
- Deve existir ao menos uma turma cadastrada no sistema.

#### 9.4 Fluxo de eventos
- O administrador irá ter acesso às turmas e poderá enviar notificações para os alunos de uma determinada turma.

#### 9.4.1 Fluxo Básico
Esse fluxo se inicia quando o administrador deseja enviar uma notificação aos alunos de uma turma.
- O administrador acessa "Turmas".
- O administrador escolhe uma das turmas.
- O administrador digita a mensagem que ele deseja enviar.
- O administrador envia a notificação.
- O caso de uso se encerra.

#### 9.4.2 Fluxo Alternativo
Não se aplica.

#### 9.4.3 Fluxo de Exceção
Não se aplica.

#### 9.5 Regras de Negócio
Não se aplica.

## 10. UC10 - Manter Agenda da felicidade
#### 10.1 Breve descrição
Essa funcionalidade permite ao administrador criar, editar ou deletar agendas.

#### 10.2 Ator Principal
Administrador.

#### 10.3 Condições prévias
- O administrador deve estar logado.

#### 10.4 Condições posteriores
- Visualização da(s) agenda(s) pelos usuários.

#### 10.5 Fluxo de eventos
- O administrador criará uma agenda (atividade).
- Os usuários poderão visualizar a agenda.

#### 10.5.1 Fluxo Básico
- O administrador acessa "Agendas".
- O administrador cria uma agenda.   

#### 10.5.2 Fluxo Alternativo

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

#### 10.5.3 Fluxo de Exceção
Não se aplica.

#### 10.6 Regras de Negócio
Não se aplica.

## 11. UC11 - Realizar agenda da felicidade
#### 11.1 Breve descrição
Essa funcionalidade permite ao usuário realizar agendas.

#### 11.2 Ator Principal
Usuário.

#### 11.3 Condições prévias
- O usuário deve estar logado.
- Deve existir ao menos uma agenda.

#### 11.4 Condições posteriores
- Visualização da resposta pelo administrador.

#### 11.5 Fluxo de eventos

#### 10.5.1 Fluxo Básico
- O usuário acessa "Agendas".
- O usuário escolhe uma agenda.   
- O usuário envia a resposta da agenda.

#### 10.5.2 Fluxo Alternativo
Não se aplica.

#### 10.5.3 Fluxo de Exceção
Não se aplica.

#### 10.6 Regras de Negócio
Não se aplica.


## 12. UC12 - Compartilhar agenda

### 12.1 Breve descrição
Essa funcionalidade permite ao usuário compartilhar sua agenda pessoal semanal com seus colegas de turma.

### 12.2 Ator Principal
Usuário.

### 12.3 Condições prévias
- O usuário deve estar logado.

### 12.4 Condições posteriores
- A agenda semanal do usuário é compartilhada com seus colegas de turma.

### 12.5 Fluxo de eventos
- O usuário compartilha sua agenda semanal de atividades com seus colegas.
- A agenda do aluno estará disponível para que a visualização seja possível por outros alunos. 

#### 12.5.1 Fluxo Básico
<ol>
    <li>O usuário acessa "Agenda pessoal".</li>
    <li>O usuário compartilha suas atividades semanais.</li>
    <li>O a agenda semanal do usuário se torna disponível para a visualização por outros usuários.</li>
    <li>O caso de uso se encerra.</li>
</ol>

#### 12.5.2 Fluxo Alternativo
Não se aplica.

#### 12.5.3 Fluxo de Exceção
Não se aplica.

### 12.6 Regras de Negócio
Não se aplica.

## 13. UC13 - Avaliar Agenda

### 13.1 Breve descrição
Esta funcionalidade permite ao usuário avaliar as atividades que foram passadas, com objetivo de avaliar quais foram as mais interessantes de se realizar.

### 13.2 Ator Principal
Usuário.

### 13.3 Condições prévias
- O usuário deve estar logado.
- Atividades devem ter sido realizadas para que o usuário possa avaliá-las.

### 13.4 Condições posteriores
- O administrador poderá visualizar as atividades mais interessantes de se realizar, comparando a avaliação de cada tipo de atividade.

### 13.5 Fluxo de eventos
- O usuário, logado, avalia (1 a 5 estrelas) atividades já realizadas de acordo com seu nível de satisfação com aquela atividade.
- O administrador tem acesso às avaliações feitas pelos alunos, e assim tem controle sobre os tipos de atividades que mais satisfazem os alunos.

#### 13.5.1 Fluxo Básico
<ol>
    <li>O usuário acessa "Atividades" e seleciona uma atividade já realizada.</li>
    <li>O usuário avalia essa atividade de 1 a 5 estrelas, de acordo com seu nível de satisfação com esta atividade.</li>
    <li>O administrador tem acesso a todas as avaliações feitas, tendo, assim, controle sobre os tipos de atividade que mais satisfazem os alunos.</li>
    <li>O caso de uso se encerra.</li>
</ol>

#### 13.5.2 Fluxo Alternativo
Não se aplica.

#### 13.5.3 Fluxo de Exceção
Não se aplica.

#### 13.6 Regras de Negócio
Não se aplica.

## 14. UC14 - Adicionar recepção da semana

### 14.1 Breve descrição
Essa funcionalidade permite aos alunos adicionar um evento chamado "recepção" com o objetivo de informar ao professor sobre atividades realizadas nessa recepção. As recepções são eventos que ocorrem

### 14.2 Ator Principal
Usuário.

### 14.3 Condições prévias
- O usuário deve estar logado.

### 14.4 Condições posteriores
- O administrador terá visualização completa e controle sobre as atividades realizadas nas recepções.

### 14.5 Fluxo de eventos
- O usuário cria uma recepção com atividades a serem realizadas.
- A partir disso, o administrador pode ver e controlar as atividades realizadas nas recepções.

#### 14.5.1 Fluxo Básico
<ol>
    <li>O usuário cria uma recepção e adiciona as atividades a serem realizadas na recepção.</li>
    <li>O administrador poderá, então, visualizar e controlar a recepção.
    <li>O caso de uso se encerra.</li>
</ol>

#### 14.5.2 Fluxo Alternativo
Não se aplica.

#### 14.5.3 Fluxo de Exceção
Não se aplica.

### 14.6 Regras de Negócio
Não se aplica.

## 15. UC15 - Realizar atividades do produto final de felicidade 
#### 15.1 Breve descrição
Essa funcionalidade permite ao usuário realizar atividades do produto final da disciplina e ao professor acompanhar o adamento do mesmo.
#### 15.2 Ator Principal
Administrador.

#### 15.3 Condições prévias
- O usuário deve estar logado.

#### 15.4 Condições posteriores
- Visualização do andamento do produto final da disciplina.

#### 15.5 Fluxo de eventos
- O usuário envia suas atividades ao decorrer do semestre.
- O administrador terá acesso ao informativo em formato de linha do tempo quanto ao andamento do projeto.

#### 15.5.1 Fluxo Básico
<ol>
    <li>O usuário acessa "Atividades".</li>
    <li>O usuário seleciona o arquivo que deseja enviar e cria uma descrição.</li>
    <li>O usuário então envia a atividade desejada.</li>
    <li>O professor acessa a linha do tempo de atividades daquele usuário.</li>
    <li>O caso de uso se encerra.</li>
</ol>

#### 15.5.2 Fluxo Alternativo
Não se aplica.

#### 15.5.3 Fluxo de Exceção
Não se aplica.

#### 15.6 Regras de Negócio
Não se aplica.

## 16. UC16 - Manter Enquete
#### 16.1 Breve descrição
Essa funcionalidade permite ao administrador criar enquetes para votação rápida através do aplicativo e deixá-las prontas para edição, visualização e votação

#### 16.2 Ator Principal
Administrador e Usuário.

#### 16.3 Condições prévias
- O administrador deve estar logado.
- Turma deve estar criada.

#### 16.4 Condições posteriores
- Visualização dos resultados da enquete.

#### 16.5 Fluxo de eventos
- O administrador criará uma enquete para a turma selecionada.
- Os usuários irão votar na enquete.
- O administrador terá acesso ao resultado da enquete criada.

#### 16.5.1 Fluxo Básico
<ol>
    <li>O administrador acessa "Mural".</li>
    <li>O administrador então seleciona a opção "Criar enquete".</li>
    <li>O administrador informa os dados da enquete a ser criada.</li>
    <li>O administrador clica na opção de criar a enquete.</li>
    <li>Os usuários acessam "Mural".</li>
    <li>Os usuários escolhem o seu voto.</li>
    <li>O administrador visualiza os resultados da enquete.</li>
    <li>O caso de uso se encerra.</li>
</ol>

#### 16.5.2 Fluxo Alternativo
Não se aplica.

#### 16.5.3 Fluxo de Exceção
Não se aplica.

#### 16.6 Regras de Negócio
Não se aplica.

## 17. UC17 - Manter Thread
#### 17.1 Breve descrição
Essa funcionalidade permite aos usuários comentar os tópicos criados por outros usuários ou administradores no Mural.

#### 17.2 Ator Principal
Usuário.

#### 17.3 Condições prévias
- O usuário deve estar logado.
- Tópico deve estar criado no mural.

#### 17.4 Condições posteriores
- Visualização dos comentários pelos outros usuários.

#### 17.5 Fluxo de eventos
- Um usuário criará um tópico para discussão.
- Outros usuários criarão comentários naquele tópico

#### 17.5.1 Fluxo Básico
<ol>
    <li>O usuário acessa "Mural".</li>
    <li>O usuário cria um tópico a ser discutido</li>
    <li>Outro usuário acessa "Mural"</li>
    <li>O outro usuário vê o tópico criado e seleciona a opção "Comentar"</li>
    <li>O outro usuário cria seu comentário e salva</li>
    <li>Os usuários poderão visualizar os comentários criados nos tópicos do mural</li>
    <li>O caso de uso se encerra.</li>
</ol>

#### 17.5.2 Fluxo Alternativo
Não se aplica.

#### 17.5.3 Fluxo de Exceção
Não se aplica.

#### 17.6 Regras de Negócio
Não se aplica.
