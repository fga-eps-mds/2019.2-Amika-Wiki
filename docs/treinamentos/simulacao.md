## Introdução

Neste treinamento, aplicaremos todos os conceitos estudados até o momento. Uma aplicação deverá ser desenvolvida em Django utilizando Docker como ambiente de desenvolvimento. As metodologias a serem seguidas deverão ser as ágeis Scrum, XP e Kanban. O versionameto do projeto devará seguir os padrões do Gitflow.

## Softwares Necessários
Para este projeto será necessário possuir Git, Docker e Docker Compose.  
Links para instalação:
* [Git](https://git-scm.com/)
* [Docker](https://www.docker.com/community-edition#/download)
* [Docker Compose](https://docs.docker.com/compose/install/)

### Repositório
Escolha uma forma de clonar o repositório deste projeto:
* HTTPS: ``` git clone https://github.com/MateusO97/Calculadora---Treinamento ```
* SSH: ``` git clone git@github.com:MateusO97/Calculadora---Treinamento.git ```

### Ambiente
Hora de rodar o projeto. Com o Docker rodando, navegue para o diretório do repositório clonado e rode o Docker Compose.

```bash
$ cd Calculadora---Treinamento
$ docker-compose up
```

E está pronto, a aplicação já está rodando. Abra o seu navegador na página `http://localhost:3000/` para ve-la funcionando!



<em>Caso os comandos acima não tenham funcionado, rode como sudo:</em>
```bash
$ sudo docker-compose up
```


## _Scrum City of Code_

O desafio deste treinamento é finalizar as _issues_ apresentadas neste repositório, mas seguindo o passo a passo do Scrum e utilizando dos conceitos aprendidos até o momento no tempo delimitado. Acompanhe as intruções a seguir:

### Planejamento da _Sprint_ [20 Minutos]

A primeira fase do treinamento será para planejar a _Sprint_ a ser executada. Nesta etapa, vocês terão um prazo de <b>10 Minutos</b> para conclui-la. Estes serão os passos dessa etapa:

  - Planning Poke: pontuar as _issues_ do backlog (Sugestão: em virtude do tempo, realizem a votação e decidam rapidamente pela maioria dos votos.)
  - Alocar Histórias: decidam quantas e quais _issues_ serão feitas nessa primeira _Sprint_, levem em consideração que teremos somente 2 _Sprints_.
  - Definir Pareamentos: montem as duplas, levando em consideração a passagem de conhecimento, e aloquem as histórias de cada dupla.
  
  
### Execução da _Sprint_ [1 semana]

Depois de definidos os pareamentos, é hora de colocar a mão no código! Nesta etapa, vocês terão um prazo de <b>30 minutos</b> para conclui-la. Levem em consideração os seguintes pontos:

  - Esquema Dojo: dentro da dupla, o desenvolvimento vai funcionar da seguinte forma: um dos membros começara como Piloto enquanto o outro irá sentar do seu lado sendo o Co-Piloto. O Piloto é o único que poderá tocar no código neste tempo, e enquanto ele estiver progamando, é seu dever falar em voz alta para o Co-Piloto tudo que estiver sendo feito. O Co-Piloto não poderá programar, mas pode falar para o Piloto o que ele deverá fazer e guia-lo caso necessário.
  - Daily: <b>10 Minutos por dia</b>, iremos parar as atividades e realizar um _Stand Up_, todos dirão, rapidamente, o que fizeram nesse tempo. Após o Daily, os Pilotos e Co-Pilotos inverterão os papéis.
  - Commits: os commits deverão ser atômicos (1 funcionalidade por commit) e devem seguir o esquema de branches do Gitflow. Os nomes das Branches criadas deverão seguir o seguinte padrão: <b>issue_x_nome_issue</b>, sendo "x" o número da _Issue_. 
- Pull Request: ao finalizar sua _Issue_, a dupla deverá criar um _Pull Request_ e solicitar a revisão e, se possível, a aceitação de outra dupla.
  
### Revisão da _Sprint_ [20 Minutos]

  - O que foi feito?: listar as _issues_ que foram finalizadas (_Pull Requests_ aceitos).
  - O que não foi feito?: listar as _issues_ que não foram finalizadas.
  - Porque não foi feito?: listar os problemas e dificuldades que impidiram de finalizar as _issues_.
  
### Retrospectiva da _Sprint_ [20 Minutos]

  - O que deu certo?: quais foram os pontos fortes da equipe nessa _Sprint_? O que funcionou melhor?
  - O que deu errado?: o que deu errado do que foi planejado? Quais fases menos funcionaram?
  - Como melhorar?: para uma próxima _Sprint_, o que poderia ser feito melhor? Quais medidas seriam interessantes? (Listar 3, uma que precisaria ocorrer imediatamente, uma que seria interessante, mas não fundamental e uma que poderia um dia ocorrer).


#### Comandos úteis do Docker
#### Como baixar uma imagem do docker
```bash
$ docker pull <imagem-desejada>
```

#### Listando imagens locais
```bash
$ docker images
```

#### Deletando imagens
```bash
$ docker rmi -f <id-da-imagem>
```

#### Listando contêineres em execução
```bash
$ docker ps
```

#### Removendo contêineres
```bash
$ docker rm [-f] <nome-do-contêiner-ou-id>
```

#### Execução de comandos de fora do contêiner
```bash
$ docker exec <nome-do-contêiner> <comando-desejado>
```

#### Comandos úteis do Django
#### Como criar migrações
```bash
$ python3 manage.py makemigrations
```

#### Como rodar migrações
```bash
$ python3 manage.py migrate
```

## Resultado

Os resultados adquiridos podem ser encontrados no seguinte repositório:
[Treinamento Calculadora](https://github.com/MateusO97/Calculadora---Treinamento)
O objetivo maior do treinamento era fornecer uma visão geral sobre o Scrum, e outras metodologias utilizadas no projeto, assim como dar para os membros de MDS um primeiro contato com uma tecnologia de desenvolvimento web, mesmo antes do tema do projeto em si ter sido definido.
