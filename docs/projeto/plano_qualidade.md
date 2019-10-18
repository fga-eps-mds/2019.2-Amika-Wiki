# Plano de Gerenciamento da Qualidade

## 1. Objetivos Estratégicos
O projeto, no contexto da disciplina, tem como objetivo principal a produtividade da equipe, para garantir que estejam seguindo e aplicando as praticas ágeis desenvolvidas, assim a qualidade do código para que seja um produto entregue que possa ser evoluido e mantido futuramente assim como a evolução da equipe, em questão de maturidade e técnica, principalmente da equipe de desenvolvimento se espera um crescimento nas tecnologias e familiaridade com o código. Sendo assim os principais objetivos para esta medição são:

- Produtividade da equipe;
- Evolução da equipe;
- Qualidade do código;

## 2. Planejamento de Medição

A abordagem GQM (Goal Question Metric) será adotada para identificar as métricas que atinjam os objetivos propostos para o contexto do projeto Amika, assim como levantar as questões necessárias que estas métricas devem bater.

## 3. Definição dos Objetivos de Medição

## 3.1 Objetivo de Equipe
### 3.1.1 - Objetivo 1 - Evolução da equipe
<table class="responsive-table highlight bordered">
<tr>
  <th><b>Analisar</b></th>
  <th>Para o propósito de</th>
  <th>Com respeito à</th>
  <th>Sob o ponto de vista de</th>
  <th>No contexto de</th>
</tr>
<tr>
    <td>Equipe de desenvolvimento</td>
    <td>Melhorar</td>
    <td>Capacitação</td>
    <td>Desenvolvedores</td>
    <td>Amika</td>
  </tr>
</table>

### 3.1.2 - Objetivo 2 - Produtividade da equipe
<table class="responsive-table highlight bordered">
<tr>
  <th><b>Analisar</b></th>
  <th>Para o propósito de</th>
  <th>Com respeito à</th>
  <th>Sob o ponto de vista de</th>
  <th>No contexto de</th>
</tr>
<tr>
    <td>Equipe de desenvolvimento</td>
    <td>Melhorar</td>
    <td>Produtividade</td>
    <td>Desenvolvedores</td>
    <td>Amika</td>
  </tr>
</table>

## 3.2 Objetivo de Produto

### 3.2.1 - Objetivo 3 - Qualidade de código
<table class="responsive-table highlight bordered">
  <tr>
    <th><b>Analisar</b></th>
    <th>Para o propósito de</th>
    <th>Com respeito à</th>
    <th>Sob o ponto de vista de</th>
    <th>No contexto de</th>
  </tr>
  <tr>
    <td>O código</td>
    <td>Melhorar</td>
    <td>Qualidade do código</td>
    <td>Desenvolvedores</td>
    <td>Amika</td>
  </tr>
</table>

## 4. Questões de Medição

### 4.1 - Questões Objetivo 1 - Equipe do Projeto Amika

* Questão 1 (O01Q01) -  A equipe está sendo produtiva ?
* Questão 2 (O01Q02) - A dedicação da equipe é constante ?
* Questão 3 (O01Q03) - A equipe esta trabalhando de maneira ágil ?
* Questão 4 (O01Q04) - A equipe evoluiu ao longo do projeto ?

### 4.2 - Questões Objetivo 2 - Produto

* Questão 1 (O02Q01) - Qual a complexidade ciclomática ?
* Questão 2 (O02Q02) - Qual a cobertura de testes ?
* Questão 3 (O02Q03) - Qual a Manutenabilidade ?

## 6. Métricas Escolhidas

### 6.1 - Métricas do Objetivo 1 - Equipe do Projeto Amika

#### Métrica 1.1 - Quadro de conhecimento
<table class="responsive-table highlight bordered">
<tr>
  <td><b>Métrica</b></td>
  <td>Pontos de evolução</td>  
</tr>
  <tr>
    <td><b>Objetivo de Medição</b></td>
    <td style="text-align: justify">Verificar quantos membros da equipe melhoraram em cada um dos conhecimentos e tecnologias necessárias para o desenvolvimento do projeto ao longo do semestre.</td>  
  </tr>
  <tr>
    <td><b>Fórmula de Obtenção</b></td>
    <td style="text-align: justify">Os conhecimentos são divididos em 5 escalas na qual enquanto mais altas as escalas maior o conhecimento sobre aquele assunto, cada vez que um integrante sobe uma escala é somado um ponto.</td>  
  </tr>
  <tr>
    <td><b>Escala de Medição</b></td>
    <td>Racional</td>  
  </tr>
  <tr>
    <td><b>Coleta</b></td>
    <td>
    Responsável: Matheus Roberto
    Periodicidade: A cada sprint
    Procedimento: Uso do quadro de conhecimento feito na planilha do grupo de desenvolvimento, e somando os pontos caso hajam mudanças.</td>  
  </tr>
  <tr>
    <td><b>Análise</b></td>
    <td style="text-align: justify">Se o número de pontos do quadro de conhecimento de uma determinada tecnologia for 0, indica que a equipe não a utilizou ou não houve nenhum ganho de conhecimento pela escolha desta, já caso o número encontrado seja 5, indica que a equipe evoluiu muito bem a respeito daquela determinada tecnologia/td>  
  </tr>
  <tr>
    <td><b>Meta</b></td>
    <td style="text-align: justify">Pontuação do quadro de conhecimento seja no mínimo 1 para cada tecnologia</td>  
  </tr>
  <tr>
    <td><b>Providência</b></td>
    <td style="text-align: justify">
    - Realizar dojos e treinamentos a respeito de tecnologias que não vem sendo evoluídas<br>
    - Identificar os membros com mais conhecimento sobre determinado assunto para parear com outros com menos conhecimento.
    </td>
  </tr>
</table>

#### Métrica 1.2 - Velocity
<table class="responsive-table highlight bordered">
<tr>
  <td><b>Métrica</b></td>
  <td>Velocity</td>  
</tr>
  <tr>
    <td><b>Objetivo de Medição</b></td>
    <td style="text-align: justify">Garantir as entregas contínuas da metodologia utilizada, e a quantidade de pontos que a equipe consegue entregar por sprint </td>  
  </tr>
  <tr>
    <td><b>Fórmula de Obtenção</b></td>
    <td> 
    V = Tp/S <br><br>
    Onde:<br>
    V - Velocity<br>
    Tp - Total de Pontos realizados na Sprint.
    S - Quantidade de Sprints.
 </td>  
  </tr>
  <tr>
    <td><b>Escala de Medição</b></td>
    <td>Nominal</td>  
  </tr>
  <tr>
    <td><b>Coleta</b></td>
    <td style="text-align: justify">Responsável: Matheus Roberto <BR>
      Periodicidade: A cada Sprint
      Procedimento: Utilizar a Plataforma Zenhub para coletar os dados do Velocity.
    </td>  
  </tr>
  <tr>
    <td><b>Análise</b></td>
    <td style="text-align: justify">O ideal seria o Velocity se manter constante ou aumentar ao longo do projeto, pois o Velocity deveria ser utilizado para planejar a Sprint
    </td>  
  </tr>
  <tr>
    <td><b>Meta</b></td>
    <td style="text-align: justify">Velocity manter constante ao longo do projeto</td>  
  </tr>
  <tr>
    <td><b>Providência</b></td>
    <td style="text-align: justify">
    Para que a meta seja atingida, algumas providências podem ser tomadas:<br><br>
    - Avaliar o tempo das sprints<br>
    - Analisar a quantidade de pontos que a equipe consegue entregar<br>
    </td>
  </tr>
</table>


### 6.2 - Métricas do Objetivo 2 - Código

#### Métrica 2.1 - Complexidade Ciclomática
<table class="responsive-table highlight bordered">
  <tr>
    <td><b>Métrica</b></td>
    <td>Complexidade Ciclomática</td>
  </tr>
  <tr>
    <td><b>Objetivo de Medição</b></td>
    <td style="text-align: justify">Identificar trechos do código com complexidade ciclomática alta como forma de corrigi-las e tratá-las, para manter a qualidade e manutenabilidade de código.</td>  
  </tr>
  <tr>
    <td><b>Fórmula de Obtenção</b></td>
    <td style="text-align: justify">
    PR = 1000000 + (A - T) * 100000<br><br>
    Onde:<br><br>
    -PR: Pontos de Remediação<br>
    - A: Valor atual, é a pontuação de um determinado método ou unidade de código<br>
    - T: é o comprimento máximo configurado ou o número de complexidade McCabe.<br>
    O resultado é exibido por letras entre "A" e "F".    
    </td>  
  </tr>
  <tr>
    <td><b>Escala de Medição</b></td>
    <td>Ordinal</td>  
  </tr>
  <tr>
    <td><b>Coleta</b></td>
    <td>
    Responsável: Equipe de EPS<br>
    Periodicidade: A cada Pull Request<br>
    Procedimento: Coleta realizada pela ferramenta de análise estática <b>Code Climate</b>.</td>  
  </tr>
  <tr>
    <td style="text-align: justify"><b>Análise</b></td>
    <td style="text-align: justify">A complexidade ciclomática deve ser monitorada em cada Pull Request para avaliar a manutenção e qualidade do código. Se a complexidade aumenta muito, isso influencia a ocorrência de erros no código e pode refletir na execução de testes.</td>  
  </tr>
  <tr>
    <td><b>Meta</b></td>
    <td>Meta é manter a classificação entre "A" e "B".</td>  
  </tr>
  <tr>
    <td><b>Providência</b></td>
    <td>Planejar a refatoração do código para melhorar o índice e qualidade do produto, a ferramenta utilizada apresenta os trechos de código nos quais a complexidade ciclomática está em um nível que deve ser refatorado.</td>
  </tr>

</table>

#### Métrica 2.2 -  Manutenibilidade
<table class="responsive-table highlight bordered">
  <tr>
    <td><b>Métrica</b></td>
    <td>Manutenibilidade</td>
  </tr>
  <tr>
    <td><b>Objetivo de Medição</b></td>
    <td style="text-align: justify">Identificar regiões de ocorrência de anomalias e discordâncias no código a fim de corrigi-los como forma de melhorar a qualidade do código.</td>  
  </tr>
  <tr>
    <td><b>Fórmula de Obtenção</b></td>
      <td style="text-align: justify">Analisada pela ferramenta de análise estática <b>Code Climate</b>, que analisa os nós das àrvores sintática abstrata (AST). O critério aplicado pela ferramenta trata-se do <b>tempo de remediação</b>, ou seja, o tempo para reverter uma anomalia encontrada. Para arquivos, são atribuidas letras de acordo com as faixas associadas, de A a F: <br><br>
    <li> A: 0 - 2M pontos de remediação </li>
    <li> B: >2M - 4M pontos de remediação</li>
    <li> C: >4M - 8M pontos de remediação</li>
    <li> D: >8M - 16M pontos de remediação</li>
    <li> F: >16M   pontos de remediação</li><br>
    A avaliação do repositório total, é dada seguindo os critérios de tempo de remediação associado ao número total de linhas do projeto:<br><br>
    DT = TR / TI<br><br>
    Onde:<br><br>
    <li> DT: Débito técnico</li>
    <li> TR: Tempo de Remediação</li>
    <li> TI: Tempo estimado de implementação</li>
    <br>
    A ferramenta gera essa classificação por repositório com uma letra entre A e F, conforme citado acima.
    </td>  
  </tr>
  <tr>
    <td><b>Escala de Medição</b></td>
    <td>Ordinal</td>  
  </tr>
  <tr>
    <td><b>Coleta</b></td>
    <td>
    Responsável: Equipe de EPS<br>
    Periodicidade: A cada Pull Request<br>
    Procedimento: Coleta realizada pela
    ferramenta de análise estática <b>Code Climate</b>.</td>  
  </tr>
  <tr>
    <td><b>Análise</b></td>
    <td style="text-align: justify">A meta é que a manutenibilidade seja A. Caso esses valores divirjam cada vez mais da classe "A", isso indica que o produto está sendo desenvolvido sem preocupação com a manutenção e qualidade, o que aumenta a ocorrência de erros e chance de falhas futuras. O ideal é que se mantenha em "A", tanto para os arquivos, quanto para o repositório.</td>  
  </tr>
  <tr>
    <td><b>Meta</b></td>
    <td>Que a classificação do projeto seja "A".</td>  
  </tr>
  <tr>
    <td><b>Providência</b></td>
    <td style="text-align: justify">Refatoração imediata do código de acordo com as informações e trechos indicados pela ferramenta, a fim de não comprometer o andamento do projeto e não se propague a proporção de crescimento do tamanho do código.</td>
  </tr>  
</table>


#### Métrica 2.3 - Cobertura de Testes
<table class="responsive-table highlight bordered">
  <tr>
    <td><b>Métrica</b></td>
    <td>Cobertura de Teste</td>
  </tr>
  <tr>
    <td><b>Objetivo de Medição</b></td>
    <td style="text-align: justify">Identificar o nível de cobertura de teste, para manter a qualidade do código.</td>  
  </tr>
  <tr>
    <td><b>Fórmula de Obtenção</b></td>
    <td style="text-align: justify"> A ferramenta <b>TravisBuilder</b> avalia os trechos de código cobertos por testes em relação a quantidade de linhas de código, e também quantas vezes algum teste passou naquela linha(Hits).
    </td>  
  </tr>
  <tr>
    <td><b>Escala de Medição</b></td>
    <td>Racional</td>  
  </tr>
  <tr>
    <td><b>Coleta</b></td>
    <td>
    Responsável: Vinicius Cantuária<br>
    Periodicidade: A cada Pull Request<br>
    Procedimento: Coleta realizada pela
    ferramenta de análise estática <b>Travis Builder</b>.</td>  
  </tr>
  <tr>
    <td><b>Análise</b></td>
    <td style="text-align: justify">O ideal é que os testes sejam realizados em paralelo com o desenvolvimento do projeto, como forma de identificar os erros e falhas encontrados de imediato. A meta é que a cobertura seja de 90%, menos que isso significaria que muitos trechos do código não estão sendo testados, causando assim uma fragilidade em suas funcionalidades e não garantindo a qualidade de forma adequada, alguns fatores que podem ocasionar nisso são a alta complexidade ciclomática e uma classe ruim de manutenabilidade, dizendo assim que suas funções são difíceis de serem testadas</td>  
  </tr>
  <tr>
    <td><b>Meta</b></td>
    <td>A meta é 90% de cobertura de teste.</td>  
  </tr>
  <tr>
    <td><b>Providência</b></td>
    <td style="text-align: justify">Caso haja dificuldade em realizar os testes, devem ser verificados o nível de manutenibilidade, complexidade ciclomática e o quadro de conhecimento na área de aplicação de testes, realizar treinamentos e dojôs, e avaliar os critérios de aceitação, que incluem a implementação de teste. Assim como só aceitar Pull Requests na quais as funcionalidades sejam testadas</td>
  </tr>  
</table>
