## 1. Introdução
#### 1.1. Objetivo

Este documento tem como finalidade fornecer uma visão geral da arquitetura do projeto Amika, contem informações pertinentes sobre qual o modelo de arquitetura adotado, diagramas que ilustram casos de uso, diagramas de classes, entre outros recursos .

#### 1.2. Escopo

Através desse documento, é possível obter um melhor entendimento da arquitetura do Gaia, permitindo ao leitor compreender o funcionamento de seu sistema, como também a abordagem utilizada para o seu desenvolvimento.

#### 1.3. Definições, Acrônimos e Abreviações

**Acrônimo/Abreviação** | **Definição**
------------------------|-------------------
UnB | Universidade de Brasília.

#### 1.4. Referências Bibliográficas

#### 1.5. Visão Geral

**Tópico** | **Definição**
---------------|-----------------------------
Introdução | Descreve informações sobre a finalidade deste documento.
Representação Arquitetural | Descreve qual é a arquitetura de software, para melhor compreensão de sua estrutura e funcionamento e mostra como ela está sendo representada.
Metas e Restrições | Descreve os requisitos e objetivos do software, e se estes  têm algum impacto sobre a arquitetura.
Visão lógica | Descreve as partes significativas do ponto de vista da arquitetura do modelo de design.

## 2. Representação Arquitetural

A arquitetura do Amika é composta por frontend e backend desacoplados, cada um possuindo seu próprio repositório. Por consequência desse desacoplamento, o risco de uma mudança em um dos dois não causará efeitos colaterais na implementação do outro. Podemos classificar a arquitetura como híbrida já que utiliza fundamentos de dois padrões arquiteturais, sendo eles: Cliente-Servidor e MVC. 

#### Cliente Servidor
É um modelo arquitetural em que a informação é dividida em plataformas independentes, cliente e servidor. Geralmente, o cliente faz requisições por meio de um protocolo específico e um servidor responde de acordo com o que foi passado para ele. No Amika o cliente é representado pela interface PWA que irá realizar requisições HTTP por meio do REST para o servidor, sendo nesse caso o Django. 

#### PWA (Progressive Web App)
Os PWA são páginas web tecnicamente regulares que podem aparecer ao usuário como aplicativos tradicionais ou aplicativos móveis. Em resumo, os PWA ter uma experiência de uso muito próxima da de mobile apps. As principais funcionalidades oferecidas por essas tecnologias são:
- Push Notification
- Ícone na tela home do smartphone
- Splash screen
- Processos rodando em background
- Suporte a funcionamento em modo Offline
- Acesso à camera e galeria
- Acesso à geolocalização
- Acesso à os contatos
- Django
- O Django é um framework com arquitetura baseada no MVC (Model-View-Controller), apesar disso, é descrita como MVT (Model-View-Template).

#### Django REST Framework
O REST é uma extensão do Django Framework que permite implementar API's REST de forma rápida. A arquitetura REST opera por métodos de protocolo HTTP.

#### Model View Template (MVT)
É uma arquitetura que separa as aplicações construídas com ela em três camadas. Essas camadas estão interconectadas e são: Model, View e Template.
- Model: é o modelo da aplicação, responsável por receber dados e interpretá-los para serem mostrados no Template. Ou seja, responsável pela escrita e leitura de dados.
- View: no django tem o mesmo papel exercido pela controller em outros padrões de arquitetura, como o Rails, por exemplo. Recebe requisições e as trata, define qual template será mostrado ao usuário e qual model usar.
- Template: é apenas a camada de interação com o usuário, simplesmente mostra os dados ao usuário.

#### PostgreSQL
É um banco de dados relacional. Relacional é a abordagem adotada nesse banco de dados e abordagem significa como os dados estão organizados. Na abordagem relacional os dados são dispostos em tabelas (linhas e colunas) e suas relações (chaves estrangeiras).

#### Angular
É um framework para criação de interfaces de aplicações. Para tal, utiliza  HTML, CSS e TypeScript. Por meio dele é possível desenvolver não somente para web, mas também para mobile. No Amika é utilizado para implementar todo o frontend respeitando a metodologia PWA.

## 3. Objetivo e Restrições da arquitetura

#### 3.1. Requisitos para o Amika:
- Funcionar em web.
- Uso do PWA, para funcionar em smartphones.

#### 3.2. Tecnologias utilizadas no Amika:
- Django: Web Framework baseada em Python.
- Django Rest Framework: caixa de ferramentas e APIs para o Django.
- Python: Linguagem utilizada no Django.
- PWA: Software utilizado para implementação do uso em smartphones.
- Angular: Web Framework utilizado no frontend.
- Java Script: Linguagem utilizado junto com o HTML e CSS, para desenvolvimento WEB.
- HTML: Linguagem base utilizado em desenvolvimento WEB.
- CSS: Linguagem usada juntamente com HTML para estilizar a pagina.


## 4. Visão Geral do Produto

## 5. Visão Lógica

## 6. Backlog
O backlog representa a acumulação de trabalho, tudo o que deve ser feito do produto que vai ser desenvolvido. Basicamente, é uma pilha de itens a fazer, solicitados por alguém com base em suas necessidades/desejos, que devem ser entregues a quem solicitou depois que forem produzidos.
Os épicos levantados para o projeto são:
- 1) Perfil de administrador:
	O projeto deve permitir a criação de usuários com algumas funcionalidades especiais, os administradores que vão gerenciar os usuários comuns, mandar notificações e gerenciar atividades.

- 2) Sistema de cadastro e login:
	O projeto deve ter um sistema para os usuários comuns se autoregistrarem e gerenciar seus dados, possibilitando a visualizar e editar os seus dados. Além disso, os administradores poderão cadastrar matrículas que serão utilizadas na validação do autoregistro dos usuários.

- 3) Gerenciador de atividades:
	O projeto deve conter um sistema gerenciador de atividades que deve possibilitar a criação de atividades por parte do administrador e a obtenção de respostas das respectivas atividades dos usuários comuns por meio de texto e anexos.

- 4) Área de compartilhamento:
	O projeto deve possuir uma área de compartilhamento onde os usuários poderão compartilhar informações, opiniões, realizar enquetes e interagir entre si.
***
