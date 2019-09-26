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