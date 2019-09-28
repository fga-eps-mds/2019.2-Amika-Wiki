## 1. Introdução
#### 1.1. Objetivo

Este documento tem como finalidade fornecer uma visão geral da arquitetura do projeto Amika: contém informações pertinentes sobre o modelo de arquitetura adotado, como diagramas que ilustram casos de uso, diagrama de pacotes, entre outros recursos.

#### 1.2. Escopo

Por meio desse documento, o leitor poderá entender o funcionando do sistema da aplicação Amika, bem como a abordagem usada no seu desenvolvimento. Desse modo, será possível ter uma compreensão ampla da arquitetura do Amika.

#### 1.3. Definições, Acrônimos e Abreviações

**Acrônimo/Abreviação** | **Definição**
------------------------|-------------------
UnB | Universidade de Brasília.

#### 1.4. Referências Bibliográficas
Angular. **Introduction to the Angular Docs**. Disponível em: https://angular.io/docs. Acesso em: 21 de Agosto de 2019. <br>
Django. **Django documentation**. Disponível em: https://docs.djangoproject.com/en/2.2/. Acesso em: 18 de Agosto de 2019. <br>
Django. **Models**. Disponível em: https://docs.djangoproject.com/en/2.2/topics/db/models/. Acesso em: 18 de Agosto de 2019. <br>
Django Rest Framework. **Django Rest Framework**. Disponível em: https://www.django-rest-framework.org/. Acesso em: 19 de Agosto de 2019. <br>
PostgreSQL. **About**. Disponível em: https://www.postgresql.org/about/. Acesso em: 21 de Agosto de 2019. <br>
UFRJ. **O Modelo Cliente Servidor**. Disponível em: https://www.gta.ufrj.br/ensino/eel878/redes1-2016-1/16_1/p2p/modelo.html. Acesso em: 18 de Agosto de 2019. <br>
UX Collective BR. **O que são Progressive Web Apps?**. Disponível em: https://brasil.uxdesign.cc/o-que-s%C3%A3o-progressive-web-apps-86e1b5306051. Acesso em: 19 de Agosto de 2019. <br>

#### 1.5. Visão Geral

**Tópico** | **Definição**
---------------|-----------------------------
Introdução | Descreve informações sobre a finalidade deste documento.
Representação Arquitetural | Traz uma descrição a respeito da arquitetura de software para melhor compreensão de sua estrutura e funcionamento. Além de mostrar a forma como ela está sendo representada.
Metas e Restrições | Traz uma descrição os requisitos e objetivos do software, e se esses têm algum impacto sobre a arquitetura.
Visão lógica | Traz uma descrição das partes relevantes relacionadas à arquitetura do modelo de design.
Backlog | Traz uma descrição da acumulação de trabalho: tudo o que deve ser feito do produto que vai ser desenvolvido.
Visão de implementação | Permite a visualização e entendimento de como o sistema será implementado e com quais tecnologias, semelhante ao que a Representação Arquitetural faz. Porém, explana como cada tecnologia é composta e distribui os serviços.

## 2. Representação Arquitetural

A arquitetura do Amika é composta por *frontend* e *backend* desacoplados, cada um possuindo seu próprio repositório. Por consequência desse desacoplamento, o risco de uma mudança em um dos dois não causará efeitos colaterais na implementação do outro. O modelo de arquitetura que será utilizada é o Cliente-Servidor. 

Cliente e Servidor é um modelo arquitetural em que a informação é dividida em plataformas independentes, cliente e servidor. Geralmente, o cliente faz requisições por meio de um protocolo específico e um servidor responde de acordo com a requisição que o foi passado. No Amika, o cliente é representado pelo Angular que irá realizar requisições *Hypertext Transfer Protocol* (HTTP) por meio do *Representational State Transfer* (REST) para o servidor, que é, nesse caso, o Django.

#### 2.1 Servidor

O servidor oferece serviços a processos usuários, ou seja, executam a tarefa solicitada e enviam uma resposta ao cliente que se traduz nos dados solicitados.

#### 2.1.1 Django
O Django é um framework com arquitetura baseada no modelo MVC, apesar disso, é descrita como *Model-View-Template* (MVT).
O MVT é uma arquitetura que separa as aplicações construídas com ela em três camadas. Essas camadas estão interconectadas e são: Model, View e Template.
- Model: é o modelo da aplicação, responsável por receber dados e interpretá-los para serem mostrados no Template. Ou seja, responsável pela escrita e leitura de dados.
- View: no django, tem o mesmo papel exercido pela controller em outros padrões de arquitetura, como no Rails, por exemplo. Recebe requisições e as trata, define qual template será mostrado ao usuário e qual model usar.
- Template: é apenas a camada de interação com o usuário, simplesmente mostra os dados ao usuário.


#### 2.1.2 Django REST Framework
O REST é uma extensão do Django Framework que permite implementar API's REST de forma rápida. A arquitetura REST opera por métodos de protocolo HTTP.

#### 2.1.3 PostgreSQL
É um banco de dados relacional. Relacional é a abordagem adotada nesse banco de dados e abordagem significa como os dados estão organizados. Na abordagem relacional os dados são dispostos em tabelas (linhas e colunas) e suas relações (chaves estrangeiras).

#### 2.2 Cliente 
O lado do cliente é responsável por solicitar um determinado serviço, através do envio de uma mensagem ao servidor e enquanto o processo servidor está trabalhando a solicitação, o cliente está livre para realizar outras tarefas.

#### 2.2.1 Angular
É um framework para criação de interfaces de aplicações. Para tal, utiliza  HTML, CSS e TypeScript. Por meio dele é possível desenvolver não somente para web, mas também para mobile. No Amika é utilizado para implementar todo o frontend respeitando a metodologia PWA.

#### 2.2.2 Progressive Web App (PWA)
Os PWA são páginas web tecnicamente regulares que podem aparecer ao usuário como aplicativos tradicionais ou aplicativos móveis. Em resumo, os PWA permitem que o usuário tenha uma experiência de uso muito próxima da de mobile apps. As principais funcionalidades oferecidas por essas tecnologias são:
- Push Notification;
- Ícone na tela home do smartphone;
- Splash screen;
- Processos rodando em background;
- Suporte a funcionamento em modo Offline;
- Acesso à camera e galeria;
- Acesso à geolocalização;
- Acesso à os contatos;



#### 2.3 Diagrama de relações
<br>
<div class="container">
	<div class="row">
		<div class="col-sm container-img">
			<img src="https://raw.githubusercontent.com/fga-eps-mds/2019.2-Amika-Wiki/master/assets/img/diagrama_relacoes_amika.png">
		</div>
	</div>
</div>
<br>

## 3. Objetivo e Restrições da arquitetura

#### 3.1. Requisitos para o Amika:
- Funcionar em web;
- Uso do PWA para funcionar em smartphones.

#### 3.2. Tecnologias utilizadas no Amika:
- Django: Web Framework baseada em Python;
- Django Rest Framework: caixa de ferramentas e API's para o Django;
- Python: Linguagem utilizada no Django;
- PWA: Software utilizado para implementação do uso em smartphones;
- Angular: Web Framework utilizada no frontend;
- Java Script: Linguagem utilizada, em conjunto com o HTML e CSS, para desenvolvimento WEB;
- HTML: Linguagem base utilizado em desenvolvimento WEB;
- CSS: Linguagem usada em conjunto HTML para estilizar a página.

## 4. Visão Lógica

#### 4.1. Visão Geral
O Amika é uma aplicação PWA composta da linguagem Python e do web framework django, usando HTML, CSS e o Angular no front-end. O objetivo do Amika é ser uma aplicação que facilite a comunicação e contato entre professor, alunos e monitores da disciplina de Felicidade ofertada na Universidade de Brasília no campus do Gama. À partir do banco de dados PostgreSQL, será possível armazenar dados dos alunos e das turmas, tanto atividades dos alunos que serão entregues pelos alunos por meio da aplicação quanto os dados básicos de cada aluno no meio acadêmico.

#### 4.2. Diagrama de Pacotes

<br>
<div class="container">
	<div class="row">
		<div class="col-sm container-img">
			<img src="https://raw.githubusercontent.com/fga-eps-mds/2019.2-Amika-Wiki/master/assets/img/diagrama_de_pacotes.png">
		</div>
	</div>
</div>
<br>

#### 4.3. Diagrama de Casos de Uso

<br>
<div class="container">
	<div class="row">
		<div class="col-sm container-img">
			<img src="https://raw.githubusercontent.com/fga-eps-mds/2019.2-Amika-Wiki/master/assets/img/diagrama_de_casos_de_uso.png">
		</div>
	</div>
</div>
<br>

#### 4.4. Diagrama de Classes

<br>
<div class="container">
	<div class="row">
		<div class="col-sm container-img">
			<img src="https://raw.githubusercontent.com/fga-eps-mds/2019.2-Amika-Wiki/master/assets/img/Diagrama_de_classes.png">
		</div>
	</div>
</div>
<br>


## 5. Backlog
O backlog representa a acumulação de trabalho: tudo o que deve ser feito do produto que vai ser desenvolvido. Basicamente, é uma pilha de itens a fazer, solicitados por alguém com base em suas necessidades/desejos, que devem ser entregues a quem solicitou depois que forem produzidos.
Os épicos levantados para o projeto são:
- 1) **_Perfil de administrador_**:
O projeto deve permitir a criação de usuários com algumas funcionalidades especiais, os administradores que vão gerenciar os usuários comuns, mandar notificações e gerenciar atividades.

- 2) **_Sistema de cadastro e login_**:
O projeto deve ter um sistema para os usuários comuns se autoregistrarem e gerenciarem seus dados, possibilitando a visualização e edição dos seus dados. Além disso, os administradores poderão cadastrar matrículas no sistema. Estas serão utilizadas na validação do autoregistro dos usuários.

- 3) **_Gerenciador de atividades_**:
O projeto deve conter um sistema gerenciador de atividades que deve possibilitar a criação de atividades por parte do administrador e a obtenção de respostas das respectivas atividades dos usuários comuns por meio de texto e anexos.

- 4) **_Área de compartilhamento_**:
O projeto deve possuir uma área de compartilhamento onde os usuários poderão compartilhar informações, opiniões, realizar enquetes e interagir entre si.

Os demais tópicos do backlog em detalhes podem ser consultados em: https://fga-eps-mds.github.io/2019.2-Amika-Wiki/#/docs/projeto/backlog 

## 6. Visão de implementação
#### 6.1. Django Rest Framework
Um projeto em Django é, geralmente, composto por diversas aplicações. Cada uma dessas aplicações é responsável por uma funcionalidade específica. Cada app é composto pelos seguintes diretórios e arquivos:
<ul>
    <li><strong>models.py:</strong> 
    <text style="font-size: 12px;">Este arquivo tem a função de implementar a camada model que, como explicado anteriormente, trabalha com a escrita e leitura de dados.</text></li>
    <li><strong>urls.py:</strong><text style="font-size: 12px;"> Funciona como um endpoint. Ou seja, provém o acesso aos templates(análogo à views no modelo MVC).</li>
    <li><strong>views.py:</strong><text style="font-size: 12px;"> Executa a camada view que recebe as requisições por meio dos métodos HTTP, trata-as e decide qual model será utilizada, e/ou template retornada ao usuário.</li>
    <li><strong>serializers.py:</strong><text style="font-size: 12px;"> É um destaque desse framework. Com ele objetos são transformados em arquivos JSON, e assim é possível, por exemplo, preencher listas com dados, e também torna possível o contrário: receber dados por um arquivo no formato JSON e criar objetos a partir desses dados.</li>
    <li><strong>tests.py:</strong><text style="font-size: 12px;"> Nele escrevemos todos os testes unitários que serão realizados na aplicação.</li>
</ul>

#### 6.2. PWA/Angular
Nesse projeto optou-se por construir a interface PWA com Angular. Sua organização é feita da seguinte forma:
<ul>
    <li><strong>app:</strong><text style="font-size: 12px;"> Pasta principal do projeto. Dentro dela estão os componentes e módulos de sua aplicação.</text></li>
    <li><strong>assets: </strong><text style="font-size: 12px;">Pasta onde estão armazenados os arquivos estáticos, como imagens e favicons.</text></li>
    <li><strong>app.components...: </strong><text style="font-size: 12px;">São os componentes da aplicação. Cada um tem seu próprio tipo. Podem ser entendidos como extensões de elementos que compõem o Modelo de Objeto de Documento (DOM em inglês). Estas extensões comunicam ao Angular para inserir alguma funcionalidade particular para esse elemento. A principal vantagem dos componentes é criar código reutilizável. </text></li>
    <li><strong>
    app.modules...: </strong><text style="font-size: 12px;">É onde cada módulo que compõe a aplicação é declarado. Toda aplicação construída com Angular é formada por módulos. Módulo é apenas uma maneira de agrupar os componentes, pipes, serviços e etc. Os módulos são unidos para formar a aplicação, e se encaixam como se fossem peças de quebra cabeça.</text></li>
<li><strong>
    app.services...: </strong><text style="font-size: 12px;">É utilizado para realizar a comunicação e o compartilhamento de informações entre classes que não têm acesso mútuo entre si.</text></li>
</ul>

