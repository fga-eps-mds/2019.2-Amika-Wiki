## 1. Introdução
#### 1.1. Finalidade
O presente documento visa proporcionar um panorama claro e detalhado compartilhado pelos integrantes da equipe de desenvolvimento do (nome do projeto) a respeito da proposta do projeto, através da apresentação das suas funcionalidades e utilidades. Dessa forma, será possível o pleno entendimento do leitor sobre os tópicos abordados, mesmo que este não possua conhecimento dos detalhes técnicos que permeiam a execução desse software. 

#### 1.2. Escopo
Este documento expõe os aspectos fundamentais para o entendimento do produto, desde a formulação até a implantação no meio alvo. Assim como descreve o ambiente em que o produto será implementado e como o aplicativo irá ser relacionado com os usuários e envolvidos. 

#### 1.3. Definições, Acrônimos e Abreviações

**Acrônimo/Abreviação** | **Definição**
------------------------|-------------------
UnB | Universidade de Brasília.
RUP | Rational Unified Process (Processo Unificado da Rational) - Processo de técnicas da engenharia de software.

#### 1.4. Referências Bibliográficas
International Business Machines Corporation. **Documento de Visão**. Disponível em: https://www.ibm.com/support/knowledgecenter/pt-br/SSWMEQ_4.0.6/com.ibm.rational.rrm.help.doc/topics/r_vision_doc.html. Acesso em: 1 de Setembro de 2019.

#### 1.5. Visão Geral
Produzido a partir do processo RUP - Rational Unified Process, este documento é organizado com as ideias, recursos, descrição e posicionamento do produto. Apresentando uma visão geral do produto, seus requisitos e a relação com os envolvidos e usuários do produto.

<h2>2. Posicionamento</h2>

<h3>2.1 Oportunidade de Negócios</h3>
Atualmente a matéria Felicidade ofertada no Campus da Universidade de Brasília localizado no Gama, Faculdade do Gama, sofre o problema de organização de notas, trabalhos e eventos. Para solucionar esse problema o professor da disciplina utiliza anotações que tornam o trabalho exaustivo e lento e acabam por não resolver o problema de organização, visto que atrasos quanto ao lançamento de notas, organização de datas e coisas do gênero ainda ocorrem todo semestre. De acordo com essa realidade, o aplicativo (adicionar nome) tem por objetivo tornar mais simples e rápido o processo de organização de datas, comunicação de notas e avisos aos alunos e interação entre esses e o professor.


<h3>2.2 Descrição do problema</h3>
<table>
<tr><td style="text-align: center;"> O problema de         </td><td style="text-align: center;"> realizar o gerenciamento de notas, grupos da disciplina, coleta de dados da disciplina e monitorar as atividades pessoais dos alunos manualmente                                                                                          </td></tr>
<tr><td style="text-align: center;"> afeta                 </td><td style="text-align: center;"><center> alunos e professor                                                                                                                                                                                                                        </td></tr>
<tr><td style="text-align: center;">cujo impacto é        </td><td style="text-align: center;"> um processo de definição e organização de datas e eventos lento e cansativo, além de muitas vezes falhar e ser novamente modificado</td></tr>
<tr><td style="text-align: center;"> uma boa solução seria </td><td style="text-align: center;"> um sistema capaz de tornar automático o lançamento de notas e avisos, coleta de dados a respeito da disciplina, organização de grupos da mesma e monitorar atividades pessoais dos alunos por um canal não poluído com outras informações </td></tr>
</table>
<h3>2.3 Sentença de posição do produto</h3>
<table>
<tr><td style="text-align: center;"> Para            </td><td style="text-align: center;"> O professor e discentes da disciplina de Felicidade                                                                        </td></tr>
<tr><td style="text-align: center;"> Que             </td><td style="text-align: center;"> necessitam de automatizar e tornar simples suas tarefas relacionadas à disciplina                                          </td></tr>
<tr><td style="text-align: center;"> O               </td><td style="text-align: center;"> (colocar nome do aplicativo quando for definido)                                                                           </td></tr>
<tr><td style="text-align: center;"> Que             </td><td style="text-align: center;"> gerencia atividades e permite a interação direta entre aluno e professor</td>                                                   </tr>
<tr><td style="text-align: center;"> Diferente da</td>    <td style="text-align: center;"> plataforma Moodle</td></tr>                                                                                          
<tr><td style="text-align: center;"> O nosso produto </td><td style="text-align: center;"> Não polui a interface do usuário com informações desnecessárias de outras matérias e possui velocidade de tráfego superior </td></tr>
</table>
## 3. Descrição dos Envolvidos e dos Usuários
#### 3.1. Resumo dos Envolvidos

#### 3.2. Resumo dos Usuários

#### 3.3. Ambiente do Usuário

#### 3.4. Perfis dos Envolvidos
##### 3.4.1. Equipe de Gestão de Projeto

##### 3.4.2. Equipe de Desenvolvimento

#### 3.5. Perfis dos Usuários
##### 3.5.1. Gestor de projeto


#### 3.6. Principais necessidades dos usuários ou envolvidos
#### 3.7. Alternativas e concorrência

## 4. Visão Geral do Produto
#### 4.1. Perspectiva do produto

O sistema terá a função de auxiliar a disciplina de felicidade por meio de recursos que permitam acompanhamento dos alunos e a interação entre os mesmos, tais recursos serão implementados junto a estratégias de gamificação, de forma que seu uso seja mais atraente e natural, outra necessidade é de que o professor e a equipe de monitores tenham acesso a atividades e as interações dos usuários.

#### 4.2. Resumo dos recursos

| Recurso  | Detalhes |
| ------------- | ------------- |
| Agenda pessoal   | Nessa agenda o aluno pode listar suas atividades, a agenda pode ser publicada ou ser privada ao aluno |
| Enquetes  | Feitas em tempo real pelo professor da disciplina para apontar questões levantadas na aula   |
| Controle de cadastro  | Alunos matriculados podem ter cadastro na aplicação e o controle de cadastros deve estar disponível para o professor e monitores  |
| Marcador para o nível de felicidade   | O feedback do nível de felicidade dos alunos deve ser mostrado em forma de uma barra de progresso  |
| Grupos  | Deve ser possível formar grupos entre os alunos, tal recurso vai ser gamificado em forma de guildas previamente definidas|
| Customização pessoal  | Customização da aplicação conforme aspectos definidos na gamificação, como stickers, badges, troféus e outros recursos cosméticos.   |
| Barra de progresso na disciplina   | Uma barra de progresso que acompanha a progressão do aluno na disciplina  |
| Tarefas  | Tarefas que podem ser acessadas pelo alunos   |
| Mural  | Quadro de avisos para os alunos, colocados pelos próprios alunos ou pelo professor e monitores para avisar sobre tarefas e lembretes |

## 5. Recursos do Produto

| Recurso  | Descrição dos Recursos |
| ------------- | ------------- |
| Agenda pessoal   | Na agenda, atividades individuais podem ser fixadas para organização própria do usuário. A agenda pode ser compartilhadas com outros usuários. |
| Enquetes  | Nesse ambiente, o professor poderá abrir enquetes para os alunos com questões levantadas em sala de aula. O ambiente de enquetes pode armazenar os dados para análises estatísticas posteriores.  |
| Controle de cadastro  | Os alunos matriculados na disciplina de Felicidade terão um cadastro na aplicação. O professor da disciplina terá o controle dos cadastros, podendo modificá-los.  |
| Marcador para o nível de felicidade   | O nível de felicidade individual do aluno deve ser mostrado em seu perfil individual. As variáveis e indicadores dos níveis de felicidade serão decididos posteriormente.  |
| Ambiente de grupos  | Na aplicação, será possível a criação de grupos. Nestes grupos, os membros poderão interagir mais facilmente. |
| Customização do perfil pessoal  | Conforme aspectos a serem definidos na gamificação, o aluno poderá personalizar o próprio perfil com recompensas recebidas das atividades propostas na matéria.   |
| Barra de progresso na disciplina   | Uma barra que acompanha a progressão do aluno será mostrada no perfil individual. As variáveis que alteram o nível de progresso serão definidas posteriormente.  |
| Tarefas  | As tarefas serão postadas pelo professor/monitor e poderão ser acessadas pelos alunos. Elas poderão ser fixadas na agenda. Completar tarefas pode aumentar os níveis de progresso e/ou felicidade do perfil de cada aluno.  |
| Mural  | Quadro de aviso para os alunos com lembretes de atividades a serem realizadas. Os lembretes podem ser colocados pelo professor, monitores ou alunos.
 |

## 6. Restrições
- O aplicativo deve estar utilizável para o usuário até o final de novembro de 2019.
- Deve-se desenvolver o aplicativo ao decorrer da matéria de Métodos de Desenvolvimento de Software e de Engenharia de Produto de Software, da Universidade de Brasília, é o mesmo deve ser desenvolvido pelo o grupo de estudantes designados.
- No processo de construção do aplicativo deve-se optar por ferramentas de baixo custo ou de ferramentas livres, que minimizem o custo final do projeto.
- O aplicativo deve permitir o acesso a internet.
- Deve possuir um meio de interação entre os alunos, monitores e professor.
- O aplicativo tem que ser uma plataforma cujo o aluno possa se sentir mais feliz ao utilizá-la.
- Deve ser implementado um sistema de guildas no aplicativo.
- Deve rodar em sistemas operacionais de smartphones(Android, IOS).


	
## 7. Intervalos de Qualidade
#### 7.1. Requisitos do Desempenho
O tempo de resposta do aplicativo depende da velocidade e qualidade da internet do aparelho, a conexão com a internet será essencial para interação do usuário com as funcionalidades do app. Assim como o tempo de execução irá depender da capacidade de processamento do aparelho.
#### 7.2. Requisitos de _Design_
O aplicativo terá interface sistemática e clara, cores variadas de acordo com o desempenho dos usuários e componentes gamificados.
#### 7.3. Requisitos de Portabilidade
Os usuários terão diferentes sistemas operacionais em seus dispositivos, portanto será necessária a portabilidade de um app que funcione em ambos os sistemas.
#### 7.4. Requisitos de Confiabilidade
Alguns dados deverão ser coletados de parte dos usuários e usados num meio acadêmico, desta forma é necessária boa segurança dos dados a serem coletados, transformados e apresentados.
#### 7.5. Requisitos de Privacidade
Como os dados coletados pelo app são para um meio acadêmico, apenas usuários com direito à gestão dos dados e do app poderão ter acesso a tais dados.

## 8. Prioridades e precedência
As prioridades da aplicação são: o controle das atividades da disciplina Felicidade, melhor compartilhamento de informações entre estudantes, monitores e o professor, e aumentar o engajamento dos usuários através da gamificação. Além disso, a aplicação deverá facilitar a obtenção de dados pelo professor, ajudando na avaliação dos alunos e na análise da disciplina como um todo.


***
